# Atlas Control — Landing Page

Сайт продуктової лінійки Atlas Control. Продакшн: **atlascontrol.pro**

## Структура

```
atlas-site/
├── index.html              # Головна сторінка (UA/EN)
├── CNAME                   # atlascontrol.pro
├── images/
│   ├── atlas-in-uav.png    # Фото контролера в БПЛА (hero секція)
│   ├── atlas-pcb-3d.png    # 3D рендер PCB Pro/Apex (about секція)
│   └── README.md
└── README.md
```

## Деплой

GitHub Pages з кастомним доменом `atlascontrol.pro`.

```bash
git add index.html
git commit -m "опис змін"
git push origin main
```

Сайт оновлюється автоматично за ~1-2 хвилини після пушу.

## Секції сторінки

| Секція | ID | Опис |
|--------|----|------|
| Hero | — | Головний заголовок, фото, кнопки CTA |
| Features | `#features` | 6 карток переваг |
| Products | `#products` | 4 моделі з цінами та бейджами |
| Comparison | `#comparison` | Таблиця порівняння характеристик |
| About | `#about` | Текст + факти + PCB фото |
| Contact | `#contact` | Signal/WhatsApp, Email, Docs |

## Продуктова лінійка

| Модель | Ціна | Статус |
|--------|------|--------|
| Atlas Control | $300 | В наявності |
| Atlas Control+ | $500 | В наявності |
| Atlas Control Pro | $800 | В наявності |
| Atlas Control Apex | $1200 | In Development |

## Двомовність

Перемикач UA/EN у навігації. Контент має атрибути `data-ua` та `data-en` на всіх текстових елементах. Логіка в `toggleLang()`.

## Мобільна підтримка

- Hamburger меню (≤768px)
- Responsive grid: 2 колонки → 1 колонка (≤1024px)
- Таблиця порівняння: горизонтальний скролл всередині контейнера
- `overflow-x: hidden` на body/html — запобігає горизонтальному скроллу сторінки
- `html { background: var(--olive-dark) }` — усуває кремову смугу на iOS Safari знизу

## Що може знадобитись оновити

- **Email** у секції контактів — зараз через Cloudflare email protection
- **Signal/WhatsApp** — наразі без реального посилання/номера
- **Ціни** — якщо зміняться
- **Бейдж "In Development"** на Apex — прибрати коли вийде в продаж
