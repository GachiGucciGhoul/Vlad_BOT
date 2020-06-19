# Vlad_BOT &mdash; музыкальный бот для Discord, способный проигрывать аудиозаписи из VK.

## Что находится в репозитории

В данном репозитории находятся 4 папки &mdash; CPP_CLIENT, хранящая приложение клиента, CPP_SERVER, содержащая приложение сервера, папка JS_BOT с модулем программы, написанным на языке JavaScript и папка KISSVK_PARSER для работы проекта с сайтом [kissvk.com](https://kissvk.com/)

## Как запустить проект
Скачиваем папки CPP_CLIENT, CPP_SERVER, JS_BOT, KISSVK_PARSER и приступаем кработе.
Для начала подключим к проектам сервера и клиента библиотеку SFML. 
Скачиваем [архив](https://www.sfml-dev.org/files/SFML-2.5.1-windows-vc15-64-bit.zip) содержащий библиотеку и распаковываем его в удобное место.
После этого открываем интересующие нас проекты, заходим в свойтсва и меняем путь до папки с библиотекой в двух местах, изображенных на скриншотах ниже.
![Рисунок 1](https://raw.githubusercontent.com/GachiGucciGhoul/Vlad_BOT/master/screenshots/1.png)
_Рисунок 1. C/C++ -> общие_
![Рисунок 2](https://raw.githubusercontent.com/GachiGucciGhoul/Vlad_BOT/master/screenshots/2.png)
_Рисунок 2. Компоновщик -> общие_  
  Обратите внимание, что в первом случае путь указывается до папки include, а во втором до папки lid. Так же нужно убедиться, что при настройке свойств проектов выставлена конфигурация Debug на платформа x64 и собираться на таких же настройках.  
  Так же нам необходимо настроить node.js. В папку JS_BOT помещаем содержание архива, расположенного на [диске](https://yadi.sk/d/l788A7aLt_zvYQ). С сайта [nodejs.org](https://nodejs.org/en/) качаем и устанавливаем текущую версию. После этого в папке JS_BOT открываем “powershell”, прописываем “npm i” и ждем окончания установки (перед этим убедитесь, что в систему на вашем компьютере установлен git и python).   
  Финальным шагом является настройка самого бота под ваш сервер. Для начала пригласим его на сервер, перейдя по [ссылке](https://discord.com/oauth2/authorize?client_id=709356180119617656&scope=bot&permissions=3222032). Выбрать в какой голосовой канал на сервере, в который должен входить бот, и скопировать ID этого канала в четвертую строчку файла "config.json" ([Инструкция о том, как это сделать](https://support.discord.com/hc/ru/articles/206346498-Где-мне-найти-ID-пользователя-сервера-сообщения-)). Если для подключения к выбранному голосовому каналу требуется особая роль, то ее необходимо выдать боту.  
  После этих настроек проект будет готов к работе.  
    
Работу выполнил Корзин Василий ПИ-б-о-191(1).
