
# Сервис прогноза погоды

Это сервис прогноза погоды, состоящий из веб-приложения. Он позволяет пользователям:
1. Получать прогнозы погоды для определённых городов, маршрутов и интервалов.
2. Использовать веб-интерфейс для визуализации погодных данных с помощью интерактивных графиков.

## Компоненты

- **Веб-сервер**: Сервис на базе Flask и Dash, который отображает прогнозы погоды с помощью графиков Plotly.

### Используемые технологии

- **Flask** и **Dash** для веб-сервера и визуализации данных.
- **Plotly** для создания графиков.
- **dotenv** для загрузки переменных окружения.

## Предварительные требования

1. **Python версии 3.10 или выше** рекомендуется для стабильной работы.
2. **Зависимости**: Установите необходимые библиотеки с помощью команд, приведённых ниже.

## Установка

1. **Склонируйте репозиторий**:
   ```bash
   git clone https://github.com/effect707/CU-Project3.git
   ```

2. **Создайте виртуальное окружение**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # Для Windows используйте `venv\Scripts\activate`
   ```

3. **Установите зависимости по отдельности**:

   **requirements.txt** — файл со всеми библиотеками:
     ```bash
     pip install -r requirements.txt
     ```

4. **Создайте файл `.env`** в корневой директории проекта и добавьте следующие переменные:

   ```plaintext
   ACCUWEATHER_TOKEN=your_accuweather_api_token
   WEATHER_API_TOKEN=your_weatherapi_token
   ```

### Описание переменных окружения:

- `ACCUWEATHER_TOKEN`: Токен для AccuWeather API, предоставляющий прогнозы погоды.
- `WEATHER_API_TOKEN`: Токен для WeatherAPI, используемый для альтернативных данных о погоде.

## Запуск проекта

**Убедитесь, что файл `.env` находится в корневой директории и содержит все необходимые API-ключи.**

 **Запустите веб-сервер**:
   ```bash
   python app.py
   ```

   - Веб-сервер на основе Flask и Dash начнёт работать, и его можно будет открыть по адресу `http://localhost:5000`.

### Использование
  
- **Веб-интерфейс**:
  - Просматривайте почасовые, дневные и недельные прогнозы и визуализируйте данные о температуре, осадках и скорости ветра для выбранных локаций.
