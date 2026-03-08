# <div align="center">

# 📁 Apache AutoIndex file directory

**Красивый, современный интерфейс для стандартного файлового листинга Apache**

<!-- скриншоты -->
| Light Mode | Dark Mode |
|:---:|:---:|
| ![Light Theme](screenshots/light.png) | ![Dark Theme](screenshots/dark.png) |

</div>

---

## ✨ Возможности

- 🌗 **Тёмная / Светлая тема** — автоопределение по системным настройкам + ручное переключение
- 🔍 **Поиск файлов** — мгновенная фильтрация в реальном времени
- 🚀 **Без зависимостей** — чистый HTML + CSS + Vanilla JS, без фреймворков

## 📋 Требования

- **Apache HTTP Server** 2.4+
- Включённые модули:
  - `mod_autoindex`
  - `mod_dir`
  - `mod_mime`
- Разрешение использования `.htaccess` (`AllowOverride All`)

### Проверка модулей

```bash
# Проверить активные модули
apache2ctl -M | grep -E "autoindex|dir|mime"

# Включить модули (если не активны)
sudo a2enmod autoindex dir mime

# Перезапустить Apache
sudo systemctl restart apache2

<br>
# Мои заметки:
Если сервер апач уже настроен, то достаточно создать папку для общего доступа в соответствующей директории:
`/var/www/html/myServer/`

Чтобы подключиться нужно знать ip устройства:
`ip addr show`
`http://192.168.0.23/myServer`

у апача по умолчанию порт 80, интерфейсы 0.0.0.0

Можно настроить стили для Apache AutoIndex file directory
Для этого нужно включить в апач поддержку .htaccess
создать файл .htaccess
создать файлы со стилями
