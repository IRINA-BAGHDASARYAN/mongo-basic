Проверка переменных окружения

1. Убедись, что в файле: c:/Users/HP/Desktop/MVC4/.env
   есть строка:

MONGO_URI=YOUR_MONGODB_URI

и (опционально):
PORT=3000

2. dotenv.config() в mongo.server.js должен подхватить .env из корня проекта.

Если MONGO_URI = undefined — значит в .env нет переменной или она записана не в формате KEY=VALUE.
