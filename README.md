# ImpulseBomber — современный набор инструментов для DDoS.

## Главное окно:
<p align="center">
  <img src="https://i.imgur.com/Eu0dMdP.png">
</p>

## Методы:
| Метод               |   Цель   | Описание |
| ---------------------| -----------|-------------|
| SMS                  | PHONE     | Отправляет огромное количество SMS-сообщений и звонков одной цели |
| EMAIL                | EMAIL     | Отправляет большое количество сообщений электронной почты адресату |
| NTP                  | IP:PORT    | Усиление NTP — это тип распределенной атаки типа отказ в обслуживании (DDoS), при которой злоумышленник использует общедоступные серверы протокола сетевого времени (NTP), чтобы перегрузить целевой трафик с помощью протокола пользовательских дейтаграмм (UDP). |
| SYN                  | IP:PORT    | SYN-флуд (полуоткрытая атака) — это тип атаки типа «отказ в обслуживании» (DDoS), цель которой — сделать сервер недоступным для легитимного трафика, потребляя все доступные ресурсы сервера. |
| UDP                  | IP:PORT    | A UDP flood is a type of denial-of-service attack in which a large number of User Datagram Protocol (UDP) packets are sent to a targeted server with the aim of overwhelming that device’s ability to process and respond. The firewall protecting the targeted server can also become exhausted as a result of UDP flooding, resulting in a denial-of-service to legitimate traffic. |
| POD (Ping of Death)  | IP         | Ping of Death (a.k.a. PoD) is a type of Denial of Service (DoS) attack in which an attacker attempts to crash, destabilize, or freeze the targeted computer or service by sending malformed or oversized packets using a simple ping command. |
| ICMP                 | IP:PORT    | Ping flood, also known as ICMP flood, is a common Denial of Service (DoS) attack in which an attacker takes down a victim's computer by overwhelming it with ICMP echo requests, also known as pings. |
| HTTP                 | URL        | HTTP Flood is a type of Distributed Denial of Service (DDoS) attack in which the attacker manipulates HTTP and POST unwanted requests in order to attack a web server or application. These attacks often use interconnected computers that have been taken over with the aid of malware such as Trojan Horses. |
| Slowloris            | IP:PORT    | Slowloris is a denial-of-service attack program which allows an attacker to overwhelm a targeted server by opening and maintaining many simultaneous HTTP connections between the attacker and the target. |
| Memcached            | IP:PORT    | A memcached distributed denial-of-service (DDoS) attack is a type of cyber attack in which an attacker attempts to overload a targeted victim with internet traffic. The attacker spoofs requests to a vulnerable UDP memcached* server, which then floods a targeted victim with internet traffic, potentially overwhelming the victim’s resources. While the target’s internet infrastructure is overloaded, new requests cannot be processed and regular traffic is unable to access the internet resource, resulting in denial-of-service. |

## Установка:
* Windows:
  * Загрузить Python 3.8 [отсюда](https://www.python.org/downloads/release/python-38).
  * Запустить установщик, нажать `add python to PATH`.
  * Загрузить 'Impulse Bomber'.
  * Открыть 'cmd' или 'powershell' в директории 'Impulse'.
  * Запустить эту команду: `pip install -r requirements.txt`.
  * После чего, эту: `python impulse.py --help`.

* Linux:
  * `sudo apt update`.
  * `sudo apt install python3 python3-pip git -y`.
  * `git clone https://github.com/damiolka/ImpulseBomber`.
  * `cd Impulse/`.
  * `pip3 install -r requirements.txt`.
  * `python3 impulse.py --help`.

* Termux:
  * `pkg update`.
  * `pkg install python3 python3-pip git -y`.
  * `git clone https://github.com/damiolka/ImpulseBomber`.
  * `cd Impulse/`.
  * `pip3 install -r requirements.txt`.
  * `python3 impulse.py --help`.

## Пример флуда SMS и звонками:
```python impulse.py --method SMS --time 20 --threads 15 --target +79771234567```

<p align="center">
  <img src="https://i.imgur.com/ZpPAJyD.png">
</p>

Создано destamido (ex. damiolka).
