# Сайт с чатом

Этот пример - с одной стороны учебный, с другой - в нём реализованые важнейшие вещи, которые обычно требуются при разработке сайтов:

- Конфигурация в файлах через nconf
- Обычные страницы, которые проходят через роутер
- Шаблонизация EJS, (ejs-locals: partials, helpers, layouts)
- JSON-сервис (та же страница по сути)
- Авторизация (Express, Connect, MongoDB)
- Закрытая страница (`/chat`, требует авторизации)
- Чат при помощи Sock.JS, интеграция с авторизацией (можно использовать Socket.IO или ws.js)
- Работа с базой данных (MongoDB, Mongoose)
- Асинхронные цепочки вызовов (Async.js)
- Логирование (winston + фабрика логгеров по модулю)
- Кластеризация (общая архитектура подходит + clusterMaster по желанию)

Архитектура пригодна для разработки и расширения.

# Использование

1. `git clone`
2. Под Mac/Linux: `npm start` (или `npm run dev` или `npm run cluster`)
2.1 Под Windows: `start.bat` (или `dev.bat`)
3. `open http://127.0.0.1:3000`

Войти в сайт можно будет через ссылку "Войти" справа.

# Примечания

- в репозитарии нет тестов, в этом примере они не рассматриваются.
- node_modules включены в репозитарий, это рекомендованная практика для приложений
(см. `https://npmjs.org/doc/faq.html`).