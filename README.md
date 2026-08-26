Новый адрес туннеля: `[https://af1c86106204f8.lhr.life/stream](https://af1c86106204f8.lhr.life/stream)`

#  Радио-Эфир

> **🔴 ПРЯМОЙ ЭФИР**  
> Ссылка на поток: [https://af1c86106204f8.lhr.life/stream](https://af1c86106204f8.lhr.life/stream)
ссылка неактивна из за таймаута а инструкция активна на август 2026
---

## 🛠️ Инструкция по запуску

### Шаг 1. Установка софта
```bash
sudo apt update
sudo apt install pavucontrol butt clementine icecast2 ssh

```

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


3. Нажмите **Play** в butt для старта эфира.
<img width="1920" height="1080" alt="изображение" src="https://github.com/user-attachments/assets/0b3b0228-8e59-42e7-8b08-b5b990bf2f99" />

### Шаг 4. Проброс туннеля в сеть

Запустите команду в терминале:

```bash
ssh -R 80:127.0.0.1:8000 nokey@localhost.run

```
<img width="1920" height="1080" alt="изображение" src="https://github.com/user-attachments/assets/b5556c9a-6cf4-4b76-8d9a-8a2e542a3103" />

---

## 👥 Команда проекта

* Артём Удмуртия
* Сергей Некто
* Иван Минутов (ИвМи)
* Ева Сырова
* Ироглефы бяо дзы

```

```
