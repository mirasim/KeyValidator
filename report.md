# Отчёт о тестировании KeyValidator

## Краткое описание

28/12/2020 - 28/12/2020 было проведено Функциональное тестирование приложения KeyValidator.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:
https://github.com/mirasim/KeyValidator/issues/1
https://github.com/mirasim/KeyValidator/issues/3


## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
1. KeyValidator.class 
2. [Руководство использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)

В качестве тестовых данных использовались данные Руководства использования KeyValidator:

##  Из списка ВАЛИДНЫХ ключей руководства использования KeyValidator:

* 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998- ОК
* 80b427f8-92cd-3aae-ba04-3927fbe17c6- FAIL - этот key короче на 1 символ чем все остальные. Заведен тикет https://github.com/mirasim/KeyValidator/issues/1 на исправление руководства
* b295bc63-9f03-3b4b-af80-969b39f8c262- ОК
* 387eedc6-12e9-3b32-9881-63b6b5e85317- FAIL - ожидалось, что будет валиндным Заведен тикет https://github.com/mirasim/KeyValidator/issues/3
* c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180- ОК




##  Из списка НЕВАЛИДНЫХ ключей руководства использования KeyValidator

* 18252235-78e0-44a5-8720-556f0c7da17a- FAIL
* e66075b6-ddad-445e-baf6-161b3289522b- FAIL
* b6d53250-f07e-4352-a293-6102ddf7f1ca- FAIL
* c2bc778a-1cb9-46c6-b435-0489649d2a42- FAIL
* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1- OK - ожидалось, что будет невалиндным. Заведен тикет https://github.com/mirasim/KeyValidator/issues/3

Тестирование производилось в следующем окружении:
* ОС Windows 10 X64
* Java-version build 11.0.9.1+1 
* Git CMD
