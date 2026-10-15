# Praktikum 6 Failiõigused Linuxis
---
Selles praktikumis tutvusin Linuxi failisüsteemi pääsuõigustega, määramasin ja haldasin failide ning kataloogide õigusi, omanikke ja täiendavaid atribuute.

# Ülesanne 1

a. /tmp/kaust/minufail.txt lugemiseks on vaja minimaalselt 500 kaustale ja 400 failile

b. /tmp/kaust/minufail.txt faili kustutamiseks on vaja minimaalselt 600 userile ja 700 kaustale

# Ülesanne 2.

Miks antud käivitusõiguse andmine chmod a=x skriptifail ei ole piisav kesta/shelli-skripti (.sh) käivitamiseks? Selgita, millist õigust on lisaks vaja, et käivitada skriptifail?
Vaja on rx

# Ülesanne 3

See hoiab ära olukorra, kus uued failid kuuluksid mingisse ühisesse üldgruppi (nt users), tehes need teistele süsteemi kasutajatele nähtavaks. Umask takistab teistel süsteemi kasutajatel neile automaatselt ligi pääseda

# Ülesanne 4

marcus@Kikerpill26:/tmp/majasiseseks-kasutamiseks$ id && ls -la && cat uusfail.txt 

uid=1000(marcus) gid=1000(marcus) groups=1000(marcus),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),100(users),111(lpadmin),114(lxd)

total 4

drwxrwxr-x  2 root  majasisene  60 Oct 12 11:32 .
drwxrwxrwt 11 root  root       260 Oct 12 11:31 ..
----r--r--  1 user1 majasisene  27 Oct 12 11:32 uusfail.txt

Paar lauset.
 Nats tektsti

# Ülesanne 5

Setuid õigust on vaja selleks, et tavakasutaja saaks programmi käivitada faili omaniku õigustes (nt. parooli vahetamiseks /etc/passwd failis)

<img width="424" height="157" alt="Screenshot 2026-10-13 at 17 29 19" src="https://github.com/user-attachments/assets/4a6ab742-c612-43cb-a9ed-b5d2d597f814" />

# Ülesanne 6

Pigem tõstab see turvalisust, sest kasutajatele ei pea andma laiu root-õigusi igapäevasteks tegevusteks, kuid samas see vähendab turvalisust hetkel, kui konkreetse programmi kood on vigane (nt. bufferoverflow).


# Ülesanne 7

Peeter, opetaja, root, marcus


# Ülesanne 8

-rw-rw----+ 1 opetaja opetaja   125 Oct 13 17:48 hinded.txt 
Mida märkad käsutulemuses ls -la õigustes? - Õiguste rea lõpus olev + annab märku, et sellel failil on kasutusel ACL laiendatud õigused.

'#' file: hinded.txt

'#' owner: opetaja

'#' group: opetaja

user::rw-

group::---

group:direktor:rw-

mask::rw-

other::---


# Ülesanne 9

Kes saab +i (immutable) atribuudiga faili sisu muuta (kirjutada)?

Mitte keegi (read only)
Milliste käskudega (ja millises järjekorras) on võimalik sellist faili siiski süsteemist kustutada?

sudo chattr -i testfail-2
sudo rm -f testfail-2
