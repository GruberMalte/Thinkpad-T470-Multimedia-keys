# Thinkpad-T470-Multimedia-keys
A quick and dirty key mapping tool for keys not accessible in ubuntu

I found that some keys on my keyboard are not avalible in
'''
/dev/input/eventX
'''
Instead this file reads the file
'''
/dev/kmsg
'''
and listens to error messages about keys.
If a error message is issued it's key code is parsed.


#Setup
Compile the program using 
'''
gcc -o main main.c -lX11 -lXtst 
'''
Make sure to have installed libxtst
'''
sudo apt-get install libxtst-dev
'''







