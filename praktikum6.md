

Ülesanne 1

a. /tmp/kaust/minufail.txt lugemiseks on vaja minimaalselt 500 kaustale ja 400 failile
b. /tmp/kaust/minufail.txt faili kustutamiseks on vaja minimaalselt 600 userile ja 700 kaustale

Ülesanne 2.

Miks antud käivitusõiguse andmine chmod a=x skriptifail ei ole piisav kesta/shelli-skripti (.sh) käivitamiseks? Selgita, millist õigust on lisaks vaja, et käivitada skriptifail?
Vaja on rx

Ülesanne 3

See hoiab ära olukorra, kus uued failid kuuluksid mingisse ühisesse üldgruppi (nt users), tehes need teistele süsteemi kasutajatele nähtavaks. Umask takistab teistel süsteemi kasutajatel neile automaatselt ligi pääseda

Ülesanne 4

marcus@Kikerpill26:/tmp/majasiseseks-kasutamiseks$ id && ls -la && cat uusfail.txt 
uid=1000(marcus) gid=1000(marcus) groups=1000(marcus),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),100(users),111(lpadmin),114(lxd)
total 4
drwxrwxr-x  2 root  majasisene  60 Oct 12 11:32 .
drwxrwxrwt 11 root  root       260 Oct 12 11:31 ..
----r--r--  1 user1 majasisene  27 Oct 12 11:32 uusfail.txt
Paar lauset.
 Nats tektsti
