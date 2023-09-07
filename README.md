# Проект на позицию QA Automation (Python) OutStream
 
Проект содержит в себе тестовые сценарии поиска по тексту, с виртуальной клавиатуры и по картинке на странице Google.com

## Инструменты

- Python 3.10
- Selenium WebDriver
- PyTest
- WebdriverManager
- pyautogui
- Allure

## Структура проекта

Положительные сценарии для поиска по тексту и картинке

Проект организован следующим образом:

- `tests/` - директория с тестовыми файлами
- `pages/` - директория с классами страниц (Page Object Model). Здесь содержатся классы, описывающие элементы и поведение каждой страницы приложения.
- `conftest.py` - файл конфигурации для инициализации драйвера. Здесь вы можете настраивать фикстуры, которые будут использоваться в ваших тестовых сценариях.
- `results/` - директория с отчетами Allure Dashboard


## Установка и настройка

1. Создайте виртуальное окружение:
   ```shell
   python -m venv venv

2. Установите зависимости из файла requirements.txt:
   ```shell
   pip install -r requirements.txt


3. Для запуска тестов используйте команду:
   ```shell
   pytest tests/* --browser=firefox

4. Для визуализации результатов теста можно создать Allure результаты
   ```shell
   pytest tests/* --browser=firefox --alluredir=results
   allure serve results
  


