apt-get install build-essential python-setuptools python3-distutils 

# install nvm for npm 
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

apt install git curl wget


git clone https://github.com/brave/brave-browser.git

npm install

# the Chromium source is downloaded, which has a large history (gigabytes of data)
# this might take really long to finish depending on internet speed

npm run init


# cd to brave-browser repo root
./src/build/install-build-deps.sh # for Linux
