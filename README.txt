Тестируемый API:  https://petstore.swagger.io/v2
ВАЖНО: адрес заканчивается на /v2.
Новый адрес petstore3.swagger.io сейчас не отвечает.
Если в браузере вы открыли другую ссылку — вернитесь на v2.

1. Создайте окружение и поставьте библиотеки:

   Windows:
     python -m venv .venv
     .venv\Scripts\activate

   macOS и Linux:
     python -m venv .venv
     source .venv/bin/activate

   Затем:
     pip install -r api_testing\requirements.txt

2. Проверьте, что API отвечает:

   python "Проверка API\check_api.py"

3. Разберитесь с базовым классом:

   api_testing\base_request.py

4. Напишите по 4 запроса на сущность store
   в файле api_testing\test_store.py

5. Напишите по 4 запроса на сущность user
   в файле api_testing\test_user.py

6. Запустите тесты:

   pytest -v

