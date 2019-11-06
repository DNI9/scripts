## Compress Android sources

### Install:
    sudo apt install repo bc pxz wput
or

    sudo apt-get install repo bc pxz wput
    
### Compress It:
    export XZ_OPT=-9e
    tar -I pxz -cf - * | split -b 4500M - ROMNAME.tar.xz.
    
### Extract It:

    cat *.tar.xz* | tar -xvJf - -i
    
Credits:
[This](https://github.com/SamarV-121/SamarV-121.github.io) & [This](https://github.com/regalstreak/skadoosh) 
