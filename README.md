# discord-message-reader

## EN
> This bot collects and exports user messages from Discord server channels to which it has been granted access.
> It is intended for moderation, archiving, auditing, or analytics purposes.
> The bot operates strictly within the permissions granted by server administrators and complies with Discord API rules.

 ---

 ### 📌 Instructions

#### Files
The bot uses external .txt files, which must be located in the same directory as the .exe:

- `DISCORD_TOKEN.txt` — The bot's token
- `USER_ID.txt` — The user's ID
- `IGNORED_CHANNELS.txt` — Channels to ignore (ID or names, separated by commas)
- `SCAN_CHANNELS.txt` — Channels to scan (optional, separated by commas)

#### Running the Bot
1. Copy message_reader.exe and the .txt files into one folder.
2. Run message_reader.exe

Upon completion, the following file will appear:
messages_<USER_ID>.txt
with the collected messages.

#### How It Works
1. The bot connects to the servers where it is present.
2. It scans the text channels, excluding the ignored ones.
3. For each message, it saves: [channel] date-time — message text

❗ If SCAN_CHANNELS.txt is specified, only these channels are scanned ❗

#### Requirements
The bot must be added to the server with "Read Message History" permissions.

## RU
> Этот бот собирает и экспортирует сообщения пользователей из каналов Discord-сервера, к которым ему предоставлен доступ.  
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
Бот добавлен на сервер с правами "Read Message History"
