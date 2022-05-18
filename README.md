
# 🏫 Личный кабинет студента
![Preview](https://user-images.githubusercontent.com/100470279/163875429-31827bb3-1e6c-4d75-8c9a-241df947d442.png)
![Preview](https://user-images.githubusercontent.com/100470279/163875341-bcd2d62d-a875-4ca1-bf04-3b8a0eb72c53.png)

# 📗 О проекте

Это приложение было написано командой из 2 человек и представляет собой личный кабинет пользователя с подключенной базой данных firebase и React TypeScript с использованием MUI.

# 📙 Запуск приложения
Для работы локального сервера сперва нужно установить платформу [NodeJS](https://nodejs.org/en/download/).

Для конфигурации проекта используется файл `package.json`. Который содержит вспомогательную информацию о имени проекта, его версии, описания и т.д.
В разделе `scripts` используются скрипты, которые можно запускать из окружения.
* start - запускает сервер с помощью `nodemon`.
* test - должен запускать тесты, но так как тестов нету, то реализована такая загрушка (которую можно убрать)
В разделе `dependencies` прописаны зависимости, которые используются в проекте
* [dotenv](https://www.npmjs.com/package/dotenv) - позволяет использовать переменные окружения для настроек (в файле `.env` описаны настройки). [исходный_код](https://github.com/motdotla/dotenv)
* [express](https://www.npmjs.com/package/express) - основной framework используемый в приложении. Тоесть его база, которая позволяет удобно обрабатывать HTTP запросы. Можно сказать, что приложение реализовано с помощью [express](https://expressjs.com/ru/) framework'a. [официальный_сайт](https://expressjs.com/ru/), [исходный_код](https://github.com/expressjs/express)
* [lowdb](https://www.npmjs.com/package/lowdb) - простенькая база данных для сохранения данных. [исходный_код](https://github.com/typicode/lowdb)
* [morgan](https://www.npmjs.com/package/morgan) - средство регистрации HTTP запросов. В данном приложении просто печатает все запросы в консоль. [исходный_код](https://github.com/expressjs/morgan)
* [multer](https://www.npmjs.com/package/multer) - это middleware для фреймворка express для обработки multipart/form-data. [исходный_код](https://github.com/expressjs/multer)
* [nodemon](https://www.npmjs.com/package/nodemon) - пакет, который реализует перезагрузку сервера при изменении его исходного кода. Удобен для разработки, что бы каждый раз не перезапускать сервер. [исходный_код](https://github.com/remy/nodemon)
* [uniqid](https://www.npmjs.com/package/uniqid) - пакет, позволяющий генерировать уникальные идентификаторы. Очень важен при создании `id` для сущностей *пользователя* и *счёта*. [исходный_код](https://github.com/adamhalasz/uniqid)

Для установки пакетов в терменале используется команда `npm i`
 
Для запуска сервера используется команда `npm run start`. В этом случае запускается сервер (с использованием `nodemon`) запуская файл `index.js`
