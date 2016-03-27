# A2SV
Auto Scanning to SSL Vulnerability v1.3.0



         █████╗ ██████╗ ███████╗██╗   ██╗
        ██╔══██╗╚════██╗██╔════╝██║   ██║
        ███████║ █████╔╝███████╗██║   ██║
        ██╔══██║██╔═══╝ ╚════██║╚██╗ ██╔╝
        ██║  ██║███████╗███████║ ╚████╔╝ 
        ╚═╝  ╚═╝╚══════╝╚══════╝  ╚═══╝ 
      [Auto Scanning to SSL Vulnerability]
          [By Hahwul / www.hahwul.com]
________________________________________________

### 1. A2SV?
Auto Scanning to SSL Vulnerability.<br>
HeartBleed, CCS Injection, SSLv3 POODLE, FREAK... etc <br>
 + [OK] heartbleed
 + [OK] ccs injection
 + [OK] SSLv3 POODLE
 + [OK] FREAK Attack
 + [OK] LOGJAM Attack
 + [PLAN] SSL ACCF
 + [PLAN] DROWN Attack

### 2. How to Install?
A. Download(clone) & Unpack A2SV
> git clone https://github.com/hahwul/a2sv.git<br>
> cd a2sv<br>

B. Install Python Package<br>
> pip install argparse<br>
> pip install netaddr<br>

C. Run A2SV<br>
> python a2sv.py -h

### 3. How to Use?
usage: a2sv.py [-h] [-t TARGET] [-p PORT] [-m MODULE] [-v]<br>
<br>
optional arguments:<br>
  -h, --help            show this help message and exit<br>
  -t TARGET, --target TARGET<br>
                        Target URL/IP Address<br>
  -p PORT, --port PORT  Custom Port / Default: 443<br>
  -m MODULE, --module MODULE<br>
                        Check Module<br>
  -v, --version         Show Version<br>
<br>
ex)<br>
python a2sv.py -t 127.0.0.1<br>
python a2sv.py -t 127.0.0.1 -m heartbleed<br>
python a2sv.py -t 127.0.0.1 -p 8111<br>
<br>
### 4. Support
Contact hahwul@gmail.com
<br>
### 5. Code Reference Site
poodle : https://github.com/supersam654/Poodle-Checker<br>
heartbleed : https://github.com/sensepost/heartbleed-poc<br>
ccs injection : https://github.com/Tripwire/OpenSSL-CCS-Inject-Test<br>
freak : https://gist.github.com/martinseener/d50473228719a9554e6a<br>
