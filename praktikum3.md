# Praktikum 3 - Ubuntu paigaldamine ja LVM seadistus
---
Praktikumis 3 paigaldasin ja seadistasin LVM kettafailisüsteemiga Ubuntu 26.04 operatsioonisüsteemi,
muutsin töölauakeskkonna ressursisäästlikuks Lubuntuks ning tõestasin süsteemi toimimist ekraanipildiga käsu screenfetch väljundist ja töölauast (Pilt 1),
misjärel lisasin virtuaalmasinale täiendava 3 GB kõvaketta (/dev/vdb), laiendasin sellega vgextend ja lvextend abil olemasolevat volüümide gruppi
ning suurendasin resize2fs abil juurpartitsiooni (/) mahtu, mida kinnitavad kontrollkäskude sudo vgdisplay (Pilt 2), sudo lvdisplay (Pilt 3), lsblk (Pilt 4) ja df -h (Pilt 5) väljundid.

Pilt 1
<img width="1440" height="900" alt="Screenshot 2026-09-23 at 14 13 38" src="https://github.com/user-attachments/assets/4040d415-1bf9-4291-8163-7f6a80c66638" />

Pilt 2
<img width="1440" height="900" alt="Screenshot 2026-09-23 at 14 14 19" src="https://github.com/user-attachments/assets/03bb0bdb-e501-4889-9c99-c78a8a8dcc43" />

Pilt 3
<img width="1437" height="900" alt="Screenshot 2026-09-23 at 14 14 31" src="https://github.com/user-attachments/assets/f09b4304-3109-4793-861f-5c1d69cbe7a8" />

Pilt 4
<img width="1440" height="900" alt="Screenshot 2026-09-23 at 14 14 47" src="https://github.com/user-attachments/assets/db974a78-98dd-4f97-83d6-05109242f7fd" />

Pilt 5
<img width="1440" height="900" alt="Screenshot 2026-09-23 at 14 15 00" src="https://github.com/user-attachments/assets/b9f39f9a-db05-495e-8b91-76293feb2615" />
