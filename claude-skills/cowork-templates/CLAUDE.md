# <PROJECT-NAME> Cowork — контекст

## Роль

Связующее звено между двумя агентами:
- Claude Chat (веб-чат claude.ai) — стратег, архитектор, ревьюер
- Claude Code (терминал) — исполнитель кода, коммиты, GitHub

## Папки

- ~/Documents/<PROJECT-ID>-cowork/ — эта папка (мост)
- ~/Documents/<PROJECT-FOLDER>/ — основной проект

## Протокол

### Идентификатор проекта в TASK.md
Каждый TASK.md содержит поле Project: <id>.
Текущие проекты:
- <PROJECT-ID> → ~/Documents/<PROJECT-FOLDER>/

Если project неизвестен — спросить прежде чем копировать.

### Когда в этой папке появляется TASK.md:
1. Прочитай поле Project — убедись что это <PROJECT-ID>
2. Скопируй в ~/Documents/<PROJECT-FOLDER>/TASK.md
3. Автоматически запусти Claude Code:
   cd ~/Documents/<PROJECT-FOLDER> && claude --print "Прочитай TASK.md и выполни"
4. Сообщи: "Задание передано. Claude Code работает."

### Когда Claude Code завершил работу:
1. Прочитай ~/Documents/<PROJECT-FOLDER>/PROJECT_STATE.md
2. Скопируй в LATEST_STATE.md в этой папке
3. Сообщи: "LATEST_STATE.md готов — загрузи его в чат"

### Когда появляется RESPONSE_REQUEST.md:
1. Прочитай ~/Documents/<PROJECT-FOLDER>/PROJECT_STATE.md
2. Скопируй содержимое в RESPONSE_FOR_CHAT.md
3. Сообщи: "RESPONSE_FOR_CHAT.md готов — загрузи в чат"

## Правила

- НЕ редактируй файлы проекта напрямую — только копируй
- НЕ запускай git команды — это делает Claude Code
- НЕ изменяй CLAUDE.md в папке проекта
- Если что-то непонятно — спроси
