# Домашнее задание к занятию 13.3. «Защита сети» - Ковбаса Анна

### Задание 1

Проведите разведку системы и определите, какие сетевые службы запущены на защищаемой системе:

**sudo nmap -sS < ip-адрес >**<br>
![sS](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sS.JPG)
![sSlog](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sS%20log.JPG)

**sudo nmap -sA < ip-адрес >**<br>
![sA](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sA.JPG)
![sAlog](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sA%20log.JPG)

**sudo nmap -sT < ip-адрес >**<br>
![sT](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sT.JPG)
![sTlog](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sT%20log.JPG)

**sudo nmap -sV < ip-адрес >**<br>
![sV](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sV.JPG)
![sVlog](https://github.com/kovbasaad/13-3-homework/blob/main/img/nmap%20sV%20log.JPG)

В логи Fail2Ban атаки не попали


------

### Задание 2

Проведите атаку на подбор пароля для службы SSH:

**hydra -L users.txt -P pass.txt < ip-адрес > ssh**

![hydra](https://github.com/kovbasaad/13-3-homework/blob/main/img/hydra.JPG)
![hydra-suricata](https://github.com/kovbasaad/13-3-homework/blob/main/img/hydra-suricata.JPG)
![hydra-fail2ban](https://github.com/kovbasaad/13-3-homework/blob/main/img/hydra-fail2ban.JPG)
