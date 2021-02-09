# Название проекта
Подключение сисетмы репортинга "Allure"
## Начало работы 
* У вас должна быть установлена IDEA
* У вас должен быть проект к которому не подключена система репортинга
## Установка и запуск
1. Зайдите на сайт https://github.com/allure-framework/allure2/releases/tag/2.13.8 и скачайте последнюю версию.
1. Создайте папку .allure в вашем проекте и положите в нее скачанную папку.
1. В файле build.gradle подключите allure ![билдгредл](https://sun9-24.userapi.com/impg/l-KzD_KhAzg7Ha3TQKxkXG-IYtJvlW1HRbqGsw/s2eOL4RB2Mk.jpg?size=822x452&quality=96&proxy=1&sign=492dbe2ec066293c8550ce8a9d0c543f&type=album)
1. Для интеграции с SELENIDE добавьте зависимость в файле build.gradle - testImplementation 'io.qameta.allure:allure-selenide:2.13.3' 
1. Подключите listener в тестах ![листенер в тестах](https://sun9-4.userapi.com/impg/GpxzeO2kxPaxyN4LpuSNi-35CqF4FQgLySMmJw/5PKdh64SbAU.jpg?size=810x212&quality=96&proxy=1&sign=08e26c6bf92ca357bfd13e6be6babf49&type=album)
1. Чтобы запустить систему в терминале IDEA пишем - gradlew clean test . Система прогонит тесты.
1. Для того чтобы снгенерировать отчет в терминале IDEA пишем gradlew allureReport . Сгенерированный отчет будет находится в вашем проекте в папке buid/reports/allure-report/index.html

![allure-report](https://sun9-56.userapi.com/impg/25xOS3Wgish9XcRXNPSiuBR-O_SF5JZ68m6eTQ/5XzENvki3n8.jpg?size=444x300&quality=96&proxy=1&sign=2ee4c11945be9b0b8f53bcc145be4f96&type=album)

Чтобы просмотреть его щелкаем правой кнопкой мыши по файлику и выбираем Open in browser и выбираем браузер в котором хотим посмотреть отчет.

8. Дополнительные инструкции по работе с Allure можно найти на сайте http://allure.qatools.ru , https://docs.qameta.io/allure/ .

# Лицензия
Дополнительные лицензии не требуются.
