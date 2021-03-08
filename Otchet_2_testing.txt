Отчёт о тестировании приложения <Credit Card Number Validator>

Приложение <Credit Card Number Validator> представлен в виде кода на платформе Java 8+ , 
предназначен запуска программы с разными тестовыми данными для проверки валидности номеров кредитных карт.

<06.03.2021> - <06.03.2021> было проведено динамическое тестирование приложения <Credit Card Number Validator>.

На тестирование затрачено: <8 часов>

В результате тестирования выявлены следующие дефекты:

Запуск приложения <Credit Card Number Validator> данными
 Diners Club - Carte Blanche: 30106313883067 вызывает ошибку “Result is FAIL”.
https://docs.google.com/document/d/1mFJh2o-X3qp_g_DS0gYaC3tAkWov9QooNtqjXbaE-ng/edit?usp=sharing


В процессе тестирования осуществлялись "Запуск приложения <Credit Card Number Validator> параметрами 
из вебсайта по ссылке: https://www.freeformatter.com/credit-card-number-generator-validator.html.  


В процессе тестирования использовались следующие артефакты*:

Тест кейс: https://drive.google.com/file/d/1w_3Bls7clUHFrrAY7oPU3S-K3_kCreuj/view?usp=sharing



В качестве тестовых данных использовались данные:
 1.Увебсайта по ссылке: https://www.freeformatter.com/credit-card-number-generator-validator.html.
 
<Ожидаемый результат: Result is OK>


Тестирование производилось в следующем окружении:

<Windows 10 домашняя верси 1909 сборка ОС 18363.1379>
<openjdk version "11.0.10" 2021-01-19
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.10+9)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.10+9, mixed mode>
<Редактор кода"Intellij IDEA Community Edition 2020.3.2"
