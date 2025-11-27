# discord-message-reader

## EN
> This bot collects and exports messages from Discord server channels it has been granted access to.  
> It is intended for moderation, archiving, auditing, or analytics.  
> The bot operates strictly within the permissions provided by server administrators and complies with Discord’s API policies.

## RU
> Этот бот собирает и экспортирует сообщения из каналов Discord-сервера, к которым ему предоставлен доступ.  
> Он предназначен для модерации, создания архивов, аудита или аналитики.  
> Бот работает только в рамках разрешений, выданных администраторами сервера, и соответствует правилам Discord API.

---

### 📌 Инструкция

#### Файлы
Бот использует внешние `.txt` файлы, которые должны лежать рядом с `.exe`:

- `DISCORD_TOKEN.txt` — токен бота  
- `USER_ID.txt` — ID пользователя  
- `IGNORED_CHANNELS.txt` — каналы, которые игнорируем (ID или имена через запятую)  
- `SCAN_CHANNELS.txt` — каналы, которые нужно сканировать (опционально, через запятую)  

#### Запуск
1. Скопируйте `message_reader.exe` и `.txt` файлы в одну папку.  
2. Запустите `message_reader.exe`

После завершения работы появится файл:
messages_<USER_ID>.txt
с собранными сообщениями.

#### Как работает
1. Бот подключается к серверам, где он есть
2. Сканирует текстовые каналы, кроме игнорируемых
3. Для каждого сообщения сохраняется: [канал] дата-время — текст сообщения

❗ Если указан SCAN_CHANNELS.txt, сканирует только эти каналы ❗

#### Требования
Бот добавлен на сервер с правами Read Message History
