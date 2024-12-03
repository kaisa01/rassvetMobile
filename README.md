# framework kivyMD
pip install kivymd

# install buildozer
pip3 install --user --upgrade buildozer

# Android on Ubuntu 20.04 and 22.04 (64bit)
sudo apt update
sudo apt install -y git zip unzip openjdk-17-jdk python3-pip autoconf libtool pkg-config zlib1g-dev libncurses5-dev libncursesw5-dev libtinfo5 cmake libffi-dev libssl-dev
pip3 install --user --upgrade Cython==0.29.33 virtualenv  # the --user should be removed if you do this in a venv

# add the following line at the end of your ~/.bashrc file
export PATH=$PATH:~/.local/bin/

# create apk
buildozer android debug deploy run
