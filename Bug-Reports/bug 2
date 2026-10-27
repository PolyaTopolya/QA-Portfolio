# BUG-d1234: POST /api/auth/register возвращает 400 для email длиной 41–50 символов

- **Проект:** API Authentication Service
- **Endpoint:** `POST http://2.59.41.2:7320/api/auth/register`
- **Окружение:** Google Chrome 151.0, Postman
- **Severity:** Major | **Priority:** High
- **Статус:** Open

## Описание
Сервер возвращает ошибку 400 Bad Request при отправке валидного email длиной от 41 до 50 символов, несмотря на то, что требования указывают `maxLength: 50`.

## Требования
- minLength: 6
- maxLength: 50
- Формат: валидный email

## Результаты тестирования граничных значений

| Длина email | Код ответа | Статус |
|-------------|------------|--------|
| 5           | 201        | ✅ OK (нижняя граница) |
| 6           | 201        | ✅ OK |
| 40          | 201        | ✅ OK |
| **41**      | **400**    | ❌ **BUG** |
| **50**      | **400**    | ❌ **BUG (верхняя граница!)** |
| 51          | 400        | ✅ OK (вне диапазона) |

## Шаги воспроизведения (cURL)
```bash
# Граничное значение 50 символов (должно работать, но не работает)
curl --location 'http://2.59.41.2:7320/api/auth/register' \
--header 'Content-Type: application/json' \
--data-raw '{
  "email": "Loowqwgerodikgkgkglflflfasgsdfsdfsdfsdfddfdfdfdfdf@gmail.com",
  "password": "M12asdf134@@"
}'
