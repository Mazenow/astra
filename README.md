# Автоматизированное тестирование веб-приложения

## Описание проекта

Этот проект представляет собой набор автоматизированных тестов для веб-приложения "astradisk", написанных с использованием Selenium WebDriver, Behave и Allure. 
Целью этих тестов является проверка функционала подтверждения действий при удалении файлов и каталогов.

Проект включает следующие компоненты:

Selenium WebDriver: инструмент для автоматизации браузеров, который позволяет тестировщикам управлять действиями браузера через код.
Python: язык программирования, используемый для написания тестов.
Behave: фреймворк для тестирования на Python, позволяющий легко создавать и запускать тесты.
Allure: инструмент генерации отчетов о результатах тестирования.

## Требования

Для запуска тестов необходимо 

1) Установка зависимостей:

- Python 3.12.4
- allure-behave                 2.13.5
- allure-python-commons         2.13.5
- behave                        1.2.6
- behave-html-formatter         0.9.10
- html-testRunner               1.2.1
- selenium                      4.25.0


## Установка

Шаг 1: Установка Python 3.12.4
Загрузите установочный файл Python 3.12.4 с официального сайта: https://www.python.org/downloads/release/python-3124/.Выберите версию, соответствующую вашей операционной системе (Windows, macOS, Linux).
Запустите установщик. Следуйте инструкциям мастера установки. Убедитесь, что вы поставили галочку напротив опции «Add Python to PATH» (если устанавливаете на Windows), чтобы команды Python были доступны через командную строку.
Проверьте установку, открыв терминал/командную строку и введя команду:
python --version
Должен отобразиться номер версии Python 3.12.4.

Шаг 2: Обновление pip до последней версии
Перед установкой пакетов рекомендуется обновить менеджер пакетов pip до самой актуальной версии:
python -m pip install --upgrade pip

Шаг 3: Установка необходимых зависимостей. Введите следующую команду в корневой директории проекта: pip install -r requirements.txt


## Запуск тестов
*Перед запуском теста убедитесь что что в облачных хранилищах "https://test-disk.promo.astradisk.ru/login" и "https://test-vanilla.promo.astradisk.ru/login" не размещены файлы "test_bmp.bmp" и "test_txt.txt"  *
1) Для запуска тестов - введите следующую команду в корневой директории проекта:	behave
2) Для формирования отчета в HTML - после проведения теста введите следующую команду в корневой директории проекта: allure generate '--clean'
3) Для открытия отчета в HTML введите следующую команду в корневой директории проекта: allure open
* Если вы хотите прогнать тесты с автоматическим формированием отчета - после запуска введите следующую команду в корневой директории проекта: 

