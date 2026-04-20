# YouTube Research Marketplace

Маркетплейс с одним плагином — `youtube-research-agent`. Превращает Claude (Cowork или Claude Code) в профессионального ресерчера и ревьюера по YouTube.

## Установка в Cowork

1. Открой **Customize → Browse plugins → Plugins**.
2. Справа сверху переключи фильтр на **Personal**.
3. Рядом с **Local uploads** нажми `+` → **Add marketplace**.
4. Вставь `maxtreysi/youtube-research-marketplace` и нажми **Sync**.
5. После синхронизации плагин `youtube-research-agent` появится в списке — нажми **Install** на его карточке.
6. Активируй коннекторы: **Customize → Personal plugins → Youtube research agent → Connectors**, нажми **Install** на **TranscriptAPI** (обязательный) и, по желанию, на **Notion**.

Подробная инструкция для пользователей — см. [гайд](../guide-youtube-researcher-agent.md) или README плагина: [`plugins/youtube-research-agent/README.md`](plugins/youtube-research-agent/README.md).

## Установка в Claude Code

```
/plugin marketplace add maxtreysi/youtube-research-marketplace
/plugin install youtube-research-agent
```

## Что внутри

```
youtube-research-marketplace/
├── .claude-plugin/
│   └── marketplace.json
└── plugins/
    └── youtube-research-agent/
        ├── .claude-plugin/
        │   └── plugin.json
        ├── .mcp.json
        ├── skills/
        │   └── youtube-review/
        │       └── SKILL.md
        ├── PROJECT_INSTRUCTIONS.md
        └── README.md
```

## Лицензия

MIT.
