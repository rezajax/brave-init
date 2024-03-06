# brave requirements 
apt-get install build-essential python-setuptools python3-distutils 

# rez requirements
apt install git curl wget



# install nvm for npm 
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
nvm install --lts

---

git clone https://github.com/brave/brave-browser.git

npm install

**the Chromium source is downloaded, which has a large history (gigabytes of data)**\
**this might take really long to finish depending on internet speed**\

npm run init


npm run init -- --target_os=android --target_arch=arm


This shell script only works on Debian and Ubuntu but check system requirements for other distros:\
**cd to brave-browser repo root**\
./src/build/install-build-deps.sh # for Linux

# this not working for me!
Use ./src/build/install-build-deps.sh --android for Android builds.


npm run build -- Debug --target_os=android --target_arch=arm --target_android_output_format=apk
