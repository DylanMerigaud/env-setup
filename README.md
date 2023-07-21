# env-setup

10/28/2021 | Tested on Windows 11 22000

Admin PowerShell
```
wsl --install
```

Ubuntu WSL2
```
cd /tmp
sudo apt update
sudo apt upgrade
sudo apt install zsh
chsh -s $(which zsh)
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
nvm install node
npm install -g yarn
wget https://release.gitkraken.com/linux/gitkraken-amd64.deb
rm -rf /usr/share/gitkraken/
sudo apt-get install ./gitkraken-amd64.deb
download from https://t.me/gitkrakencrackchat
cd GitCracken/
yarn install
yarn build
sudo "$(nvm which node)" dist/bin/gitcracken.js patcher
echo '\nexport PATH="$PATH:$(yarn global bin)"\n' >> ~/.zshrc
```
