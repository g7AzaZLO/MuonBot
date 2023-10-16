# MuonBot
## Отслеживать Muon ноду теперь можно при помощи бота
Данный бот покажет статистику по всем нодам(актив/неактив), покажет информацию про вашу ноду. Присутствует функция утановки мониторинга состояния ноды, которое будет присылать оповещение, если нода упала
## Команды в боте
/start - Инициализация бота <br />
/check_node <ip_address> - Показать информацию о ноде, по заданному ip <br />
/status - Общая информация про ноды в сети<br />
/watchdog <ip_address> - Мониторинг ноды по заданному ip. Если нода упала, то бот пришлет сообщение<br />
/watchdog_stop - Остановить мониторинг ноды<br />
/about - Информация про команду и автора<br />
/help - Вывести все команды<br />
## Установка и настройка
1) Скачиваем бота

```
sudo git clone https://github.com/MaloyMeee/MuonBot.git

```
2) Переходим в папку
```
cd MuonBot
cd bot
```
3) Прописываем токен от нашего бота в конфиг(бота создаем в https://t.me/BotFather)
```
nano config.py
```
4 )Устанавливаем docker и docker-compose
```
sudo apt install docker.io 
sudo apt install docker-compose
```
5) Запускаем контейнер
```
sudo docker-compose up -d --build
```
