# VPN Telegram Bot

## Описание
Автоматизированная система управления доступом к VPN через Telegram бота. Позволяет пользователям получать WireGuard конфигурации напрямую через бот без необходимости ручной настройки.

## Технологический стек
- **Backend**: Node.js
- **База данных**: PostgreSQL
- **VPN**: WireGuard API
- **Мессенджер**: Telegram Bot API
- **Процесс-менеджер**: PM2

## Основные возможности
- ✅ Автоматическая выдача VPN ключей через Telegram
- ✅ Управление пользователями и их конфигурациями
- ✅ Мониторинг статуса подключений
- ✅ Хранение данных в PostgreSQL
- ✅ Интеграция с WireGuard сервером
- ✅ Защищенное хранение ключей

## Архитектура
```
[Telegram Bot] <-> [Node.js Backend] <-> [PostgreSQL DB]
                          |
                          v
                  [WireGuard Server]
```

## Установка

### Требования
- Node.js 16+
- PostgreSQL 12+
- WireGuard установлен на сервере
- Telegram Bot Token

### Быстрый старт
```bash
git clone https://github.com/berejnovsky/vpn-telegram-bot.git
cd vpn-telegram-bot
npm install
cp .env.example .env
npm start
```

## Использование
1. Запустите бота в Telegram
2. Отправьте `/start`
3. Получите VPN конфигурацию
4. Импортируйте в WireGuard клиент

## Лицензия
MIT
