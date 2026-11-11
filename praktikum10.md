





|Ülesanne  |Linux   |Windows|Linuxis kasutatud käsud|Windowsis kasutatud tööriist ja väli|
|---|---|---|---|---|
|1   |217   |150 |ps aux wc -l   |Task Manager -> Jõudlus -> Preotsessid |
|2  |/usr/lib/systemd/systemd   |smss.exe   |ps aux -> Start   |Process Explorer -> Start Time   |
|3 |avahi,_chrony,colord,cups-br+,lp,marcus,message+,polkitd,root,rtkit,syslog,systemd+ |UMFD-0, UMFD-1, MarcusAriston, SYSTEM,DWM-1   |  ps aux | awk '{print $1}' | sort | uniq  |Process Explorer -> User Name   |
|4   |14 min   | 26 min  |fastfetch -> Uptime   |Tegumihaldur -> Jõudlus -> Tööaeg   |
|5  |kworker/2:2-cgroup_free   |DismHost.exe   | ps aux -> start   |Process Explorer -> Start Time   |
|6 |htop ~2%   |Enim CPU aega võtab procexp64.exe 2-3%|htop -> CPU% |Process Explorer -> CPU Time   |
|7   |snapd   |Enim virtuaalmälu võtab msedgewebview2.exe   |   |Process Explorer -> Virtual Size   |
|8  |miriway-shell   |explorer.exe |   |htop -> RES   |
|9 |Füüsilisest mälust on hüivatud 1.63GB  ehk ~49% vaba on 1.67GB ehk ~51%|Füüsilisest mälust on hõivatud 2.6GB ehk 67% vaba on 1.4GB ehk 33%| htop -> Mem|Process Explorer -> System Information -> Physical Memory   |
|10   |7.3GB ehk ~31%   |Põhikettal on 21.3GB ehk ~34% vaba ruumi   |fastfetch -> Disk (/)   |File Explorer -> Kohalik ketas (C:)  |
|11  |Enim andmemahtu hõivav kaust on /usr ja suurim fail on Swap.img|Enim andmemahtu hõivav kaust on Windows ja suurim fail on Pagefile.sys   | `sudo du -h --max-depth=1 / 2>/dev/null \| sort -hr && sudo find / -type f -exec du -h {} + 2>/dev/null \| sort -hr \| head -n3`  |WizTree -> Size   |
|12   |   |   |   |   |
|13.1 |   |Enim kirjutab salvestusseadmele System   |   |Resource Monitor -> Disk -> Write   |
|13.2  |   |SLogFile   |   |Resource Monitor -> Disk Activity -> File   |
|13.3  |  | svchost.exe   |   |   |
|13.4  |   |arm64_microsoft.windows.common-controls_6595b64144ccf1df_6.0.26100.9711_none_3e07b80ee334e969\comctl32.dll   |   |Resource Monitor -> Disk -> Disk Activity -> Read|
|14  |   |   |   |   |
|15 |   |   |   |   |
<img width="1069" height="729" alt="Screenshot 2026-11-10 at 17 56 12" src="https://github.com/user-attachments/assets/0e875e75-9301-47b8-af45-1df9c314509c" />
