# Универсальные Принципы Структуры Документации 3.0

## Современная архитектура документации для любых проектов

> **Основано на анализе лучших практик индустрии и исследованиях пользовательского опыта** > **Статус**: ✅ **Production-Ready** | **Версия**: 3.0.0 | **Обновлено**: 2025-01-15

## 🎯 Современная Философия Структуры

### 📋 Принципы Организации Контента

**Универсальная Архитектура Документации:**

```yaml
архитектура_документации:
  пользователе_центричная_организация:
    - user_journey_first: "Структура следует путям пользователей, не техническим границам"
    - task_oriented_hierarchy: "Группировка по задачам, которые пользователи хотят выполнить"
    - progressive_disclosure: "Информация раскрывается по мере углубления пользователя"
    - multi_persona_navigation: "Различные точки входа для разных типов пользователей"

  масштабируемая_архитектура:
    - modular_organization: "Модульные компоненты, которые могут расти независимо"
    - consistent_patterns: "Повторяющиеся паттерны во всей документации"
    - flexible_taxonomy: "Таксономия, которая адаптируется к росту продукта"
    - automated_organization: "Автоматизированное поддержание структурной целостности"

  интеллектуальная_навигация:
    - contextual_wayfinding: "Умная навигация на основе текущего местоположения пользователя"
    - related_content: "AI-рекомендации связанного контента"
    - search_first_design: "Архитектура оптимизированная для поисковых запросов"
    - cross_reference_intelligence: "Автоматические перекрестные ссылки и связи"
```

## 🏗️ Универсальная Структура Документации

### 📁 Основная Организация

```
README.md
LICENSE.md
CHANGELOG.md
CONTRIBUTING.md
GUIDE.md
docs/
├── 🏠 index.md                      # Главная страница документации (ОБЯЗАТЕЛЬНО для Docusaurus)
├── 📋 api/                         # API документация и техническая справка
│   ├── 📄 _category_.yml             # Метаданные категории (ОБЯЗАТЕЛЬНО)
│   ├── 📄 index.md                   # Обзор секции (ОБЯЗАТЕЛЬНО)
│   ├── 📄 authentication.md           # Методы аутентификации и авторизации
│   ├── 📂 endpoints/                  # Документация всех эндпоинтов
│   |   ├── 📄 _category_.yml           # Метаданные категории
│   │   ├── 📄 users.md                # Пользовательские эндпоинты
│   │   ├── 📄 data.md                 # Эндпоинты для работы с данными
│   │   └── 📄 admin.md                # Административные эндпоинты
│   ├── 📂 schemas/                    # Схемы данных и модели
│   ├── 📂 examples/                   # Примеры запросов и ответов
│   ├── 📄 webhooks.md                 # Документация вебхуков
│   ├── 📄 rate-limiting.md            # Ограничения по скорости запросов
│   └── 📄 changelog.md                # История изменений API
├── 🏛️ architecture/                # Системные и архитектурные документы
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 system-overview.md          # Общая архитектура системы
│   ├── 📄 component-design.md         # Дизайн отдельных компонентов
│   ├── 📄 data-flow.md                # Потоки данных
│   ├── 📄 security-model.md           # Модель безопасности
│   ├── 📄 scalability.md              # Планы масштабирования
│   ├── 📂 decision-records/           # Архитектурные решения (ADR)
│   └── 📂 diagrams/                   # Архитектурные диаграммы
├── 📦 archive/                     # Архив устаревших, но необходимых документов
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                # Обзор секции
│   ├── 📂 deprecated/                 # Устаревшие функции и их миграция
│   ├── 📂 legacy-docs/                # Документация предыдущих версий
│   ├── 📂 migration-guides/           # Руководства по миграции
│   ├── 📂 old-api-versions/           # Документация старых версий API
│   └── 📄 historical-decisions        # Исторические решения и их контекст
├── ⚙️ configuration/               # Руководства по конфигурации и настройке
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                # Обзор секции
│   ├── 📄 basic-setup.md              # Базовая настройка
│   ├── 📄 advanced-config.md          # Продвинутая конфигурация
│   ├── 📄 environment-vars.md         # Переменные окружения
│   ├── 📄 security-config.md          # Настройки безопасности
│   ├── 📄 performance-tuning.m        # Настройка производительности
│   ├── 📂 examples/                   # Примеры конфигураций
│   └── 📂 templates/                  # Шаблоны конфигурационных файлов
├── 📝 contributing/                # Руководства для контрибьюторов
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 getting-started.md          # Первые шаги для контрибьюторов
│   ├── 📄 code-of-conduct.md          # Кодекс поведения
│   ├── 📄 development-setup.md        # Настройка среды разработки
│   ├── 📄 pull-request-guide.m        # Руководство по PR
│   ├── 📂 issue-templates/            # Шаблоны для создания задач
│   ├── 📂 style-guides/               # Руководства по стилю кода
│   └── review-process.md           # Процесс ревью и утверждения
├── 🚢 deployment/                  # Развертывание и операции
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📂 docker/                     # Контейнеризация и Docker
│   ├── 📂 kubernetes/                 # Развертывание в K8s
│   ├── 📂 cloud-providers/            # Развертывание в облаке
│   |   ├── 📄 _category_.yml           # Метаданные категории
│   │   ├── 📄 aws.md                  # Amazon Web Services
│   │   ├── 📄 gcp.md                  # Google Cloud Platform
│   │   └── 📄 azure.md                # Microsoft Azure
│   ├── 📄 on-premises.md              # Развертывание на собственных серверах
│   ├── 📄 security.md                 # Безопасность при развертывании
│   └── 📄 monitoring.md               # Мониторинг и логирование
├── 📋 development/                 # Руководства для разработчиков
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 CURRENT_STATUS.md          # Текущий статус разработки (обновляется ежедневно)
│   ├── 📄 ROADMAP.md                 # План развития проекта
│   ├── 📄 DEVELOPMENT_PLAN.md        # Мастер-план разработки
│   ├── 📂 setup/                      # Настройка среды разработки
│   │   ├── 📄 _category_.yml
│   │   ├── 📄 index.md
│   │   ├── 📄 prerequisites.md
│   │   ├── 📄 environment-setup.md
│   │   └── 📄 ide-setup.md
│   ├── 📂 workflows/                  # Процессы разработки
│   │   ├── 📄 _category_.yml
│   │   ├── 📄 index.md
│   │   ├── 📄 git-workflow.md
│   │   ├── 📄 code-review.md
│   │   └── 📄 ci-cd.md
│   ├── 📂 tools/                      # Инструменты разработки
│   │   ├── 📄 _category_.yml
│   │   ├── 📄 index.md
│   │   ├── 📄 makefile.md
│   │   └── 📄 docker-tools.md
│   ├── 📂 environments/               # Среды разработки, тестирования, продакшн
│   │   ├── 📄 _category_.yml
│   │   ├── 📄 index.md
│   │   ├── 📄 local.md
│   │   ├── 📄 staging.md
│   │   └── 📄 production.md
│   ├── 📄 coding-standards.md         # Стандарты кодирования и стиль
│   ├── 📄 testing-guide.md            # Руководство по тестированию
│   ├── 📄 debugging.md                # Отладка и диагностика
│   ├── 📄 local-development.md        # Локальная разработка
│   ├── 📄 setup.md                    # Быстрая настройка
│   ├── 📄 tools.md                    # Обзор инструментов
│   └── 📄 workflow.md                 # Рабочий процесс
├── 🧪 examples/                    # Работающие примеры и демо-проекты
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции (НУЖЕН СРОЧНО)
│   ├── 📂 basic/                      # Базовые примеры для начинающих
│   ├── 📂 advanced/                   # Продвинутые сценарии использования
│   ├── 📂 integrations/               # Примеры интеграций
│   ├── 📂 use-cases/                  # Реальные случаи использования
│   ├── 📂 code-samples/               # Образцы кода
│   ├── 📂 configurations/             # Примеры конфигураций
│   └── 📂 demos/                      # Демонстрационные проекты
├── 🚀 getting-started/             # Быстрый старт для всех пользователей
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 01-quickstart.md          # 5-минутный путь к первому успеху
│   ├── 📄 02-installation.md        # Детальная установка всех опций
│   ├── 📄 03-first-steps.md         # Основные концепции + первая задача
│   ├── 📄 04-configuration.md       # Основная конфигурация
│   ├── 📄 05-verification.md        # Как проверить что все работает
│   └── 📄 06-next-steps.md          # Куда идти дальше
├── 🔧 how-to/                      # Решения конкретных проблем
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 cors-setup.md             # Настройка CORS (НУЖЕН)
│   ├── 📄 docker-vs-local.md        # Docker против локального запуска (НУЖЕН)
│   ├── 📄 mock-mode-setup.md        # Настройка режима имитации (НУЖЕН)
│   ├── 📄 service-management.md     # Управление сервисами (НУЖЕН)
│   ├── 📂 authentication/             # Задачи аутентификации
│   │   ├── 📄 jwt-setup.md          # Настройка JWT токенов (НУЖЕН)
│   │   └── 📄 api-keys.md           # Управление API ключами (НУЖЕН)
│   ├── 📂 data-management/            # Управление данными
│   │   ├── 📄 data-extraction.md    # Извлечение данных (НУЖЕН)
│   │   └── 📄 form-handling.md      # Работа с формами (НУЖЕН)
│   ├── 📂 integrations/               # Задачи интеграций
│   │   ├── 📄 webhook-setup.md      # Настройка веб-хуков (НУЖЕН)
│   │   └── 📄 external-apis.md      # Интеграция с внешними API (НУЖЕН)
│   ├── 📂 customization/              # Кастомизация и настройка
│   ├── 📂 monitoring/                 # Мониторинг и алерты
│   │   └── 📄 health-checks.md      # Проверки состояния системы (НУЖЕН)
│   ├── 📂 backup-recovery/            # Резервные копии и восстановление
│   └── 📂 performance/                # Оптимизация производительности
├── 🔗 integration/                 # Интеграции и подключения к внешним системам
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 getting-started.md          # Быстрый старт интеграций
│   ├── 📂 authentication/             # Настройка аутентификации
│   ├── 📂 third-party/                # Интеграции с внешними сервисами
│   |   ├── 📄 _category_.yml           # Метаданные категории
│   │   ├── 📄 databases.md            # Подключение баз данных
│   │   ├── 📄 messaging.md            # Системы сообщений
│   │   └── 📄 analytics.md            # Аналитические платформы
│   ├── 📂 webhooks/                   # Настройка и использование вебхуков
│   ├── 📂 sdk/                        # Software Development Kits
│   └── 📂 plugins/                    # Система плагинов и расширений
├── 🛠️ operations/                  # Операционные руководства и процедуры
├── 📋 reference/                   # Техническая справочная информация
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📂 api/                        # Полная API документация
│   |   ├── 📄 _category_.yml           # Метаданные категории
│   │   ├── 📄 authentication.md
│   │   ├── 📂 endpoints/
│   │   ├── 📂 schemas/
│   │   └── 📂 examples/
│   ├── 📂 cli/                        # Справка командной строки
│   ├── 📂 configuration/              # Все опции конфигурации
│   ├── 📂 glossary.md                 # Определения терминов
│   ├── 📂 specifications/             # Технические спецификации
│   └── compatibility.md            # Таблицы совместимости
├── 📊 reports/                     # Отчеты и аналитические материалы
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📂 performance/                # Отчеты о производительности
│   ├── 📂 security/                   # Отчеты по безопасности
│   ├── 📂 usage-analytics/            # Аналитика использования
│   ├── 📂 compliance/                 # Отчеты соответствия требованиям
│   ├── 📂 quarterly/                  # Квартальные отчеты
│   ├── 📂 incident-reports/           # Отчеты об инцидентах
│   └── 📂 improvement-plans/          # Планы улучшений
├── 📚 resources/                   # Дополнительные ресурсы и материалы
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 glossary.md                 # Словарь терминов
│   ├── 📄 faq.md                      # Часто задаваемые вопросы
│   ├── 📄 community.md                # Ресурсы сообщества
│   ├── 📄 external-links.md           # Полезные внешние ссылки
│   ├── 📂 tools/                      # Рекомендуемые инструменты
│   ├── 📂 templates/                  # Шаблоны документов
│   └── 📂 checklists/                 # Чек-листы для различных задач
├── 🛠️ troubleshooting/             # Устранение неполадок и FAQ
│   ├── 📄 _category_.yml             # Метаданные категории
│   ├── 📄 index.md                   # Обзор секции
│   ├── 📄 common-issues.md            # Часто встречающиеся проблемы
│   ├── 📄 error-codes.md              # Справочник кодов ошибок
│   ├── 📄 diagnostic-tools.md         # Инструменты диагностики
│   ├── 📂 performance/                # Проблемы производительности
│   ├── 📂 connectivity/               # Проблемы соединения
│   ├── 📂 configuration/              # Проблемы конфигурации
│   ├── 📂 security/                   # Проблемы безопасности
│   └── 📂 emergency/                  # Экстренные процедуры
├── 📖 tutorials/                   # Пошаговые обучающие материалы
│   ├── 📄 _category_.yml           # Метаданные категории
│   ├── 📄 index.md                 # Обзор секции
│   ├── 📂 basics/                    # Основы для начинающих
│   |   ├── 📄 _category_.yml           # Метаданные категории
│   │   ├── 📄 01-introduction.md  # Введение в систему
│   │   ├── 📄 02-first-steps.md     # Первые шаги
│   │   └── 📄 03-basic-concepts.md  # Базовые концепции
│   ├── 📂 intermediate/              # Промежуточный уровень
│   ├── 📂 advanced/                  # Продвинутые темы
│   ├── 📂 integrations/              # Туториалы по интеграциям
│   ├── 📂 best-practices/            # Лучшие практики
│   └── 📂 video-guides/              # Видео-руководства
└── 📚 user-guides/                   # Задаче-ориентированные руководства
    ├── 📄 _category_.yml
    ├── 📄 index.md
    ├── 📄 core-concepts.md          # Фундаментальные концепции
    ├── 📄 common-workflows.md       # Типичные рабочие процессы
    ├── 📄 advanced-features.md      # Продвинутые возможности
    ├── 📄 best-practices.md         # Проверенные лучшие практики
    ├── 📄 performance-optimization.md # Оптимизация производительности
    ├── 📄 security-guide.md         # Рекомендации по безопасности
    └── 📄 migration-guide.md        # Миграция между версиями

```

## 🎯 Docusaurus-Специфичные Требования

### 📋 Обязательные Элементы для Docusaurus

#### Структурные требования:

```yaml
docusaurus_обязательные_элементы:
  файловая_структура:
    - index_files: "Каждая папка docs/ ДОЛЖНА содержать index.md или index.md"
    - category_metadata: "Каждая папка ДОЛЖНА содержать _category_.yml для настройки sidebar"
    - numeric_prefixes: "Используйте числовые префиксы (01-, 02-) для принудительного порядка"
    - extension_rules: ".md для интерактивного контента, .md для статичного"

  именование_файлов:
    - kebab_case: "Используйте kebab-case для имен файлов (getting-started.md)"
    - no_spaces: "Никаких пробелов в именах файлов"
    - no_special_chars: "Избегайте специальных символов (&, %, #, ?)"
    - descriptive_names: "Имена должны описывать содержание"
```

#### Файлы _category_.yml для организации Sidebar:

```yaml
# docs/getting-started/_category_.yml
label: "Быстрый старт" # Название категории в sidebar
position: 1 # Позиция среди других категорий
link: # Настройки ссылки категории
  type: generated-index # Автогенерируемая индексная страница
  title: Быстрый старт с нашим продуктом # Заголовок для индексной страницы
  description: | # Описание для индексной страницы
    Быстро начните работу с нашим продуктом за несколько простых шагов.
    Эта секция содержит все необходимое для успешного старта.
  slug: /getting-started # Кастомный slug для категории
collapsible: true # Можно ли сворачивать категорию
collapsed: false # Свернута ли категория по умолчанию
className: getting-started-category # CSS класс для стилизации
customProps: # Кастомные свойства
  icon: "🚀" # Иконка для категории
  highlight: true # Выделить категорию
```

### 📋 Правила организации

#### 1. Корневая директория

- **Минимализм**: Только essential файлы
- **Документация**: README, LICENSE, CHANGELOG, CONTRIBUTING
- **Конфигурация**: Основные конфиг файлы проекта
- **НЕ размещать**: Временные файлы, скрипты, тесты

#### 2. Исходный код

- **cmd/**: Точки входа приложений
- **pkg/**: Публичные, переиспользуемые пакеты
- **internal/**: Приватная логика приложения
- **Разделение**: Четкое разделение публичного и приватного API

#### 3. Документация

- **docs/**: Вся проектная документация
- **README файлы**: В каждой важной директории
- **Архив**: Устаревшие документы в docs/archive/
- **Актуальность**: Обновление при изменении кода

#### 4. Тесты

- **tests/**: Централизованное хранение тестов
- **Организация**: По типам (unit, integration, e2e)
- **Mocks**: Отдельная директория для mock объектов
- **Coverage**: Минимум 80% покрытие

#### 5. Скрипты

- **scripts/**: Все скрипты автоматизации
- **Именование**: Описательные имена с подчеркиванием
- **Документация**: README в scripts/ директории
- **Архив**: Устаревшие скрипты в scripts/archive/

#### 6. Конфигурация

- **configs/**: YAML/JSON конфигурации
- **deployments/**: Deployment специфичные конфиги
- **.env файлы**: В корне для локальной разработки
- **Секреты**: В .private/ (не коммитить!)

#### 7. Плагины

- **plugins/**: Системные плагины
- **examples/**: Примеры плагинов
- **templates/**: Шаблоны для создания плагинов
- **Документация**: README в каждом плагине

### 🎯 Преимущества структуры

1. **Ясность**: Понятно где что находится
2. **Масштабируемость**: Легко добавлять новые компоненты
3. **Изоляция**: Четкое разделение ответственности
4. **Тестируемость**: Организованные тесты
5. **Безопасность**: Изоляция конфиденциальных данных
6. **CI/CD**: Оптимизация для автоматизации
7. **Онбординг**: Быстрое понимание проекта

### 📝 Checklist для новых файлов

- [ ] Правильная директория согласно типу файла
- [ ] Описательное имя файла
- [ ] README в новой директории
- [ ] Обновлен .gitignore если нужно
- [ ] Документация обновлена
- [ ] Тесты добавлены
- [ ] Импорты корректны

---

### 🎯 Пользователе-Центричная Навигация

**Организация по Пользовательским Ролям:**

```yaml
навигация_по_ролям:
  новые_пользователи:
    точки_входа:
      - "getting-started/quickstart.md" # 5-минутный старт
      - "getting-started/installation.md" # Настройка
      - "getting-started/first-steps.md" # Первые задачи
    путь_обучения:
      - tutorials/ # Структурированное обучение
      - examples/ # Практические примеры
      - user-guides/ # Углубленные руководства

  опытные_пользователи:
    точки_входа:
      - "reference/" # Техническая справка
      - "how-to/" # Решения конкретных задач
      - "integration/" # Продвинутые интеграции
    инструменты_эффективности:
      - "search functionality" # Быстрый поиск
      - "API reference" # Техническая документация
      - "troubleshooting/" # Быстрое решение проблем

  разработчики:
    технические_ресурсы:
      - "architecture/" # Системный дизайн
      - "reference/api/" # API документация
      - "contributing/" # Разработка и вклад
    инструменты_разработки:
      - "examples/" # Образцы кода
      - "integration/" # SDK и библиотеки
      - "deployment/" # DevOps и CI/CD
```

## 📋 Детальная Структура Директорий (Docusaurus)

### 📋 Frontmatter для Docusaurus

```yaml
---
# Обязательные поля для Docusaurus
id: unique-document-id # Уникальный ID документа
title: "Заголовок документа" # Заголовок для navbar и meta
description: "Описание для SEO" # Meta description (макс 160 символов)

# Навигация и структура
sidebar_label: "Краткий заголовок" # Короткий заголовок для sidebar
sidebar_position: 1 # Позиция в sidebar (число)
hide_title: false # Скрыть заголовок на странице
hide_table_of_contents: false # Скрыть оглавление
toc_min_heading_level: 2 # Минимальный уровень заголовков в TOC
toc_max_heading_level: 3 # Максимальный уровень заголовков в TOC

# SEO и метаданные
keywords: [keyword1, keyword2, keyword3] # Ключевые слова для SEO
image: /img/social-card.png # Изображение для социальных сетей
slug: /custom-url-path # Кастомный URL путь

# Дополнительные поля (расширенные)
last_update:
  date: 2025-01-15
  author: Author Name
tags: [tag1, tag2, tag3] # Теги для группировки
draft: false # Черновик (не будет опубликован)
unlisted: false # Не показывать в навигации
pagination_prev: null # Предыдущая страница
pagination_next: getting-started/installation # Следующая страница

# Кастомные поля проекта
audience: [developer, devops, user] # Целевая аудитория
complexity: beginner # Уровень сложности
estimated_time: "5 minutes" # Время чтения/выполнения
version: "1.0.0" # Версия документа
status: active # Статус документа
canonical_url: "/docs/canonical-path" # Каноническая ссылка
wcag_level: "AAA" # Уровень доступности

# Переводы и локализация
locale: ru # Локаль документа
translators: [translator1, translator2] # Переводчики
translation_status: completed # Статус перевода

# Для разработчиков
source_of_truth: true # Является ли источником истины
api_version: "2.0" # Версия API
---
```

### 🏷️ Файлы _category_.yml для Организации Sidebar

```yaml
# docs/getting-started/_category_.yml
label: "Быстрый старт" # Название категории в sidebar
position: 1 # Позиция среди других категорий
link: # Настройки ссылки категории
  type: generated-index # Автогенерируемая индексная страница
  title: Быстрый старт с нашим продуктом # Заголовок для индексной страницы
  description: | # Описание для индексной страницы
    Быстро начните работу с нашим продуктом за несколько простых шагов.
    Эта секция содержит все необходимое для успешного старта.
  slug: /getting-started # Кастомный slug для категории
collapsible: true # Можно ли сворачивать категорию
collapsed: false # Свернута ли категория по умолчанию
className: getting-started-category # CSS класс для стилизации
customProps: # Кастомные свойства
  icon: "🚀" # Иконка для категории
  highlight: true # Выделить категорию
```

### 📝 Улучшенные Стандарты Контента для Docusaurus

#### 1. MDX Компоненты и Интерактивность

````mdx
---
title: "Интерактивная документация API"
description: "Живые примеры использования API"
---

import Tabs from "@theme/Tabs";
import TabItem from "@theme/TabItem";
import CodeBlock from "@theme/CodeBlock";
import Admonition from "@theme/Admonition";

# API Аутентификация

<Admonition type="tip" title="Лучшая практика">
  Используйте API ключи для production окружения и токены для development.
</Admonition>

## Примеры запросов

<Tabs>
<TabItem value="curl" label="cURL">

```bash
curl -X POST https://api.example.com/auth \
  -H "Content-Type: application/json" \
  -d '{"username": "user", "password": "pass"}'
```
````

</TabItem>
<TabItem value="javascript" label="JavaScript">

```javascript
const response = await fetch("https://api.example.com/auth", {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
  },
  body: JSON.stringify({
    username: "user",
    password: "pass",
  }),
});
```

</TabItem>
<TabItem value="python" label="Python">

```python
import requests

response = requests.post('https://api.example.com/auth',
  json={
    'username': 'user',
    'password': 'pass'
  }
)
```

</TabItem>
</Tabs>

## Интерактивный пример

```mdx live
function AuthenticationExample() {
const [token, setToken] = useState('');

const authenticate = async () => {
// Симуляция API вызова
setToken('eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...');
};

return (
<div>
<button onClick={authenticate}>Получить токен</button>
{token && <p>Токен: <code>{token}</code></p>}
</div>
);
}
```

````

#### 2. Правила Именования для Docusaurus
```yaml
именование_файлов_docusaurus:
  обязательные_соглашения:
    - index_files: "index.md или index.md в каждой категории"
    - category_metadata: "_category_.yml в папках для настройки sidebar"
    - numeric_prefixes: "01-first.md, 02-second.md для принудительного порядка"
    - extension_consistency: ".md для интерактивного контента, .md для статичного"

  запрещенные_практики:
    - spaces_in_filenames: "Используйте kebab-case вместо пробелов"
    - special_characters: "Избегайте &, %, #, ? в именах файлов"
    - uppercase_extensions: "Используйте .md/.md, не .MD/.md"
    - reserved_words: "Избегайте _app, _document, _error как имена файлов"

  рекомендованная_структура:
    - category_index: "index.md для обзора категории"
    - numbered_order: "01-intro.md, 02-setup.md для последовательности"
    - semantic_names: "authentication.md, deployment.md"
    - subsections: "подпапки для группировки связанного контента"
````

#### 3. Адmonitions и Специальные Блоки

```markdown
:::note Примечание
Это важная информация, которую пользователи должны знать.
:::

:::tip Совет
Это полезный совет для более эффективной работы.
:::

:::info Информация
Дополнительная информация для контекста.
:::

:::caution Внимание
Будьте осторожны при выполнении этого действия.
:::

:::danger Опасность
Это может привести к потере данных или другим серьезным проблемам.
:::

:::warning Предупреждение
Устаревший функционал, который будет удален в будущих версиях.
:::
```

#### 4. Интеграция с Поиском и SEO

```yaml
seo_optimization:
  structured_headings:
    - h1_once: "Только один H1 заголовок на страницу"
    - logical_hierarchy: "H1 → H2 → H3 → H4 (без пропусков уровней)"
    - descriptive_headings: "Заголовки должны описывать содержание секции"

  meta_optimization:
    - title_length: "50-60 символов для title"
    - description_length: "150-160 символов для description"
    - keywords_relevance: "3-5 релевантных ключевых слов"
    - image_alt_text: "Описательный alt текст для всех изображений"

  internal_linking:
    - relative_links: "Используйте относительные ссылки между документами"
    - anchor_descriptive: "Описательные тексты ссылок (не 'нажмите здесь')"
    - breadcrumb_support: "Логическая иерархия для автогенерации breadcrumbs"
```

### 🚀 Автоматизация Docusaurus

#### 1. Сценарии Валидации Структуры

```bash
#!/bin/bash
# scripts/validate-docusaurus-structure.sh

echo "🔍 Валидация Docusaurus структуры..."

# Проверка обязательных файлов
required_files=(
  "docs/index.md"
  "docusaurus.config.js"
  "sidebars.js"
)

for file in "${required_files[@]}"; do
  if [[ ! -f "$file" ]]; then
    echo "❌ Отсутствует обязательный файл: $file"
    exit 1
  fi
done

# Проверка категорий
find docs -type d -not -path "*/.*" | while read -r dir; do
  if [[ -f "$dir/index.md" || -f "$dir/index.md" ]]; then
    echo "✅ Найден индексный файл в $dir"
  elif [[ "$dir" != "docs" ]]; then
    echo "⚠️  Отсутствует index.md в категории: $dir"
  fi

  if [[ -f "$dir/_category_.yml" ]]; then
    echo "✅ Метаданные категории найдены в $dir"
  elif [[ "$dir" != "docs" && $(find "$dir" -maxdepth 1 -name "*.md" -o -name "*.md" | wc -l) -gt 0 ]]; then
    echo "⚠️  Рекомендуется добавить _category_.yml в $dir"
  fi
done

echo "✅ Валидация завершена"
```

#### 2. Генератор Метаданных

```javascript
// scripts/generate-metadata.js
const fs = require("fs");
const path = require("path");
const yaml = require("yaml");

function generateCategoryMetadata(dirPath, categoryName, position) {
  const categoryData = {
    label: categoryName,
    position: position,
    link: {
      type: "generated-index",
      title: `${categoryName} - Документация`,
      description: `Полное руководство по ${categoryName.toLowerCase()}`,
      slug: `/${path.basename(dirPath)}`,
    },
    collapsible: true,
    collapsed: false,
  };

  const yamlContent = yaml.stringify(categoryData);
  fs.writeFileSync(path.join(dirPath, "_category_.yml"), yamlContent);
  console.log(`✅ Создан _category_.yml для ${categoryName}`);
}

// Автоматическое создание метаданных для всех категорий
const docsDir = "docs";
const categories = [
  { name: "getting-started", label: "Быстрый старт", position: 1 },
  { name: "tutorials", label: "Обучающие материалы", position: 2 },
  { name: "user-guides", label: "Руководства пользователя", position: 3 },
  { name: "how-to", label: "Инструкции", position: 4 },
  { name: "api", label: "API Справочник", position: 5 },
  { name: "reference", label: "Справочник", position: 6 },
];

categories.forEach((category) => {
  const categoryPath = path.join(docsDir, category.name);
  if (fs.existsSync(categoryPath)) {
    generateCategoryMetadata(categoryPath, category.label, category.position);
  }
});
```

#### 3. Конфигурация Docusaurus

````javascript
// docusaurus.config.js
const config = {
  title: 'Документация Проекта',
  tagline: 'Комплексная техническая документация',
  url: 'https://docs.example.com',
  baseUrl: '/',

  presets: [
    [
      'classic',
      {
        docs: {
          sidebarPath: require.resolve('./sidebars.js'),
          editUrl: 'https://github.com/example/docs/tree/main/',
          routeBasePath: '/',
          showLastUpdateAuthor: true,
          showLastUpdateTime: true,
          remarkPlugins: [
            [require('@docusaurus/remark-plugin-npm2yarn'), {sync: true}]
          ],
        },
        theme: {
          customCss: require.resolve('./src/css/custom.css'),
        },
        sitemap: {
          changefreq: 'weekly',
          priority: 0.5,
        },
      },
    ],
  ],

  themeConfig: {
    navbar: {
      title: 'Документация',
      logo: {
        alt: 'Логотип проекта',
        src: 'img/logo.svg',
      },
      items: [
        {
          type: 'search',
          position: 'right',
        },
        {
          href: 'https://github.com/example/project',
          label: 'GitHub',
          position: 'right',
        },
      ],
    },

    footer: {
      style: 'dark',
      links: [
        {
          title: 'Документация',
          items: [
            {
              label: 'Быстрый старт',
              to: '/getting-started',
            },
            {
              label: 'API Справочник',
              to: '/api',
            },
          ],
        },
        {
          title: 'Сообщество',
          items: [
            {
              label: 'GitHub',
              href: 'https://github.com/example/project',
            },
          ],
        },
      ],
    },

    // Улучшенный поиск
    algolia: {
      appId: 'YOUR_APP_ID',
      apiKey: 'YOUR_SEARCH_API_KEY',
      indexName: 'YOUR_INDEX_NAME',
      contextualSearch: true,
      searchParameters: {},
      searchPagePath: 'search',
    },

    // Код блоки с улучшенной подсветкой
    prism: {
      theme: require('prism-react-renderer/themes/github'),
      darkTheme: require('prism-react-renderer/themes/dracula'),
      additionalLanguages: ['bash', 'yaml', 'json'],
    },
  },

  plugins: [
    // Плагин для диаграмм Mermaid
    '@docusaurus/theme-mermaid',

    // Плагин для OpenAPI документации
    [
      'docusaurus-plugin-openapi-docs',
      {
        id: "api",
        docsPluginId: "classic",
        config: {
          api: {
            specPath: "api/openapi.yaml",
            outputDir: "docs/api",
            sidebarOptions: {
              groupPathsBy: "tag",
            },
          }
        }
      },
    ],
  ],

  markdown: {
    mermaid: true,
  },

  themes: [
    '@docusaurus/theme-mermaid',
    'docusaurus-theme-openapi-docs'
  ],
};
```README

#### 4. Автоматическая Генерация Sidebar
```javascript
// sidebars.js
const sidebars = {
  // Автоматически генерируемый sidebar
  tutorialSidebar: [
    {
      type: 'autogenerated',
      dirName: '.',
    },
  ],

  // Или кастомный sidebar для более точного контроля
  manualSidebar: [
    'index',
    {
      type: 'category',
      label: 'Быстрый старт',
      items: [
        'getting-started/index',
        'getting-started/quickstart',
        'getting-started/installation',
        'getting-started/first-steps',
      ],
    },
    {
      type: 'category',
      label: 'API Справочник',
      collapsed: false,
      items: [
        'api/index',
        'api/authentication',
        {
          type: 'autogenerated',
          dirName: 'api/endpoints',
        },
      ],
    },
  ],
};

module.exports = sidebars;
````

## 🤖 Автоматизированное Управление Структурой

### 🔧 Автоматические Валидации Структуры

```yaml
# .github/workflows/docs-structure-validation.yml
структурные_проверки:
  обязательные_файлы:
    - "docs/README.md": "Главная точка входа обязательна"
    - "docs/getting-started/": "Директория быстрого старта обязательна"
    - "CHANGELOG.md": "История изменений в корне проекта обязательна"

  соглашения_об_именах:
    - pattern: "kebab-case для директорий"
    - pattern: "kebab-case.md для файлов"
    - forbidden: "Пробелы и специальные символы"

  структурная_целостность:
    - orphaned_files: "Обнаружение файлов без ссылок"
    - broken_links: "Проверка всех внутренних ссылок"
    - missing_metadata: "Валидация frontmatter"
    - toc_sync: "Синхронизация оглавлений"
```

### 📊 Умная Генерация Навигации

```bash
# Автоматическое создание индексов и навигации
./scripts/docs/generate-navigation.sh

# Возможности:
# - Авто-генерация Index.md файлов для директорий
# - Создание интеллектуальных оглавлений
# - Генерация карты сайта
# - Обновление перекрестных ссылок
# - Создание пользовательских путей навигации
```

## 🔄 CI/CD Интеграция Структуры

### 🚀 Автоматическая Организация Контента

```yaml
# .github/workflows/content-organization.yml
организация_контента:
  структурный_линтинг:
    - file_placement: "Валидация размещения файлов в правильных директориях"
    - naming_conventions: "Соблюдение соглашений об именах"
    - structure_consistency: "Последовательность структуры по проектам"

  автоматические_улучшения:
    - index_generation: "Авто-создание индексных страниц"
    - cross_reference_updates: "Обновление связанного контента"
    - metadata_enrichment: "Добавление недостающих метаданных"
    - tag_optimization: "Умная система тегов для лучшего поиска"

  качественные_ворота:
    - completeness_check: "Все необходимые разделы присутствуют"
    - accessibility_validation: "Структурная доступность"
    - seo_optimization: "Структура оптимизирована для поиска"
    - mobile_responsiveness: "Навигация работает на мобильных"
```

### 📈 Мониторинг Использования Структуры

```bash
# Аналитика использования структуры документации
./scripts/docs/structure-analytics.sh

# Отслеживаемые метрики:
# - Наиболее используемые пути навигации
# - Показатели отказов по разделам
# - Эффективность поиска по структуре
# - Конверсионные воронки пользовательских путей
# - Пробелы в навигационном опыте
```

## 🌍 Адаптация для Различных Типов Проектов

> **Принцип**: Структура документации должна отражать природу и потребности конкретного типа проекта

### 💻 Для Программных Продуктов

```yaml
адаптация_софт_продуктов:
  обязательные_разделы:
    - "getting-started/" # Быстрая установка и настройка
    - "api/" # Полная API документация
    - "sdk/" # Software Development Kits
    - "examples/" # Работающие примеры кода

  специфичные_разделы:
    - "plugins/" # Расширения и плагины
    - "themes/" # Темы и кастомизация
    - "webhooks/" # Интеграционные хуки
    - "cli/" # Командная строка и инструменты
    - "migration/" # Руководства по миграции между версиями

  техническая_документация:
    - "reference/api/" # REST/GraphQL/gRPC API
    - "reference/database/" # Схемы и миграции БД
    - "architecture/" # Системная архитектура
    - "deployment/" # Развертывание и DevOps
    - "security/" # Модель безопасности и аутентификация

  разработчикам:
    - "contributing/setup/" # Настройка среды разработки
    - "contributing/workflow/" # Процесс разработки
    - "contributing/testing/" # Тестирование и QA
    - "contributing/release/" # Процесс релизов
```

### 📚 Для Библиотек и Фреймворков

```yaml
адаптация_библиотек:
  фокус_на_разработчиков:
    - "quickstart/" # 5-минутная интеграция
    - "installation/" # Все способы установки
    - "api-reference/" # Исчерпывающий API справочник
    - "cookbook/" # Рецепты для типичных задач

  специфичные_разделы:
    - "compatibility/" # Таблицы совместимости
    - "performance/" # Бенчмарки и оптимизация
    - "ecosystem/" # Связанные библиотеки и инструменты
    - "migration-guides/" # Переход между версиями
    - "internals/" # Внутреннее устройство для контрибьюторов

  примеры_по_сложности:
    - "examples/basic/" # Простые примеры
    - "examples/intermediate/" # Промежуточные
    - "examples/advanced/" # Продвинутые сценарии
    - "examples/real-world/" # Реальные проекты
```

### 🎨 Для Дизайн-Систем

```yaml
адаптация_дизайн_систем:
  визуальная_документация:
    - "foundation/" # Основы: цвета, типографика, spacing
    - "components/" # Библиотека UI компонентов
    - "patterns/" # Композиционные паттерны
    - "layouts/" # Сетки и макеты страниц
    - "icons/" # Иконочная система

  дизайн_специфичные_разделы:
    - "tokens/" # Дизайн-токены и их использование
    - "guidelines/" # Принципы и правила дизайна
    - "accessibility/" # Доступность и инклюзивность
    - "branding/" # Брендинговые элементы
    - "prototypes/" # Интерактивные прототипы

  для_разных_платформ:
    - "web/" # Веб-компоненты
    - "mobile/" # Мобильные паттерны
    - "print/" # Печатные материалы
    - "email/" # Email шаблоны

  инструменты:
    - "figma-library/" # Библиотека Figma
    - "code-snippets/" # Готовые фрагменты кода
    - "design-tokens-export/" # Экспорт токенов
```

### 🏢 Для Корпоративных Решений

```yaml
адаптация_enterprise:
  корпоративные_требования:
    - "compliance/" # Соответствие требованиям (GDPR, SOX, etc.)
    - "governance/" # Управление и политики
    - "audit/" # Аудит и отчетность
    - "risk-management/" # Управление рисками
    - "data-privacy/" # Конфиденциальность данных

  корпоративная_интеграция:
    - "sso/" # Single Sign-On
    - "ldap-ad/" # Интеграция с Active Directory
    - "enterprise-apis/" # Корпоративные API
    - "data-connectors/" # Коннекторы данных
    - "workflow-automation/" # Автоматизация процессов

  масштабирование:
    - "multi-tenant/" # Мультитенантность
    - "high-availability/" # Высокая доступность
    - "disaster-recovery/" # Аварийное восстановление
    - "capacity-planning/" # Планирование мощностей

  обучение_и_поддержка:
    - "admin-training/" # Обучение администраторов
    - "end-user-training/" # Обучение конечных пользователей
    - "certification/" # Программы сертификации
    - "support-procedures/" # Процедуры поддержки
```

### 🚀 Для SaaS Продуктов

```yaml
адаптация_saas:
  пользователь_центричный_подход:
    - "onboarding/" # Пошаговое знакомство с продуктом
    - "feature-guides/" # Подробные руководства по функциям
    - "use-cases/" # Сценарии использования
    - "best-practices/" # Лучшие практики

  бизнес_функции:
    - "billing/" # Биллинг и тарифы
    - "account-management/" # Управление аккаунтом
    - "team-collaboration/" # Командная работа
    - "permissions/" # Роли и права доступа
    - "data-export/" # Экспорт данных

  интеграции:
    - "api/" # REST API для интеграций
    - "webhooks/" # Уведомления о событиях
    - "zapier/" # Интеграция через Zapier
    - "third-party/" # Сторонние интеграции
```

### 📱 Для Мобильных Приложений

```yaml
адаптация_mobile:
  платформо_специфичные_разделы:
    - "ios/" # iOS специфичная документация
    - "android/" # Android специфичная документация
    - "cross-platform/" # Кроссплатформенные решения
    - "responsive/" # Адаптивность и responsive design

  мобильные_особенности:
    - "push-notifications/" # Push уведомления
    - "offline-mode/" # Работа офлайн
    - "device-permissions/" # Разрешения устройства
    - "biometric-auth/" # Биометрическая аутентификация
    - "deep-linking/" # Глубокие ссылки

  публикация:
    - "app-store/" # Публикация в App Store
    - "google-play/" # Публикация в Google Play
    - "beta-testing/" # Бета-тестирование
    - "review-guidelines/" # Рекомендации для ревью
```

### 🌐 Для Open Source Проектов

```yaml
адаптация_open_source:
  сообщество_центричный_подход:
    - "community/" # Сообщество и участие
    - "contributors/" # Руководство для контрибьюторов
    - "maintainers/" # Руководство для мейнтейнеров
    - "governance/" # Управление проектом
    - "code-of-conduct/" # Кодекс поведения

  прозрачность:
    - "roadmap/" # Публичная дорожная карта
    - "decisions/" # Архитектурные решения (ADR)
    - "meetings/" # Протоколы встреч
    - "rfcs/" # Request for Comments
    - "project-status/" # Статус проекта

  вклад_в_проект:
    - "first-contribution/" # Первый вклад
    - "development-setup/" # Настройка среды разработки
    - "testing/" # Тестирование
    - "documentation/" # Написание документации
    - "translation/" # Переводы
```

### 🎓 Для Образовательных Проектов

```yaml
адаптация_educational:
  структурированное_обучение:
    - "curriculum/" # Учебная программа
    - "lessons/" # Структурированные уроки
    - "exercises/" # Практические упражнения
    - "assessments/" # Тесты и оценки
    - "projects/" # Учебные проекты

  поддержка_обучения:
    - "prerequisites/" # Предварительные требования
    - "learning-paths/" # Траектории обучения
    - "glossary/" # Словарь терминов
    - "references/" # Справочные материалы
    - "additional-resources/" # Дополнительные ресурсы

  для_преподавателей:
    - "instructor-guide/" # Руководство преподавателя
    - "lesson-plans/" # Планы уроков
    - "grading-rubrics/" # Критерии оценивания
    - "classroom-setup/" # Настройка аудитории
```

### 🤖 Для AI/ML Проектов

```yaml
адаптация_ai_ml:
  специфика_машинного_обучения:
    - "models/" # Документация моделей
    - "datasets/" # Описание наборов данных
    - "training/" # Процесс обучения
    - "inference/" # Использование модели
    - "evaluation/" # Метрики и оценка

  технические_аспекты:
    - "model-architecture/" # Архитектура моделей
    - "hyperparameters/" # Гиперпараметры
    - "preprocessing/" # Предобработка данных
    - "deployment/" # Развертывание моделей
    - "monitoring/" # Мониторинг в продакшене

  этика_и_безопасность:
    - "bias-fairness/" # Предвзятость и справедливость
    - "privacy/" # Конфиденциальность
    - "interpretability/" # Интерпретируемость
    - "responsible-ai/" # Ответственный ИИ
```

### 🔬 Для IoT/Hardware Проектов

```yaml
адаптация_iot_hardware:
  аппаратная_документация:
    - "hardware-specs/" # Технические характеристики
    - "schematics/" # Схемы и диаграммы
    - "assembly/" # Сборка устройства
    - "firmware/" # Прошивка
    - "calibration/" # Калибровка

  подключение_и_настройка:
    - "device-setup/" # Настройка устройства
    - "connectivity/" # Подключение (WiFi, Bluetooth, etc.)
    - "protocols/" # Протоколы связи
    - "cloud-integration/" # Интеграция с облаком
    - "edge-computing/" # Граничные вычисления

  обслуживание:
    - "maintenance/" # Техническое обслуживание
    - "troubleshooting-hardware/" # Устранение аппаратных проблем
    - "updates/" # Обновления прошивки
    - "replacement-parts/" # Запасные части
```

### 🏛️ Для Государственных/Регулируемых Проектов

```yaml
адаптация_government:
  соответствие_требованиям:
    - "regulations/" # Нормативные требования
    - "standards/" # Стандарты и спецификации
    - "certifications/" # Сертификации
    - "audit-trail/" # Аудиторский след
    - "legal-compliance/" # Правовое соответствие

  прозрачность_и_подотчетность:
    - "public-reports/" # Публичные отчеты
    - "foi-responses/" # Ответы на запросы информации
    - "transparency-logs/" # Журналы прозрачности
    - "public-consultations/" # Публичные консультации

  доступность:
    - "accessibility/" # Доступность для всех групп населения
    - "multilingual/" # Многоязычность
    - "digital-inclusion/" # Цифровая инклюзивность
    - "plain-language/" # Простой язык
```

### 🧪 Для Научно-исследовательских Проектов

```yaml
адаптация_research:
  научная_документация:
    - "methodology/" # Методология исследования
    - "experiments/" # Описание экспериментов
    - "results/" # Результаты исследований
    - "publications/" # Публикации и статьи
    - "datasets/" # Научные данные

  воспроизводимость:
    - "reproducibility/" # Воспроизводимость результатов
    - "code-availability/" # Доступность кода
    - "data-sharing/" # Совместное использование данных
    - "computational-environment/" # Вычислительная среда

  сотрудничество:
    - "collaboration/" # Научное сотрудничество
    - "peer-review/" # Экспертная оценка
    - "conferences/" # Конференции и мероприятия
    - "funding/" # Финансирование исследований
```

## 📊 Аналитика и Оптимизация Структуры

### 🎯 Метрики Эффективности Структуры

```yaml
метрики_структуры:
  навигационная_эффективность:
    - average_clicks_to_target: "<3 клика до нужной информации"
    - search_success_rate: ">85% успешных поисков"
    - bounce_rate_by_section: "<20% показатель отказов"
    - user_flow_completion: ">70% завершение пользовательских путей"

  контентная_обнаруживаемость:
    - search_result_relevance: ">90% релевантность результатов"
    - cross_reference_usage: "Активное использование связанного контента"
    - content_coverage: "100% ключевых тем покрыто"
    - update_propagation: "Автоматическое распространение обновлений"

  пользовательское_удовлетворение:
    - task_completion_rate: ">85% успешное завершение задач"
    - time_to_information: "<2 минуты до нужной информации"
    - user_satisfaction_score: ">4.5/5 по структуре навигации"
    - return_user_engagement: ">60% пользователей возвращаются"
```

### 🔄 Непрерывная Оптимизация

```bash
# Система непрерывного улучшения структуры
./scripts/docs/structure-optimization.sh

# Процесс оптимизации:
# 1. Анализ паттернов использования пользователей
# 2. Выявление болевых точек навигации
# 3. A/B тестирование структурных изменений
# 4. Реализация улучшений на основе данных
# 5. Мониторинг влияния изменений
# 6. Документирование лучших практик
```

## 🎉 Ожидаемые Результаты

### 🚀 Для Пользователей:

- ✅ **Интуитивная навигация** - находите нужную информацию за <30 секунд
- ✅ **Прогрессивное обучение** - от новичка к эксперту по четкому пути
- ✅ **Многоканальный доступ** - одинаково хорошо работает на всех устройствах
- ✅ **Контекстная помощь** - релевантная информация в нужное время

### 👨‍💻 Для Команды Документации:

- ✅ **Масштабируемая система** - легко добавлять новый контент
- ✅ **Автоматизированное обслуживание** - структура поддерживается автоматически
- ✅ **Консистентность качества** - единые стандарты по всей документации
- ✅ **Data-driven оптимизация** - решения основаны на реальном использовании

### 💼 For Organization:

- ✅ **Сниженные затраты поддержки** через лучшую самообслуживающуюся документацию
- ✅ **Ускоренная адаптация** новых пользователей и сотрудников
- ✅ **Улучшенное удовлетворение клиентов** через лучший опыт документации
- ✅ **Конкурентное преимущество** через превосходную документацию

---

## 🚨 Критические Принципы Успеха

> **Пользователи Важнее Технических Ограничений**: Организуйте для успеха пользователей, не для удобства техники
>
> **Данные Стимулируют Структуру**: Регулярно анализируйте использование и оптимизируйте соответственно
>
> **Простота Важнее Полноты**: Лучше простая навигация чем исчерпывающая но сложная
>
> **Консистентность Обеспечивает Предсказуемость**: Пользователи должны знать что ожидать

**Помните**: Лучшая структура документации невидима - она просто работает и помогает пользователям добиваться успеха без размышлений о навигации.

---

## 🚀 Docusaurus-Совместимые Расширения

### 📋 Адаптация для Современных Static Site Generators

**Расширения для Docusaurus 2.0+:**

```yaml
docusaurus_compatibility:
  обязательные_файлы:
    - index_files: "index.md в каждой категории для автогенерации sidebar"
    - category_metadata: "_category_.yml для настройки навигации"
    - numeric_prefixes: "01-intro.md, 02-setup.md для принудительного порядка"

  enhanced_frontmatter:
    - id: "unique-document-id"
    - sidebar_label: "Короткое название для навигации"
    - sidebar_position: "Числовая позиция в sidebar"
    - description: "SEO описание (макс 160 символов)"
    - keywords: ["keyword1", "keyword2", "keyword3"]
    - slug: "/custom-url-path"
    - hide_table_of_contents: false

  mdx_integration:
    - interactive_components: "React компоненты в документации"
    - tabs_and_admonitions: "Расширенное форматирование"
    - live_code_blocks: "Интерактивные примеры кода"
    - dynamic_content: "Условный контент на основе JSX"
```

### 📁 Docusaurus-Оптимизированная Структура

**Пример категории с полной Docusaurus совместимостью:**

```
docs/
├── index.md                           # Главная страница документации
├── getting-started/
│   ├── _category_.yml                # label: 'Быстрый старт', position: 1
│   ├── index.md                      # Обзор секции (автогенерируется в sidebar)
│   ├── 01-quickstart.md             # Быстрый старт (MDX для интерактивности)
│   ├── 02-installation.md           # Установка
│   ├── 03-configuration.md          # Конфигурация
│   └── 04-verification.md           # Верификация
├── api/
│   ├── _category_.yml                # label: 'API Reference', position: 2
│   ├── index.md                  # Интерактивная API документация
│   ├── authentication.md            # С живыми примерами
│   └── endpoints/
│       ├── _category_.yml
│       ├── users.md
│       └── admin.md
└── troubleshooting/
    ├── _category_.yml                # label: 'Troubleshooting', position: 10
    ├── index.md
    ├── common-issues.md             # С интерактивными решениями
    └── diagnostic-tools.md
```

### 🏷️ Типовой _category_.yml

```yaml
# docs/getting-started/_category_.yml
label: "Быстрый старт"
position: 1
link:
  type: generated-index
  title: Быстрый старт с нашим продуктом
  description: |
    Быстро начните работу за несколько простых шагов.
    Эта секция содержит все необходимое для успешного старта.
  slug: /getting-started
collapsible: true
collapsed: false
customProps:
  icon: "🚀"
  highlight: true
```

### 📝 Расширенный Frontmatter для Docusaurus

```yaml
---
# Обязательные поля Docusaurus
id: unique-document-id
title: "Заголовок документа"
description: "SEO описание (макс 160 символов)"

# Навигация
sidebar_label: "Короткий заголовок"
sidebar_position: 1
hide_title: false
hide_table_of_contents: false
toc_min_heading_level: 2
toc_max_heading_level: 3

# SEO и метаданные
keywords: [keyword1, keyword2, keyword3]
image: /img/social-card.png
slug: /custom-url-path

# Дополнительные поля
last_update:
  date: 2025-01-15
  author: Author Name
tags: [tag1, tag2, tag3]
draft: false
unlisted: false
pagination_prev: null
pagination_next: getting-started/installation

# Кастомные поля проекта
audience: [developer, devops, user]
complexity: beginner
estimated_time: "5 minutes"
version: "1.0.0"
status: active
wcag_level: "AAA"
---
```

### 🎨 MDX Компоненты и Интерактивность

**Примеры использования MDX в документации:**

````mdx
import Tabs from "@theme/Tabs";
import TabItem from "@theme/TabItem";
import Admonition from "@theme/Admonition";

# API Аутентификация

<Admonition type="tip" title="Лучшая практика">
  Используйте API ключи для production окружения и токены для development.
</Admonition>

## Примеры запросов

<Tabs>
<TabItem value="curl" label="cURL">

```bash
curl -X POST https://api.example.com/auth \
  -H "Content-Type: application/json" \
  -d '{"username": "user", "password": "pass"}'
```
````

</TabItem>
<TabItem value="javascript" label="JavaScript">

```javascript
const response = await fetch("https://api.example.com/auth", {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
  },
  body: JSON.stringify({
    username: "user",
    password: "pass",
  }),
});
```

</TabItem>
<TabItem value="python" label="Python">

```python
import requests

response = requests.post('https://api.example.com/auth',
  json={
    'username': 'user',
    'password': 'pass'
  }
)
```

</TabItem>
</Tabs>

## Интерактивный пример

```mdx live
function AuthenticationExample() {
const [token, setToken] = useState('');

const authenticate = async () => {
// Симуляция API вызова
setToken('eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...');
};

return (
<div>
<button onClick={authenticate}>Получить токен</button>
{token && <p>Токен: <code>{token}</code></p>}
</div>
);
}
```

````

### 📐 Детальные Правила Именования для Docusaurus

```yaml
именование_файлов_docusaurus:
  обязательные_соглашения:
    - index_files: "index.md или index.mdв каждой категории"
    - category_metadata: "_category_.yml в папках для настройки sidebar"
    - numeric_prefixes: "01-first.md, 02-second.md для принудительного порядка"
    - extension_consistency: ".md для интерактивного контента, .md для статичного"

  запрещенные_практики:
    - spaces_in_filenames: "Используйте kebab-case вместо пробелов"
    - special_characters: "Избегайте &, %, #, ? в именах файлов"
    - uppercase_extensions: "Используйте .md/.md, не .md/.md"
    - reserved_words: "Избегайте _app, _document, _error как имена файлов"

  рекомендованная_структура:
    - category_index: "index.md для обзора категории"
    - numbered_order: "01-intro.md, 02-setup.md для последовательности"
    - semantic_names: "authentication.md, deployment.md"
    - subsections: "подпапки для группировки связанного контента"
````

### 🎨 Admonitions и Специальные Блоки

```markdown
:::note Примечание
Это важная информация, которую пользователи должны знать.
:::

:::tip Совет
Это полезный совет для более эффективной работы.
:::

:::info Информация
Дополнительная информация для контекста.
:::

:::caution Внимание
Будьте осторожны при выполнении этого действия.
:::

:::danger Опасность
Это может привести к потере данных или другим серьезным проблемам.
:::

:::warning Предупреждение
Устаревший функционал, который будет удален в будущих версиях.
:::
```

### 🔍 SEO Оптимизация для Docusaurus

```yaml
seo_optimization:
  structured_headings:
    - h1_once: "Только один H1 заголовок на страницу"
    - logical_hierarchy: "H1 → H2 → H3 → H4 (без пропусков уровней)"
    - descriptive_headings: "Заголовки должны описывать содержание секции"

  meta_optimization:
    - title_length: "50-60 символов для title"
    - description_length: "150-160 символов для description"
    - keywords_relevance: "3-5 релевантных ключевых слов"
    - image_alt_text: "Описательный alt текст для всех изображений"

  internal_linking:
    - relative_links: "Используйте относительные ссылки между документами"
    - anchor_descriptive: "Описательные тексты ссылок (не 'нажмите здесь')"
    - breadcrumb_support: "Логическая иерархия для автогенерации breadcrumbs"
```

### 🛠️ Автоматизация и Валидация

```bash
#!/bin/bash
# Пример валидации Docusaurus структуры

echo "🔍 Валидация Docusaurus структуры..."

# Проверка обязательных файлов
required_files=(
  "docs/index.md"
  "docusaurus.config.js"
  "sidebars.js"
)

for file in "${required_files[@]}"; do
  if [[ ! -f "$file" ]]; then
    echo "❌ Отсутствует обязательный файл: $file"
    exit 1
  fi
done

# Проверка структуры категорий
find docs -type d -mindepth 1 | while read -r dir; do
  if [[ ! -f "$dir/_category_.yml" ]]; then
    echo "⚠️ Отсутствует _category_.yml в: $dir"
  fi
  if [[ ! -f "$dir/index.md" && ! -f "$dir/index.md" ]]; then
    echo "⚠️ Отсутствует index.md/mdx в: $dir"
  fi
done

echo "✅ Валидация завершена"
```

---

**Версия**: 3.1.0 (Универсальная Структура + Docusaurus)
**Статус**: ✅ **Production-Ready**
**Адаптируемость**: 🌍 **Универсально для всех типов проектов**
**Docusaurus**: ✅ **Полная совместимость с v2.0+**
**Основано на**: Исследования пользователей + аналитика использования + лучшие практики индустрии
**Последнее обновление**: 2025-01-15

<!-- METADATA
{
  "created_at": "2025-01-15",
  "updated_at": "2025-01-15",
  "author": "Universal Documentation Structure Team",
  "version": "3.1.0",
  "status": "production_ready",
  "category": "universal_structure_docusaurus",
  "priority": "foundational",
  "scope": "universal",
  "user_tested": true,
  "analytics_driven": true,
  "automation_ready": true,
  "scalable": true,
  "docusaurus_compatible": true,
  "static_site_ready": true,
  "mdx_enabled": true,
  "seo_optimized": true,
  "language": "ru"
}
-->
