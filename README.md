# Atlas Control — Landing Page

Лендінг-сторінка продуктової лінійки Atlas Control.

## Структура

```
atlas-landing/
├── index.html          # Головна сторінка (UA/EN)
├── images/
│   ├── atlas-case.png  # Фото алюмінієвого корпусу
│   └── atlas-pcb-3d.png # 3D рендер PCB Pro/Apex
└── README.md
```

## Деплой на GitHub Pages

1. Створіть репо `AltasFlight/atlas-landing` на GitHub
2. Запуште ці файли:
   ```bash
   git init
   git add .
   git commit -m "Initial landing page"
   git branch -M main
   git remote add origin git@github.com:AltasFlight/atlas-landing.git
   git push -u origin main
   ```
3. Перейдіть в Settings → Pages → Source: `main` branch, folder: `/ (root)`
4. Сайт буде доступний за адресою: `https://altasflight.github.io/atlas-landing/`

## Що змінити перед деплоєм

- **Email**: замініть `contact@atlascontrol.ua` на реальний email в секції контактів
- **Signal/WhatsApp**: додайте реальний номер або посилання
- **Посилання на docs**: зараз вказує на `https://altasflight.github.io/atlas-docs/`

## Двомовність

Перемикач UA/EN в навігації. Весь контент має атрибути `data-ua` та `data-en`.
