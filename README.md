# Weather App

A small Django web application for looking up current weather by city. Enter a city on the home page to retrieve its country code, coordinates, temperature, pressure, and humidity from the OpenWeatherMap current-weather service.

## Features

- Search for a city using a simple web form.
- Display the returned weather details on the same page.
- Use Django templates with Bootstrap styling and a project stylesheet.
- Provide Django's admin route at `/admin/`.

The app makes a live request to OpenWeatherMap when a city is submitted, so weather searches require an internet connection.

## Built with

- Python
- Django 6.1.3
- SQLite (Django's configured default database)
- OpenWeatherMap Current Weather API
- Bootstrap 3

## Getting started

### Prerequisites

- Python compatible with Django 6.1.3
- pip

### Install and run

From the repository root, create and activate a virtual environment, then install Django:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install Django==6.1.3
```

Run the database migrations and start the development server:

```powershell
cd weatherapp
python manage.py migrate
python manage.py runserver
```

Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) and search for a city.

## Project layout

```text
weatherapp/
├── manage.py                 # Django management commands
├── weather/                  # Weather search view, route, and app configuration
├── weatherapp/               # Project settings and root URL configuration
├── templates/index.html      # Weather search page
└── static/                   # Stylesheet and background image
```
