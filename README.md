# [Jinja Template](https://appseed.us/jinja-template) Black Dashboard PRO

> Template Theme provided by [AppSeed](https://appseed.us) - Features:

- UI Kit: **Black Dashboard PRO** by **Creative-Tim**
- Render Engine: Flask / [Jinja2](https://jinja.palletsprojects.com/)
- **Commercial License**: [Personal](https://github.com/app-generator/license-personal) / [Developer](https://github.com/app-generator/license-developer)
- 24/7 Live Support via [Discord](https://discord.gg/fZC6hup).

<br />

> Links

- [Jinja Black Dashboard PRO - DEMO](https://jinja-black-dashboard-pro.appseed-srv1.com) - starter in action
- More [Jinja Templates](https://appseed.us/jinja-template) provided by AppSeed

<br />

## Black Dashboard PRO

Black Dashboard PRO is a beautiful Bootstrap 4 Admin Dashboard that comes in 2 versions: Dark and Light Mode. 
If you are looking for a tool to manage and visualize data about your business, this dashboard is the thing for you. It combines colors that are easy on the eye, spacious cards, beautiful typography, and graphics.

> Links

- [Black Dashboard PRO](https://themes.getbootstrap.com/product/black-dashboard-pro-premium-bootstrap-4-admin/) - product page
- [Black Dashboard PRO Docs](https://demos.creative-tim.com/marketplace/black-dashboard-pro/docs/1.0/getting-started/introduction)

<br />

![Jinja2 Theme - Black Dashboard PRO - Template project provided by AppSeed.](https://raw.githubusercontent.com/app-generator/theme-jinja2-black-dashboard-pro/master/media/theme-jinja2-black-dashboard-pro-screen.png)

<br />

## Build from sources

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/priv-jinja-black-dashboard-pro.git
$ cd priv-jinja-black-dashboard-pro
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ # Install requirements
$ pip3 install -r requirements.txt
$
$ # Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=run.py
$ (Windows) set FLASK_APP=run.py
$ (Powershell) $env:FLASK_APP = ".\run.py"
$
$ # Set up the DEBUG environment
$ # (Unix/Mac) export FLASK_ENV=development
$ # (Windows) set FLASK_ENV=development
$ # (Powershell) $env:FLASK_ENV = "development"
$
$ # Run the Jinja Template
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the UI in browser: http://127.0.0.1:5000/
```

<br />

## Code-base structure

The project has a simple structure, represented as bellow:

```bash
< PROJECT ROOT >
   |
   |-- app/__init__.py
   |-- app/
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/
   |    |    |
   |    |    |-- includes/                 # Page chunks, components
   |    |    |    |
   |    |    |    |-- navigation.html      # Top bar
   |    |    |    |-- sidebar.html         # Left sidebar
   |    |    |    |-- scripts.html         # JS scripts common to all pages
   |    |    |    |-- footer.html          # The common footer
   |    |    |
   |    |    |-- layouts/                  # App Layouts (the master pages)
   |    |    |    |
   |    |    |    |-- base.html            # Used by common pages like index, UI
   |    |    |    |-- base-fullscreen.html # Used by auth pages (login, register)
   |    |    |
   |    |  index.html                      # The default page
   |    |  login.html                      # Auth Login Page
   |    |  register.html                   # Auth Registration Page
   |    |  page-404.html                   # Error 404 page (page not found)
   |    |  page-500.html                   # Error 500 page (server error)
   |    |    *.html                        # All other pages provided by the UI Kit
   |
   |-- requirements.txt
   |
   |-- run.py
   |
   |-- ************************************************************************
```

<br />

## Deployment

The project comes with a basic configuration for [Docker](https://www.docker.com/), [Gunicorn](https://gunicorn.org/), and [Waitress](https://docs.pylonsproject.org/projects/waitress/en/stable/).

<br />

### [Docker](https://www.docker.com/) execution
---

The steps to start the template using Docker:

> Get the code

```bash
$ git clone https://github.com/app-generator/priv-jinja-black-dashboard-pro.git
$ cd priv-jinja-black-dashboard-pro
```

> Start the app in Docker

```bash
$ sudo docker-compose pull && sudo docker-compose build && sudo docker-compose up -d
```

Visit `http://localhost:5005` in your browser. The app should be up & running.

<br />

### [Gunicorn](https://gunicorn.org/)
---

Gunicorn 'Green Unicorn' is a Python WSGI HTTP Server for UNIX.

> Install using pip

```bash
$ pip install gunicorn
```
> Start the app using gunicorn binary

```bash
$ gunicorn --bind 0.0.0.0:8001 run:app
Serving on http://localhost:8001
```

Visit `http://localhost:8001` in your browser. The app should be up & running.

<br />

### [Waitress](https://docs.pylonsproject.org/projects/waitress/en/stable/)
---

Waitress (Gunicorn equivalent for Windows) is meant to be a production-quality pure-Python WSGI server with very acceptable performance. It has no dependencies except ones that live in the Python standard library.

> Install using pip

```bash
$ pip install waitress
```
> Start the app using [waitress-serve](https://docs.pylonsproject.org/projects/waitress/en/stable/runner.html)

```bash
$ waitress-serve --port=8001 run:app
Serving on http://localhost:8001
```

Visit `http://localhost:8001` in your browser. The app should be up & running.

<br />

## Credits & Links

- [Flask Framework](https://www.palletsprojects.com/p/flask/) - The official website

<br />

---
[Jinja Template](https://appseed.us/jinja-template) Black Dashboard PRO - Provided by **AppSeed** [App Generator](https://appseed.us/app-generator).
