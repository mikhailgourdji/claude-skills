# claude-skills

Персональные скиллы, память и шаблоны для работы с Claude.

## Структура

```
claude-skills/
├── README.md                          — этот файл
├── MEMORY_BACKUP.md                   — резервная копия памяти claude.ai
├── REVISION_LOG.md                    — история изменений
│
├── skills/
│   └── new-project-setup-SKILL.md    — старт нового проекта Chat+Code+Cowork
│
└── cowork-templates/
    └── CLAUDE.md                      — шаблон CLAUDE.md для любого проекта
```

## Как использовать

### Переезд на новый компьютер

1. Клонировать репо: `git clone https://github.com/mikhailgourdji/claude-skills`
2. Открыть `MEMORY_BACKUP.md` и восстановить записи в памяти claude.ai вручную
3. Для каждого нового проекта скопировать `cowork-templates/CLAUDE.md` в папку `<project>-cowork/`

### Новый проект

1. Создать папку `~/Documents/<project-id>-cowork/`
2. Скопировать `cowork-templates/CLAUDE.md` туда
3. Отредактировать PROJECT-ID и пути в файле
4. Подключить в Claude Desktop → Cowork

### Поделиться с коллегой

Дать ссылку на репо. Скиллы универсальные — работают у любого пользователя Claude.

## Ревизия

Раз в месяц открывать `REVISION_LOG.md` и обновлять что устарело.
