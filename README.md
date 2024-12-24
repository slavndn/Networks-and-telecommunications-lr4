# Славный Даниил Михайлович - Исследование транспортного уровня

1. Провел исследование открытых соединений на компьютере с помощью утилиты Netstat: 

```
C:\Windows\System32>netstat

Активные подключения

  Имя    Локальный адрес        Внешний адрес          Состояние
  TCP    127.0.0.1:49726        linuxoid:49727         ESTABLISHED
  TCP    127.0.0.1:49727        linuxoid:49726         ESTABLISHED
  TCP    127.0.0.1:49728        linuxoid:49729         ESTABLISHED
  TCP    127.0.0.1:49729        linuxoid:49728         ESTABLISHED
  TCP    127.0.0.1:49733        linuxoid:49734         ESTABLISHED
  TCP    127.0.0.1:49734        linuxoid:49733         ESTABLISHED
  TCP    127.0.0.1:49735        linuxoid:49736         ESTABLISHED
  TCP    127.0.0.1:49736        linuxoid:49735         ESTABLISHED
  TCP    192.168.1.63:54546     149.154.167.99:https   ESTABLISHED
  TCP    192.168.1.63:54654     xiva-daria:https       ESTABLISHED
  TCP    192.168.1.63:54657     lm-in-f188:5228        ESTABLISHED
  TCP    192.168.1.63:54664     api:https              ESTABLISHED
  TCP    192.168.1.63:54666     yandex:https           ESTABLISHED
  TCP    192.168.1.63:54678     yabs:https             ESTABLISHED
  TCP    192.168.1.63:54689     api:https              ESTABLISHED
  TCP    192.168.1.63:54729     mc:https               ESTABLISHED
  TCP    192.168.1.63:54735     api:https              ESTABLISHED
  TCP    192.168.1.63:54755     a2-18-121-72:https     ESTABLISHED
  TCP    192.168.1.63:54784     router:domain          TIME_WAIT
  TCP    192.168.1.63:54785     router:domain          TIME_WAIT
  TCP    192.168.1.63:54787     router:domain          TIME_WAIT
  TCP    192.168.1.63:54788     router:domain          TIME_WAIT
  TCP    192.168.1.63:54789     router:domain          TIME_WAIT
  TCP    192.168.1.63:54791     router:domain          TIME_WAIT
  TCP    192.168.1.63:54794     router:domain          TIME_WAIT
  TCP    192.168.1.63:54797     router:domain          TIME_WAIT
  TCP    192.168.1.63:54798     router:domain          TIME_WAIT
  TCP    192.168.1.63:54800     static:https           TIME_WAIT
  TCP    192.168.1.63:54802     router:domain          TIME_WAIT
  TCP    192.168.1.63:54803     router:domain          TIME_WAIT
  TCP    192.168.1.63:54805     router:domain          TIME_WAIT
  TCP    192.168.1.63:54806     router:domain          TIME_WAIT
  TCP    192.168.1.63:54808     router:domain          TIME_WAIT
  TCP    192.168.1.63:54809     router:domain          TIME_WAIT
```

2. Исследую открытые порты 'GitHub'

```
C:\Windows\System32>nmap -v github.com
Starting Nmap 7.95 ( https://nmap.org ) at 2024-12-24 16:40 RTZ 2 (чшьр)
Initiating Ping Scan at 16:40
Scanning github.com (140.82.121.3) [4 ports]
Completed Ping Scan at 16:40, 0.05s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 16:40
Completed Parallel DNS resolution of 1 host. at 16:40, 0.07s elapsed
Initiating SYN Stealth Scan at 16:40
Scanning github.com (140.82.121.3) [1000 ports]
Discovered open port 80/tcp on 140.82.121.3
Discovered open port 443/tcp on 140.82.121.3
Discovered open port 22/tcp on 140.82.121.3
Completed SYN Stealth Scan at 16:40, 5.04s elapsed (1000 total ports)
Nmap scan report for github.com (140.82.121.3)
Host is up (0.011s latency).
rDNS record for 140.82.121.3: lb-140-82-121-3-fra.github.com
Not shown: 997 filtered tcp ports (no-response)
PORT    STATE SERVICE
22/tcp  open  ssh
80/tcp  open  http
443/tcp open  https
```

```
PORT    STATE SERVICE
22/tcp  open  ssh
80/tcp  open  http
443/tcp open  https
```

3. Исследую открытые порты 'scanme.nmap.org' Это официальный сайт проекта Nmap для тестирования

```
PORT      STATE    SERVICE
22/tcp    open     ssh
80/tcp    open     http
135/tcp   filtered msrpc
139/tcp   filtered netbios-ssn
445/tcp   filtered microsoft-ds
9929/tcp  open     nping-echo
31337/tcp open     Elite
```

4. Исследую открытые порты 'demo.testfire.net' Демонстрационный сайт для анализа безопасности от IBM

```
PORT     STATE  SERVICE
80/tcp   open   http
443/tcp  open   https
8080/tcp open   http-proxy
8443/tcp closed https-alt
```

5. Скриншоты:

![image](https://github.com/user-attachments/assets/dbf69027-0cb5-40cc-9367-bdd4b31a7f17)

![image](https://github.com/user-attachments/assets/d7df6134-28a4-42b6-b3bb-0a16afa77eae)

![image](https://github.com/user-attachments/assets/e3dca08f-5a02-4e8b-a08c-e7794d46af5a)

![image](https://github.com/user-attachments/assets/75110b9c-81c9-4b6d-a870-b5dcc188dd3f)





