# Мобильный Радио-Эфир

> ** ПРЯМОЙ ЭФИР**  
> Ссылка на поток: [https://19fdf0b160f5bc.lhr.life/stream](https://19fdf0b160f5bc.lhr.life/stream)

---

## 🛠️ Инструкция по запуску

### Шаг 1. Настройка Icecast
Скопируйте конфиг и запустите сервер:
```bash
sudo cp /etc/icecast2/icecast.xml ~/icecast.xml
sudo chown $USER:$USER ~/icecast.xml
sed -i 's|/var/log/icecast2|/home/$USER|g' ~/icecast.xml
icecast2 -c ~/icecast.xml

Шаг 2. Настройка butt и Clementine

    Включите музыку в плеере Clementine.

    В butt укажите параметры:

        Server: 127.0.0.1:8000

        Mountpoint: /stream

        Password: hackme

    Нажмите Play в butt для старта эфира.

Шаг 3. Проброс туннеля в сеть

Запустите команду в терминале:
ssh -R 80:127.0.0.1:8000 nokey@localhost.run

 Команда проекта

    Артём Удмуртия

    Сергей Некто

    Иван Минутов (ИвМи)

    Ева Сырова

    Ироглефы бяо дзы
