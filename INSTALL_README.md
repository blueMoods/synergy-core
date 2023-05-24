

git clone https://github.com/symless/synergy-core.git
cd synergy-core/
sudo apt-get install curl
sudo apt-get install libssl-dev libcurl4-openssl-dev
sudo apt install qtcreator qtbase5-dev qttools5-dev cmake make g++ xorg-dev libssl-dev libx11-dev libsodium-dev libgl1-mesa-glx libegl1-mesa libcurl4-openssl-dev libavahi-compat-libdnssd-dev qtdeclarative5-dev libqt5svg5-dev libsystemd-dev 
cd ext
unzip gmock-1.6.0.zip -d gmock-1.6.0
unzip gtest-1.6.0.zip -d gtest-1.6.0
cd ../
mkdir build
cd build/
cmake ../
make
cd ../src/gui/
ls
qmake gui.pro
make
cd ../../bin