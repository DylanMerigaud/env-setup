# env-setup

10/28/2021 | Tested on Windows 11 22000

Admin PowerShell
```
wsl --install
```

Ubuntu WSL2
```
mkdir Downloads
cd ~/Downloads
sudo apt update
sudo apt upgrade
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
nvm install-latest-npm
npm install -g yarn
wget https://release.gitkraken.com/linux/gitkraken-amd64.deb
sudo apt-get install ./gitkraken-amd64.deb
git clone https://github.com/5cr1pt/GitCracken.git #(https://github.com/5cr1pt/GitCracken/pull/79)
cd GitCracken/GitCracken/
yarn install
yarn build
sudo "$(nvm which node)" dist/bin/gitcracken.js patcher
echo '\nexport PATH="$PATH:$(yarn global bin)"\n' >> ~/.zshrc
```
