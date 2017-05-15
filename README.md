# libubox
#Instalacion de libubux

git clone git@github.com:aquiles19/libubox.git /opt/git/libubox
cd /opt/git/libubox/

cmake CMakeLists.txt -DBUILD_LUA=OFF

make

sudo make install
sudo ln -sf /usr/local/lib/libubox.so /usr/lib/libubox.so
sudo mkdir -p /usr/share/libubox
sudo ln -sf /usr/local/share/libubox/jshn.sh /usr/share/libubox/jshn.sh
