---
# SEO-оптимизированный title для главной страницы
title: 'Маркетолог B2B | Консультант по промышленному маркетингу | Алена Ирошникова'
description: 'Профессиональный маркетолог B2B с 18+ летним опытом. Эксперт по промышленному маркетингу, стратегическому планированию. Консультации для технических компаний. Опыт работы с KNIPEX, Jungheinrich, Siemens.'
keywords: 'маркетолог B2B, промышленный маркетинг, консультант по маркетингу, стратегический маркетинг, маркетинг технических продуктов, B2B консультант, маркетинговая стратегия'
date: 2022-10-24
type: landing

design:
  # Default section spacing - optimized for mobile
  spacing: '4rem'
  # Mobile-first responsive spacing
  spacing_mobile: '2rem'

sections:
  - block: resume-biography-3
    id: hero
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: |
        **Head of Marketing | Эксперт по B2B-маркетингу сложных технических продуктов.**

        18+ лет в международных индустриальных гигантах KNIPEX, Jungheinrich, Siemens. Строю системный маркетинг, вывожу бренды в лидеры и внедряю инновации.
      # Show call-to-action buttons under your biography
      buttons:
        - text: Связаться со мной
          url: 'mailto:alena.iroshnikova@gmail.com?subject=Связаться по проекту'
        - text: Скачать Media Kit
          url: uploads/media-kit.zip
      headings:
        about: 'О себе'
        education: 'Образование'
        interests: 'Экспертиза'
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient resume-biography hero-section
      # Avatar customization - responsive sizing
      avatar:
        size: large # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      # Mobile optimization
      spacing:
        padding: ['3.5rem', '2rem', '2.5rem', '2rem'] # top, right, bottom, left
        margin: [0, 0, '2rem', 0]
  - block: markdown
    id: summary
    content:
      title: 'Стратег и играющий тренер'
      subtitle: 'Управляю маркетинговыми командами inhouse и outsource с 2012 года'
      text: |-
        «Стратег и играющий тренер. Управляю маркетинговыми командами inhouse и outsource с 2012 года».

        «Специализируюсь на омниканальном маркетинге, ABM (Account Based Marketing) и цифровой трансформации в B2B».

        **Ключевые цифры**

        | 20+ лет в маркетинге | 13+ лет на управленческих позициях | 3 международных бренда | C2 уровень английского |
        | --- | --- | --- | --- |
        | Полный цикл — от стратегии до реализации | Руководство командами и агентствами | KNIPEX, Jungheinrich, Siemens | Готова к переговорам и выступлениям |
    design:
      columns: '1'
      css_class: 'markdown-block summary-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: markdown
    id: cases
    content:
      title: 'Кейсы и измеримые результаты'
      subtitle: 'Было → Сделала → Стало'
      text: |-
        **Запуск собственной торговой марки (KNIPEX)**  
        Было: нужен новый бренд с нуля.  
        Сделала: нейминг, брендбук, ценообразование, обучение дилеров, запуск e-com.  
        Стало: топ-10 в категории на маркетплейсах, окупаемость за 8 месяцев, +15% выручки.  
        [Подробнее →](/projects/pandas/)

        **Трансформация бренда Jungheinrich**  
        Было: «неизвестный немецкий производитель».  
        Сделала: новая стратегия позиционирования, единая коммуникация, отраслевые мероприятия, дилерская программа.  
        Стало: узнаваемость 67%, топ-3 рынка, +40% продаж за 2 года.  
        [Подробнее →](/projects/pytorch/)

        **ABM для ключевых дилеров**  
        Было: разрозненная работа с крупными аккаунтами.  
        Сделала: сегментация топ-50, персональные планы, кастомные материалы, KPI-трекинг.  
        Стало: +25% к среднему чеку, +35% repeat-sales, retention 89%.  
        [Подробнее →](/projects/scikit/)
    design:
      columns: '1'
      css_class: 'markdown-block cases-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: markdown
    id: timeline
    content:
      title: 'Карьерный путь'
      subtitle: 'Бренды, роли и главные результаты'
      text: |-
        **KNIPEX (2020 – н.в.) — Head of Marketing.** Запуск e-com стратегии, рост узнаваемости бренда, построение digital-воронки.

        **Jungheinrich (2009 – 2019) — Head of Marketing.** Разработка B2B-стратегии, вывод на рынок новых продуктов, масштабирование дилерской сети.

        **Siemens (2004 – 2009) — от ассистента до PR/Marketing specialist.** Старт карьеры в глобальной корпорации, фокус на коммуникациях и PR.

        [Скачать CV в PDF →](uploads/resume.pdf)
    design:
      columns: '1'
      css_class: 'markdown-block timeline-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: markdown
    id: media-kit
    content:
      title: 'Спикер и эксперт для СМИ'
      subtitle: 'Материалы для конференций, подкастов и журналистов'
      text: |-
        **Темы выступлений**

        - Маркетинг сложных технических продуктов  
        - ИИ в маркетинге: практические кейсы  
        - Account Based Marketing (ABM) в России  
        - Трайбл-маркетинг и community management  
        - Построение дилерских сетей и trade marketing  

        **Видео-превью**  
        Запросите шоурил (1–2 минуты) с яркими фрагментами выступлений: [получить ссылку](mailto:alena.iroshnikova@gmail.com?subject=Запрос%20шоурила).

        **Фотогалерея «Алёна на сцене»**  
        Фото с ключевых конференций и панельных дискуссий — доступно в пресс-папке.

        **Скачать пресс-папку**  
        - Профессиональные фото (вертикальное, горизонтальное, ч/б)  
        - Краткая и полная биография  
        - Темы выступлений с тезисами  
        - Логотипы компаний для анонсов  

        [Скачать пресс-папку →](uploads/media-kit.zip)

        **Календарь выступлений**

        - Предстоящие: откройте даты для конференций и корпоративных сессий — пишите, чтобы забронировать слот.  
        - Архив: прошлые выступления, записи и презентации доступны по запросу.
    design:
      columns: '1'
      css_class: 'markdown-block media-kit-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: markdown
    id: events
    content:
      title: 'Где меня можно услышать'
      subtitle: 'Календарь выступлений и записей'
      text: |-
        **Предстоящие**  
        - (добавьте дату/город) — тема из списка: ИИ в маркетинге / ABM / дилерские сети. [Забронировать слот](mailto:alena.iroshnikova@gmail.com?subject=Бронирование%20выступления)

        **Прошедшие**  
        - (пример) Суровый Питерский Маркетинг — панель о B2B, запись доступна по запросу.  
        - (пример) Индустриальный форум — кейс внедрения ABM, материалы по запросу.

        Уточнить расписание и получить записи можно по письму или в Telegram.
    design:
      columns: '1'
      css_class: 'markdown-block events-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: markdown
    id: services
    content:
      title: 'Услуги и консалтинг'
      subtitle: 'Четко разграничиваю форматы работы'
      text: |-
        **1. Карьерные консультации**  
        Менторинг для маркетологов, подготовка к росту до Head of Marketing, работа над личным брендом.

        **2. Стратегические сессии для B2B**  
        Аудит текущего маркетинга, запуск бренда, настройка воронки продаж, ABM и омниканальные кампании.

        **3. Корпоративное обучение**  
        Лекции и воркшопы для отделов маркетинга и продаж: стратегия, дилерские сети, trade marketing, внедрение ИИ.

        [Записаться на консультацию](mailto:alena.iroshnikova@gmail.com?subject=Запрос%20консультации) · [Пригласить спикером](mailto:alena.iroshnikova@gmail.com?subject=Приглашение%20спикером)
    design:
      columns: '1'
      css_class: 'markdown-block services-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: markdown
    id: lead-magnet
    content:
      title: 'Лид-магнит для B2B-команд'
      subtitle: 'Скачайте чек-лист и оцените готовность к росту'
      text: |-
        **Чек-лист:** «Готов ли ваш B2B-бренд к выходу в e-com»  
        - 10 шагов подготовки: продукт, контент, дистрибуция, SLA с продажами, аналитика.  
        - Типичные ошибки при участии в промышленных выставках и как их избегать.  
        - Фреймворк быстрой оценки готовности команды и каналов.

        [Получить чек-лист →](uploads/lead-magnet.pdf)
    design:
      columns: '1'
      css_class: 'markdown-block lead-magnet-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: collection
    id: blog
    content:
      title: Блог / Статьи
      subtitle: 'Свежие материалы и кейсы о B2B-маркетинге'
      text: 'Последние публикации: внедрение ИИ в маркетинг, тренды 2025, выставки и индустриальные коммуникации.'
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      css_class: 'blog-section'
      columns: 3
      columns_mobile: 1
      columns_tablet: 2
      # Mobile-optimized spacing
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
        gap: '1.5rem'
  - block: markdown
    id: recognition
    content:
      title: 'Рекомендации и награды'
      subtitle: ''
      text: |-
        **Battle of Marketers, ноябрь 2023 — победитель.** Фото диплома и трофея: ![](/uploads/battle-of-marketers.png)

        Дополнительно: отраслевые награды за запуск СТМ, digital-прорывы и рост брендов в промышленном секторе.
    design:
      columns: '1'
      css_class: 'markdown-block recognition-section'
      spacing:
        padding: ['2rem', '1rem', '2rem', '1rem']
  - block: markdown
    id: contacts
    content:
      title: 'Контакты'
      subtitle: 'Оперативно отвечаю на запросы по спикерству, консалтингу и совместным проектам'
      text: |-
        **Телефон:** [+7 (926) 468 12 37](tel:+79264681237)  
        **Email:** [alena.iroshnikova@gmail.com](mailto:alena.iroshnikova@gmail.com)  
        **Telegram:** [@Alena_Sea_Inside](https://t.me/Alena_Sea_Inside)

        **Соцсети:** [LinkedIn](https://linkedin.com/in/alena-iroshnikova) · [TenChat](https://tenchat.ru/) · [VC.ru](https://vc.ru/)

        **Заявки:** [Пригласить спикером](mailto:alena.iroshnikova@gmail.com?subject=Приглашение%20спикером) · [Записаться на консультацию](mailto:alena.iroshnikova@gmail.com?subject=Запрос%20консультации)
    design:
      columns: '1'
      css_class: 'markdown-block contacts-section'
      spacing:
        padding: ['2.5rem', '1rem', '3rem', '1rem']
---
