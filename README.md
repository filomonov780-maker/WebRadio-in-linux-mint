
# Радио-Эфир

все что надо скачать в конце!!!!!

> **🔴 ПРЯМОЙ ЭФИР**  
> Ссылка на поток: [https://49cd0c2a183322.lhr.life/stream](https://49cd0c2a183322.lhr.life/stream)

---

## 🛠️ Инструкция по запуску

### Шаг 1. Настройка Icecast
Скопируйте конфиг и запустите сервер:
```bash
sudo cp /etc/icecast2/icecast.xml ~/icecast.xml
sudo chown $USER:$USER ~/icecast.xml
sed -i 's|/var/log/icecast2|/home/$USER|g' ~/icecast.xml
icecast2 -c ~/icecast.xml

```

### Шаг 2. Настройка butt и Clementine

1. Включите музыку в плеере **Clementine**.
2. В **butt** укажите параметры:
* **Server:** `127.0.0.1:8000`
* **Mountpoint:** `/stream`
* **Password:** `hackme`


3. Нажмите **Play** в butt для старта эфира.

### Шаг 3. Проброс туннеля в сеть

Запустите команду в терминале:

```bash
ssh -R 80:127.0.0.1:8000 nokey@localhost.run

```

---

## 👥 Команда проекта

* Артём Удмуртия
* Сергей Некто
* Иван Минутов (ИвМи)
* Ева Сырова
* Ироглефы бяо дзы

```
sudo apt update
sudo apt install pavucontrol
sudo apt install butt
sudo apt install clementine
sudo apt install icecast2
sudo apt install ssh
```
