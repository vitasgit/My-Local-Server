# <div align="center">

# 📁 Apache AutoIndex file directory

**Красивый, современный интерфейс для стандартного файлового листинга Apache**

![Apache](https://img.shields.io/badge/Apache-2.4+-D22128?style=for-the-badge&logo=apache&logoColor=white)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

<br/>

<!-- Замените на реальные скриншоты -->
| Light Mode | Dark Mode |
|:---:|:---:|
| ![Light Theme](screenshots/light.png) | ![Dark Theme](screenshots/dark.png) |

</div>

---

## ✨ Возможности

- 🌗 **Тёмная / Светлая тема** — автоопределение по системным настройкам + ручное переключение
- 🔍 **Поиск файлов** — мгновенная фильтрация в реальном времени
- 🍞 **Breadcrumb-навигация** — удобное перемещение по директориям
- 🎨 **Кастомные SVG-иконки** — разные иконки для разных типов файлов
- 📱 **Адаптивный дизайн** — корректное отображение на мобильных устройствах
- ⚡ **Анимации** — плавное появление элементов
- 🖨 **Print-стили** — корректная печать страницы
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
