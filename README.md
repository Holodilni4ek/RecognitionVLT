# Проект: Распознавание автомобильных номеров

Этот проект предназначен для автоматического распознавания автомобильных номеров с изображений и проверки, разрешен ли въезд автомобиля на основе списка зарегистрированных номеров.

---

## Оглавление

1. [Требования](#требования)
2. [Установка](#установка)
3. [Запуск проекта](#запуск-проекта)
4. [Использование](#использование)
5. [Формат файла registered.txt](#формат-файла-registeredtxt)
6. [Структура проекта](#структура-проекта)
7. [Лицензия](#лицензия)

---

## Требования

Для работы проекта необходимо установить следующие компоненты:

- **Python 3.8 или выше**
- Установленные библиотеки:
  - wxPython
  - tensorflow
  - opencv-python
  - scikit-image
  - matplotlib
  - requests
  - gdown
  - watchdog
  - numpy

---

## Установка

1. Скачайте или клонируйте репозиторий с проектом:

   ```bash
   git clone https://github.com/RecognitionVLT.git
   cd RecognitionVLT

2. Установите необходимые зависимости:

    ```bash
    pip install -r requirements.txt

3. Убедитесь, что у вас есть доступ к интернету для загрузки моделей.

    ```bash
    pip install wxPython tensorflow opencv-python scikit-image matplotlib requests gdown watchdog numpy

---

## Запуск проекта

1. Перейдите в папку проекта:

    ```bash
    cd путь-к-проекту

2. Запустите проект:

    ```bash
    python main.py

3. После запуска откроется графическое окно приложения.

---

## Использование

1. Подготовка папки Object:

    Создайте папку Object в корневой директории проекта
    Поместите в папку Object изображения автомобилей, номера которых нужно распознать.

2. Подготовка файла registered.txt:

    Создайте файл registered.txt в корневой директории проекта
    Добавьте в файл номера автомобилей, которым разрешен въезд (по одному номеру на строку).
    Пример:

    - A111AB12
    - B222BC34
    - C333CD56

3. Распознавание:

    Приложение автоматически начнет распознавание, как только в папку Object будет добавлено новое изображение.
    Результаты распознавания будут отображаться в текстовом поле приложения:
    Если номер найден в файле registered.txt, появится сообщение: "Вход разрешен".
    Если номер не найден, появится сообщение: "Вход запрещен".
    Изображение с выделенным номером будет отображаться в интерфейсе приложения.

---

## Формат файла registered.txt

Файл registered.txt должен содержать номера автомобилей, которым разрешен въезд.
Каждый номер должен быть записан на новой строке. 
Пример:

- A111AB12
- B222BC34
- C333CD56

Убедитесь, что номера записаны в том же формате, что и результат распознавания.
Избегайте лишних пробелов и пустых строк.

---

## Структура проекта

'''
RecognitionVLT/
├── Object/ # Папка для загрузки изображений
├── registered.txt # Файл с зарегистрированными номерами
├── main.py # Основной скрипт для запуска проекта
├── model_resnet.tflite # Модель для распознавания (скачивается автоматически)
├── model1_nomer.tflite # Модель для распознавания номеров (скачивается автоматически)
├── README.md # Инструкция по использованию
└── requirements.txt # Список зависимостей (опционально)
'''

---

## Лицензия

Этот проект распространяется под лицензией MIT. Подробнее см. в файле LICENSE.

---

## Поддержка

Если у вас возникли вопросы или проблемы, создайте issue в репозитории проекта или свяжитесь с автором:
    Email: <cadetstepan13@gmail.com>
    <!-- GitHub: ваш-профиль -->
