

```markdown
# 📻 Мобильный Радио-Эфир

> **🔴 ПРЯМОЙ ЭФИР**  
> Ссылка на поток: [https://a548b766daa97f.lhr.life/stream](https://a548b766daa97f.lhr.life/stream)

---

## 🛠️ Инструкция по запуску

### Шаг 1. Установка софта
```bash
sudo apt update
sudo apt install pavucontrol butt clementine icecast2 ssh

```
<img width="1920" height="1080" alt="изображение" src="https://github.com/user-attachments/assets/a1d4ee0f-4720-4c0a-9c89-02f0dd9102c7" />
это для галочки

### Шаг 2. Настройка Icecast

Скопируйте конфиг и запустите сервер:

```bash
sudo cp /etc/icecast2/icecast.xml ~/icecast.xml
sudo chown $USER:$USER ~/icecast.xml
sed -i 's|/var/log/icecast2|/home/$USER|g' ~/icecast.xml
icecast2 -c ~/icecast.xml

```

### Шаг 3. Настройка butt и Clementine

1. Включите музыку в плеере **Clementine**.
2. В **butt** укажите параметры:
* **Server:** `127.0.0.1:8000`
* **Mountpoint:** `/stream`
* **Password:** `hackme`
<img width="1920" height="1080" alt="изображение" src="https://github.com/user-attachments/assets/d103bf25-8528-48f8-9d5c-ef7490d8c171" />


3. Нажмите **Play** в butt для старта эфира.

### Шаг 4. Проброс туннеля в сеть

Запустите команду в терминале:

```bash
ssh -R 80:127.0.0.1:8000 nokey@localhost.run

```
<img width="1920" height="1080" alt="изображение" src="https://github.com/user-attachments/assets/d950c5da-eee4-40a4-a9a5-da6e94f19714" />

---

## 👥 Команда проекта

* Артём Удмуртия
* Сергей Некто
* Иван Минутов (ИвМи)
* Ева Сырова
* Ироглефы бяо дзы

```

```
