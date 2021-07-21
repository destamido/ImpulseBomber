# ImpulseBomber — современный набор инструментов для DDoS.

## Главное окно:
<p align="center">
  <img src="https://i.imgur.com/Eu0dMdP.png">
</p>

## Методы:
| Метод               |   Цель   | Описание |
| ---------------------| -----------|-------------|
| SMS                  | PHONE     | Отправляет огромное количество SMS-сообщений и звонков одной цели. |
| EMAIL                | EMAIL     | Отправляет большое количество сообщений на введённую электронную почту. |
| NTP                  | IP:PORT    | Усиление NTP — тип распределённой атаки DoS, при которой злоумышленник использует общедоступные серверы протокола сетевого времени (NTP), чтобы перегрузить целевой трафик с помощью протокола пользовательских дейтаграмм (UDP). |
| SYN                  | IP:PORT    | SYN-флуд (полуоткрытая атака) — тип атаки DoS, цель которой — сделать сервер недоступным для легитимного трафика, потребляя все доступные ресурсы сервера. |
| UDP                  | IP:PORT    | UDP-лавинная рассылка — тип атаки DoS, при которой большое количество пакетов протокола пользовательских дейтаграмм (UDP) отправляется на целевой сервер с целью подавить способность этого устройства обрабатывать и отвечать. Брандмауэр, защищающий целевой сервер, также может выйти из строя в результате лавинной рассылки UDP, что приведет к отказу в обслуживании легитимного трафика. |
| POD (Ping of Death)  | IP         | Ping of Death (PoD) — тип атаки DoS, при которой злоумышленник пытается вывести из строя, дестабилизировать или заморозить целевой компьютер или службу, отправив неверно сформированные или слишком большие пакеты с помощью простой команды "ping". |
| ICMP                 | IP:PORT    | Ping-флуд, также известный как ICMP-флуд, представляет собой распространенную атаку DoS, при которой злоумышленник выключает компьютер жертвы, подавляя его эхо-запросами ICMP, также известными как эхо-запросы. |
| HTTP                 | URL        | HTTP Flood — тип распределенного DDoS, при котором злоумышленник манипулирует нежелательными запросами HTTP и POST, чтобы атаковать веб-сервер или приложение. В этих атаках часто используются взаимосвязанные компьютеры, которые были захвачены с помощью вредоносных программ, таких как троянские кони. |
| Slowloris            | IP:PORT    | Slowloris — программа атаки DDos, которая позволяет злоумышленнику перегрузить целевой сервер, открывая и поддерживая множество одновременных HTTP-соединений между злоумышленником и целью. |
| Memcached            | IP:PORT    | Распределенная атака DDoS-memcached — тип кибератаки, при которой злоумышленник пытается перегрузить целевую жертву интернет-трафиком. Злоумышленник подделывает запросы к уязвимому UDP-серверу memcached, который затем наводняет целевую жертву интернет-трафиком, потенциально перегружая ресурсы жертвы. В то время как интернет-инфраструктура цели перегружена, новые запросы не могут быть обработаны, а обычный трафик не может получить доступ к интернет-ресурсу, что приводит к отказу в обслуживании. |

## Установка:
* Windows:
  * Загрузить Python 3.8 отсюда — [ссылка](https://www.python.org/downloads/release/python-38).
  * Запустить установщик, нажать "add python to PATH".
  * Загрузить Impulse.
  * Открыть командную строку (cmd) или Powershell в директории Impulse.
  * Запустить команду: `pip install -r requirements.txt`.
  * Потом эту: `python impulse.py --help`.


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
