# @imperialglaz_bot
# 🎓 Telegram Bot для управления контактами студентов

📲 Бот для регистрации и управления контактами студентов, распределяя их по учебным группам.  

## 🚀 Возможности

### ✅ **Регистрация студентов** с вводом:
- **👤 Имени и фамилии**:  
  Бот запрашивает у пользователя его имя и фамилию, которые сохраняются в базе данных. Это позволяет идентифицировать студента и отображать его данные в профиле.

- **📱 Номера телефона**:  
  Пользователь вводит свой номер телефона, который также сохраняется в базе данных. Это может быть полезно для связи с студентом вне Telegram.

- **💬 Telegram-ника**:  
  Бот автоматически получает username пользователя Telegram, если он есть. Если username отсутствует, бот может запросить альтернативный способ идентификации.

- **🔗 Ссылки на VK**:  
  Пользователь может ввести ссылку на свой профиль ВКонтакте. Это может быть полезно для дополнительной информации о студенте.

- **📚 Учебной группы**:  
  Пользователь выбирает или вводит название учебной группы, к которой он относится. Группы могут быть добавлены администратором с помощью команды `/add_group`.

### 🔍 **Просмотр профиля** `/profile`:
- Команда `/profile` позволяет студенту просмотреть свои данные, которые он ввел при регистрации. Бот отображает имя, фамилию, номер телефона, Telegram-ник, ссылку на VK и учебную группу.

### ❌ **Удаление профиля** `/delete`:
- Команда `/delete` позволяет студенту удалить свой профиль из базы данных. После удаления все данные пользователя стираются, и он может зарегистрироваться заново.

### 🔑 **Админ-команды:**
- **🆕 Добавление групп → `/add_group {название}`**:  
  Администратор может добавлять новые учебные группы с помощью команды `/add_group`. Например, `/add_group Группа_101`. Это позволяет гибко управлять списком групп.

- **📚 Список групп → `/groups`**:  
  Команда `/groups` отображает список всех доступных учебных групп. Это полезно для администратора и студентов, чтобы узнать, какие группы уже существуют.

- **👥 Список студентов в группе → `/group_info {название}`**:  
  Команда `/group_info` позволяет администратору просмотреть список всех студентов, зарегистрированных в конкретной группе. Например, `/group_info Группа_101` покажет всех студентов, относящихся к этой группе.

---

## 🛠 Установка и запуск

### 1️⃣ **Клонируем репозиторий**
```sh
git clone https://github.com/your_username/your_repository.git
cd your_repository
```

### 2️⃣ **Устанавливаем зависимости**
```sh
pip install aiogram sqlite3
```
- **aiogram**: Фреймворк для создания Telegram-ботов на Python.
- **sqlite3**: Встроенная база данных для хранения данных студентов и групп.

### 3️⃣ **Настраиваем бота**
- **Замените `YOUR_BOT_API_TOKEN` в `bot.py` на ваш токен бота**:  
  Токен можно получить у [BotFather](https://core.telegram.org/bots#botfather) в Telegram.
  
- **Укажите `YOUR_ADMIN_ID` (ID администратора)**:  
  Это ID пользователя Telegram, который будет иметь доступ к админ-командам. Узнать свой ID можно с помощью бота, например, [userinfobot](https://t.me/userinfobot).

### 4️⃣ **Запускаем бота**
```sh
python bot.py
```
После запуска бот начнет работать и будет готов к взаимодействию с пользователями.

---

## 🔧 Используемые технологии

### � **Aiogram**:
- Aiogram – это современный фреймворк для создания Telegram-ботов на Python. Он предоставляет удобный интерфейс для работы с Telegram API, поддерживает асинхронные запросы и позволяет легко создавать сложные сценарии взаимодействия с пользователями.

### 🗄 **SQLite**:
- SQLite – это встроенная база данных, которая не требует отдельного сервера. Она идеально подходит для небольших проектов, таких как этот бот, где нужно хранить данные о студентах и группах. SQLite обеспечивает быстрый доступ к данным и простоту в использовании.

### 🐍 **Python 3.9+**:
- Python – основной язык разработки этого проекта. Выбор Python обусловлен его простотой, читаемостью и большим количеством библиотек, которые упрощают разработку. Версия 3.9+ обеспечивает поддержку современных функций языка.

---

## 📜 Лицензия

Этот проект распространяется под лицензией MIT.  
Если у вас есть предложения или улучшения, создавайте Issues или Pull Requests!  

💡 *Разработано для удобного управления контактами студентов!* 🚀
