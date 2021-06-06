# Discord-Account-Generator
For edu purpose only uses gmailnator and random username to gen the acc. Proof of concept of how the creation of Discord accounts can be automated without the need to type/click buttons on browser using XPATHS.

## About
A script that automates creating discord accounts. It shows how accounts can be created automatically without the user typing unless there is a captcha (h-Captcha just needs to be clicked) . It automatically verifies your Discord account via email for you and automatically saves login info in `login.txt` in `email:password:token` format. This is used for educational purposes only.

## Features
- Auto scrape email
- Random username from list
- Random password
- Random date
- Auto-email-verify
- Automatically get Discord token and other login info
- Proxy support
- Multi-threading

## Preview
![Picture](https://i.imgur.com/PSpaUEB.png)

## Usage
1. You can customize usernames by editing the usernames in discord_usernames.txt.
2. Run the file and use normal mode if you are a inexperienced with proxies and theading.

### Get Python
If you dont have python installed, download python and make sure you click on the 'ADD TO PATH' option during the installation.

### Run via Python
1. install the required modules
```
run requirements.bat
```

2. To run the script..
```
open discordgenerator.py or python it from cmd
```

#### Proxy support
- If you want to use proxies, simply paste the proxies in config/proxies.txt.  If you want to stop using proxies, just remove all the proxies from the .txt file. The script automatically checks for proxies on startup. HTTP proxies are only supported as of now. If the proxies are not alive, the script will throw a WebDriver error.

#### Threading mode 
- Uses multiple chrome windows
- Only run this when you have proxies or else one of you Chrome windows will get rate limited.
- Do put more than 6 threads unless you think your PC can handle it. I recommend using 2-3 threads.

#### No Threading
- This only uses one chrome window. 

#### FAQ
IF it doesnt open...
1. Make sure your chromedriver.exe file is the same version as your Chrome web browser version this one is 91 
2. Download the latest version chromedriver.exe: https://chromedriver.chromium.org/downloads
3. Then replace the chromedriver.exe file in the folder.

Where can i found my generated accounts?

1. It is located in the output folder. Open up login.txt to see the accounts 
that has been generated.
