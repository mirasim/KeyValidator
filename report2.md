# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

29/12/2020 - 29/12/2020 было проведено Функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1 часа

В результате тестирования выявлены следующие дефекты: [Номера карт некоторых платежных систем не валидные](https://github.com/mirasim/KeyValidator/issues/2)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
1. [netology-code
    /
    javaqa-homeworks](https://github.com/netology-code/javaqa-homeworks/tree/master/intro)
2. [Руководство по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)
3. [Get Credit Card Numbers](https://www.getcreditcardnumbers.com/)

В качестве тестовых данных использовались данные [Get Credit Card Numbers](https://www.getcreditcardnumbers.com/):

##  Номера карт которые являются правильными,  приложение по приему платежей банковских карт показало что они Валидные:

* 4929303367938246 VISA - ОК
* 4485613184887889 VISA - ОК
* 5119103430388552 Mastercard - ОК
* 5504579995450379 Mastercard - ОК
* 3088522092924747 JCB - ОК
* 3112787178920865 JCB - OK
* 6011058069638601 Discover - OK
* 6011519312832036 Discover - OK

##  Номера карт которые являются правильными, но приложение по приему платежей банковских карт показало что они Невалидные:

* 372408972243013 American Express - FAIL
* 374669428592885 American Express - FAIL
* 30035654930544 Diners Club - FAIL
* 36980943127606 Diners Club - FAIL
* 869916358357231 Voyager - FAIL
* 869954080690074 Voyager - FAIL
* 4716819340636 Visa 13 digit - FAIL
* 4716240233483 Visa 13 digit - FAIL
* 214958300432391 enRoute - FAIL
* 214999526252783 enRoute - FAIL
* 210049740693315 JCB 15 digit - FAIL
* 180040312484122 JCB 15 digit - FAIL

## Номера карт некорректного ввода:
* 492930336793824622 (просто номер) - FAIL
* 4929303367938246Н (номер карты с добавлением буквы) - FAIL
* 4929303367938246,,,,,,! (номер карты с добавлением символов) - FAIL


## Тестирование производилось в следующем окружении:
* ОС Windows 10 X64
* Java-version build 11.0.9.1+1 
* Git CMD
* IntelliJ IDEA
