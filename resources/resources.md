# Resources.md

query: /usr/bin/ld: cannot find Scrt1.o: No such file or directory
[How to fix linker error "cannot find crt1.o"?](https://stackoverflow.com/questions/6329887/how-to-fix-linker-error-cannot-find-crt1-o)




The problem is you likely only have the gcc for your current architecture and that's 64bit. You need the 32bit support files. For that, you need to install them


$ sudo apt install gcc-multilib


Alpine


$ apk add musl-dev
