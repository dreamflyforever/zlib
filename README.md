*  cross compiling
./configure --prefix=/home/opt/zlib-1.2.3/etc --shared  
modify Makefile file  
CC=mipsel-linux-gcc
LDSHARED=mipsel-linux-gcc -shared -Wl,-soname,libz.so.1  
CPP=mipsel-linux-gcc -E  
make && make install  
