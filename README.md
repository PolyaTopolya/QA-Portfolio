# QA Portfolio — Полина Мильниченок

Портфолио тестировщика: мануальное тестирование, API, тест-дизайн и документация.
Все артефакты основаны на практических заданиях и реальных кейсах.

## 🛠 Навыки и инструменты
- **Тест-дизайн:** граничные значения, классы эквивалентности, предугадывание ошибок
- **API Testing:** Postman, SoapUI, cURL, JSON/XML
- **Базы данных:** MongoDB (Compass, mongosh), CRUD-операции
- **Документация:** баг-репорты, чек-листы, тест-кейсы, отчеты
- **Окружения:** Web, Mobile (iOS/Android), Desktop

## 📂 Структура портфолио

| Папка | Что внутри | Объект / Проект |
|-------|------------|-----------------|
| [Bug-Reports](./Bug-Reports) | Баг-репорты с шагами, скриншотами и cURL | Twinby, Wildberries, API Auth |
| [API-Testing](./API-Testing) | Коллекции Postman, SoapUI проекты, негативные кейсы | Calculator SOAP, Auth API |
| [Checklists](./Checklists) | Чек-листы функционального, UI/UX, сетевого тестирования | Kufar (Mobile App) |
| [Test-Cases](./Test-Cases) | Тест-кейсы по техникам тест-дизайна | Registration API |
| [Test-Documentation](./Test-Documentation) | Отчеты о тестировании, описание окружений | Различные учебные проекты |
| [Database-Testing](./Database-Testing) | Запросы к MongoDB, проверка данных | Library DB |

## 🔥 Ключевые кейсы (рекомендую начать с них)

1. **[Баг в API регистрации](./Bug-Reports/API-auth-register-boundary-bug.md)** — найдено несоответствие требований maxLength через граничные значения (Postman + cURL).
2. **[Чек-лист мобильного приложения Kufar](./Checklists/kufar-mobile-checklist.md)** — полный цикл: инсталляция, навигация, сеть, безопасность, локализация.
3. **[Баг даты рождения в Twinby](./Bug-Reports/twinby-web-future-date-bug.md)** — классический функциональный баг с четкими предусловиями.
4. **[SOAP API Calculator](./API-Testing/soapui-calculator-project.md)** — тестирование legacy SOAP сервиса, TestSuite, assertions.

## 📌 Как читать это портфолио
- В **Bug-Reports** каждый баг оформлен по стандарту: ID, Steps, Actual/Expected Result, Evidence.
- В **API-Testing** есть не только позитивные запросы, но и негативные сценарии с объяснением ожидаемых кодов.
- В **Checklists** учтены нефункциональные требования: производительность, безопасность, совместимость.

> ⚠️ **Примечание:** Некоторые объекты (Twinby, Wildberries, Kufar) являются реальными сервисами. Баги зафиксированы в рамках учебных заданий. API-эндпоинты и тестовые данные предоставлены курсом.
