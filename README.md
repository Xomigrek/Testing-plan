# Тестирование возможности записаться на обучение профессии «Тестировщик ПО»

## Перечень автоматизируемых сценариев.

1. Переход на страницу тестирования через Блок "Программирование" - "Тестировщик ПО"
    * Ожидаемый результат - открывается страница для тестирования
1. Переход на страницу тестирования через "Каталог курсов" - "Программирование" - "Тестировщик ПО"
    * Ожидаемый результат - открывается страница для тестирования
1. Happy path - запись на курс. В поле "Имя" водим валидное имя с "ё", "-", без спезсимволов, на русском и английском языке. В поле "Телефон" водим 11ти значный номер, начинающийся с "+7". Нажимаем на кнопку "Записаться"
    * Ожидаемый результат - форма принята, появилось сообщение "Ваша заявка принята"
1. Happy path - получить консультацию. В поле "Имя" водим валидное имя с "ё", "-", без спезсимволов, на русском и английском языке, длина имени от 2 до 60 символов. В поле "Телефон" водим 11ти значный номер, начинающийся с "+7". Нажимаем на кнопку "Получить консультацию"
    * Ожидаемый результат - форма принята, появилось сообщение "Ваша заявка принята"
1. Ввод невалидных значений в поле "Имя". В поле "Имя" вводим значение с спецсиволами или цифрами. В поле "Телефон" водим 11ти значный номер, начинающийся с "+7". Нажимаем на кнопку "Записаться" или "Получить консультацию"
    * Ожидаемый результат - Сообщение ошибки "Имя должно состоять из букв"
1. Ввод граничных значений в поле "Имя". В поле "Имя" вводим 0, 1, 61, 62 символа. В поле "Телефон" водим 11ти значный номер, начинающийся с "+7". Нажимаем на кнопку "Записаться" или "Получить консультацию"
    * Ожидаемый результат - Сообщение ошибки "Имя должно быть не короче 2 символов" или "Имя должно быть не длиннее 60 символов"
1. Ввод невалидных значений в поле "Телефон". В поле "Имя" вводим валидное значение. В поле "Телефон" вводим буквы, спецсимволы. Нажимаем на кнопку "Записаться" или "Получить консультацию"
    * Ожидаемый результат - Сообщение ошибки "Телефон должен состоять из цифр"
1. Ввод граничных значений в поле "Телефон". В поле "Имя" вводим валидное значение. В поле "Телефон" вводим 9,10,12,13 цифр. Нажимаем на кнопку "Записаться" или "Получить консультацию"
    * Ожидаемый результат - Сообщение ошибки "Телефон должен быть в формате +9 (999) 999-99-99"
1. Пустое значение в поле "Телефон". В поле "Имя" вводим валидное значение. Поле "Телефон" оставляем пустым. Нажимаем на кнопку "Записаться" или "Получить консультацию"
    * Ожидаемый результат - Сообщение ошибки "Телефон должен быть в формате +9 (999) 999-99-99"
## Перечень используемых инструментов с обоснованием выбора.
1. IDEA - требуется для написания автотестов
1. Система для сборки проекта Gradle
1. Библиотека Faker для генерации слуайных данных для тестирования
1. Selenide для написания тестов
1. Стандартная отчетность Gradle для предоставлени отчета о тестировании
## Перечень необходимых разрешений, данных и доступов.
Доступ к тестовому ресурсу или разрешение на тестирование на боевой среде
## Перечень и описание возможных рисков при автоматизации.
Изменение селекторов или интерфейса во время подготовки к тестированию
## Перечень необходимых специалистов для автоматизации.
Специалист по автоматическому тестированию
## Интервальная оценка с учётом рисков в часах.
4 часа для составления плана тестирования. 6 часов для написания и редактирования кода. 2 часа для подготовки отчета о проделанной работе 