Звіт про тестування Beet Seed (JSONPlaceholder)
Дата тестування: 24.07.2025
Тест-план: BeetSeedTest.jmx
Мета: Базове тестування GET, POST, PUT, PATCH, DELETE запитів до JSONPlaceholder з використанням Assertions та Listener'ів.
Висновки за Listener'ом "View Results in Tree"
GET Request - Posts
Усі ітерації запиту завершилися успішно (зелені іконки).
Assertions:
"GET Status Code 200": Пройдено.
"GET Size Assertion": Пройдено.
"GET Response Time < 2000ms": Пройдено (фактичний час відповіді був 50ms).
Вміст відповіді відповідає очікуваному (отримано пост з ID 1).
POST Request - Create Post
Усі ітерації запиту завершилися успішно.
Assertions:
"POST Status Code 201": Пройдено.
"POST Body Contains foo": Пройдено.
"POST Response Time < 2000ms": Пройдено (фактичний час відповіді був 161ms).
Сервер успішно створив новий ресурс і повернув його у відповіді.
PUT Request - Update Post
Усі ітерації запиту завершилися успішно.
Assertions:
"PUT Status Code 200": Пройдено.
"PUT Body Contains foo_updated": Пройдено.
"PUT Response Time < 2000ms":  Пройдено (фактичний час відповіді був 163ms)
Ресурс був успішно оновлений, і зміни відображені у відповіді.
PATCH Request - Partial Update Post
Усі ітерації запиту завершилися успішно.
Assertions:
"PATCH Status Code 200": Пройдено.
"PATCH Body Contains foo_patched": Пройдено.
"PATCH Response Time < 2000ms": Пройдено (фактичний час відповіді був 137ms).
Часткове оновлення ресурсу пройшло успішно, нове значення поля 'title' присутнє у відповіді.
DELETE Request - Delete Post
Усі ітерації запиту завершилися успішно.
Assertions:
"DELETE Status Code 200": Пройдено.
"DELETE Body Is Empty": Пройдено (відповідь була порожнім JSON-об'єктом {}).
"DELETE Response Time < 2000ms": Пройдено.
Запит на видалення був успішно оброблений сервером.
Висновки за Listener'ом "Summary Report"
Total Samples: Загальна кількість семплів - 15.
Average Response Time: Середній час відповіді за всіма запитами - 120 ms.
Error Rate: 0.00% (всі запити виконано без помилок).
Throughput: Total -  8,3/sec.
Мінімальний та максимальний час відповіді знаходились у прийнятних рамках.
Загальний висновок
Тестування базових HTTP-запитів (GET, POST, PUT, PATCH, DELETE) до JSONPlaceholder пройшло успішно. Усі запити повернули очікувані статуси та дані, і всі налаштовані твердження були пройдені. Продуктивність API на базовому рівні задовільна, середній час відповіді не перевищує очікуваних значень. JMeter успішно впорався з надсиланням запитів, виконанням і перевіркою тверджень, а також збором агрегованих результатів.

