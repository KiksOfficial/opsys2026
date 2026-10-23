



# Ülesanne 1

Uued andmekandjad vajavad lähtestamist, kuna neil puuduvad sageli vajalikud partitsioonitabelid ja ühilduvad failisüsteemid.
Lähtestamise käigus luuakse andmekandjale uus loogiline struktuur, mis annab kasutajale täieliku kontrolli partitsioonide ja nende suuruse üle.
Samuti võimaldab see kohandada failisüsteemi (nt NTFS, ext4 või exFAT) konkreetse operatsioonisüsteemi nõuetele vastavaks.
See tagab seadme korrektse toimimise arvutis.

# Ülesanne 2

MBR partitsioonitabel piirdub 2TB-ga ning sellel saab olla maksimaalselt 4 partitsiooni. GPT on vajalik ka UEFI süsteemides (tänapäeval on BIOS asendunud UEFI-ga).
Võrreldes MBR-iga pakuvad GPT varundustabelid (backup tables) paremat kaitset andmekao eest, mis on tingitud partitsioonitabeli korruptsioonist.

# Ülesanne 3

https://kodu.ut.ee/~marcusariston/opsys/hdd.png

# Ülesanne 4

<img width="1440" height="899" alt="Screenshot 2026-10-22 at 08 20 13" src="https://github.com/user-attachments/assets/4b4345cf-370e-4761-8919-74a8aa56c4bb" />

# Ülesanne 5

mount parameetrid -o -ro tähendavad, et mount käivitatakse täpsustavate valikutega, milleks praegu on ro ehk read only
-t auto puhul tähendab -t failisysteemi tüüpi, auto selle taga tähendab, et mount proovib ise automaatselt tuvastada failisüsteemi tüüpi kasutades selleks libblkid library.

# Ülesanne 6

Ubuntu asendas auto parameetri ext4-ga

# Ülesanne 7
<img width="1440" height="900" alt="Screenshot 2026-10-23 at 10 35 10" src="https://github.com/user-attachments/assets/1d73d017-6771-4f75-b300-a8299881b5eb" />
