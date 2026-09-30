# Описание конфликта

Конфликт возник в файле api-plan.md, в строке с эндпоинтом GET /products.

- В ветке feature-pricing строка была изменена на: GET /products?category=all
- В ветке feature-cart строка была изменена на: GET /products?limit=20

При merge веток feature-cart и feature-pricing в main Git не смог автоматически
объединить изменения одной и той же строки, и возник конфликт.

Решение: строки объединены вручную в GET /products?category=all&limit=20,
после чего сделан отдельный коммит с исправлением.
