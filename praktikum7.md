


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
