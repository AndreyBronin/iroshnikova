# Деплой сайта на GitHub Pages

Этот репозиторий настроен для автоматического деплоя Hugo сайта на GitHub Pages с помощью GitHub Actions.

## Настройка деплоя

### 1. Включить GitHub Pages

1. Перейдите в **Settings** → **Pages** в вашем GitHub репозитории
2. В разделе **Source** выберите **GitHub Actions**
3. Workflow будет запускаться автоматически при push в ветку `main`

### 2. Настройка пользовательского домена (опционально)

Если у вас есть собственный домен:

1. В **Settings** → **Pages** → **Custom domain** укажите ваш домен
2. Обновите `baseURL` в `config/_default/hugo.yaml`:
   ```yaml
   baseURL: 'https://yourdomain.com/'
   ```

### 3. Проверка деплоя

- Workflow запускается автоматически при каждом push в `main`
- Статус сборки можно посмотреть в разделе **Actions**
- Сайт будет доступен по адресу: `https://username.github.io/repository-name/`

## Локальная разработка

### Требования
- Hugo Extended v0.150.0+
- Go v1.21.5+
- Node.js v22+
- pnpm

### Команды разработки

```bash
# Установка зависимостей
pnpm install

# Локальный сервер разработки
npm run dev
# или
hugo server --disableFastRender

# Сборка для продакшена  
npm run build
# или
hugo --minify
```

### Обновление Hugo модулей

```bash
hugo mod get -u
hugo mod tidy
```

## Особенности конфигурации

- **SEO**: Настроены метатеги, структурированные данные, Open Graph
- **Производительность**: Минификация, оптимизация изображений, сжатие
- **Мультиязычность**: Поддержка русского и английского языков
- **Адаптивность**: Оптимизация для мобильных устройств

## Структура проекта

```
├── .github/workflows/       # GitHub Actions workflows
├── config/_default/         # Конфигурация Hugo
├── content/                 # Контент сайта
├── layouts/                 # Кастомные шаблоны
├── static/                  # Статические файлы
└── assets/                  # Ассеты для обработки
```

## Мониторинг и отладка

- **Логи сборки**: GitHub Actions → ваш workflow → Build job
- **Локальная отладка**: `hugo server --logLevel debug`
- **Проверка ссылок**: `hugo --printUnusedTemplates --printI18nWarnings`

## Поддержка

При возникновении проблем:

1. Проверьте логи в GitHub Actions
2. Убедитесь, что все зависимости установлены
3. Проверьте синтаксис YAML файлов
4. Локально протестируйте сборку командой `hugo --minify`
