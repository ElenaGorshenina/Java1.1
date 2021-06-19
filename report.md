# Отчёт о тестировании валидации номера банковской карты.

## Краткое описание

09.06.21 было проведено функциональное тестирование приложения валидации номера банковской карты.

На тестирование затрачено: 01:30

В результате тестирования выявлены следующие дефекты:
* [При валидации номера банковской карты не принимает карту с номером больше 16 цифр](https://github.com/ElenaGorshenina/Java1.1/issues/1)
* [При валидации номера банковской карты не принимает карту с номером меньше 16 цифр](https://github.com/ElenaGorshenina/Java1.1/issues/2)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Домашнее задание к занятию «1.1. Введение в Java: JDK, JRE, JVM, IntelliJ IDEA»](https://github.com/netology-code/javaqa-homeworks/tree/master/intro);
* [Руководство по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md);
* [Генератор номеров кредитных карт](https://cartoved.ru/common/generator-kreditnyh-kart.html); 
* [freeformatter.com](https://www.freeformatter.com/credit-card-number-generator-validator.html).

В качестве тестовых данных использовались данные [Генератор номеров кредитных карт](https://cartoved.ru/common/generator-kreditnyh-kart.html) и [freeformatter.com](https://www.freeformatter.com/credit-card-number-generator-validator.html):
* 5404 3679 6305 9740
* 4125 8325 3563 0170
* 5592 0989 3618 4529
* 5315 7035 2390 8604 
* 5315 7167 8438 5478
* 5218 4113 1254 1051
* 4654 2400 0574 4191 
* 4105 9272 6491 3583
* 5937 6344 4145 3324
* 4485219688682543
* 5893361697459423
* 5464817415084099
* 5521457290956516
* 36218103270050 Diners Club - International: FAIL
* 6382488283889089
* 3533157834177675
* 4539049877436523564 VISA: FAIL
* 378875900700443 American Express (AMEX): FAIL

Тестирование производилось в следующем окружении:
* Windows 7 (64)
* Java 11.0.11

