## Creted By Ziddi Hacker 2

# Please install Requirements Tools

sudo apt install tshark

sudo apt install sox

sudo apt install lolcat

#  Run:

chmod 777 pcap2wav

./pcap2wav

# Usage:

  ./pcap2wav [options] filename.pcap [target filename]
  

Script attempts to create a few files: a .<codec> file and a .wav file for each RTP stream
  

It requires Tshark to be installed on the system. If a codec other than PCMA or PCMU

is used then the script will attempt to use fs_cli to decode and create a wav.

Supported codecs:

 PCMU (G711 ulaw)
 
 PCMA (G711 Alaw)
 
 GSM
 
 G722 (requires fs_encode)
 
 G729 (requres fs_encode with mod_com_g729)

Supported options:

 -z  Perform "clean and zip" - After converting to wav files the program will "clean up"
 
                               by putting the wav files into a .tgz file and then removing
                               
                               the .wav and .<codec> files from the disk.
# Credit By Ziddi Hacker 2
