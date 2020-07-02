# Project title

[![Language](https://img.shields.io/badge/language-python-brightgreen?style=flat-square)](https://www.python.org/)
[![Language](https://img.shields.io/badge/language-javascript-brightgreen?style=flat-square)](https://developer.mozilla.org/uk/docs/Web/JavaScript)

Hello everyone! This is the example of REST API on **Django** and **React**.

## Table of contents

- [Project title](#project-title)
- [Motivation](#motivation)
- [Build status](#build-status)
- [Badges](#badges)
- [Tech/framework used](#techframework-used)
- [Features](#features)
- [Code Example](#code-example)
- [Installation](#installation)
- [Fast usage](#fast-usage)
- [Tests](#tests)
- [License](#license)

## Motivation

One time I just have met the book William S. Vincent "Django for APIs". So I tried do the project. Here it is!

## Build status

Here you can see build status of [continuous integration](https://en.wikipedia.org/wiki/Continuous_integration)

[![Build Status](https://travis-ci.com/mezgoodle/Todo-API.svg?branch=master)](https://travis-ci.com/mezgoodle/Todo-API)

## Badges

Other badges

[![Build Status](https://img.shields.io/badge/Theme-REST_API-brightgreen?style=flat-square)](https://www.google.com.ua/)

## Tech/framework used

**Built with**

- [Django](https://www.djangoproject.com/)
- [React](https://uk.reactjs.org/)

## Features

Show Todo-list on page.

## Code Example

- `serializers.py`

```python
from rest_framework import serializers
from .models import Todo


class TodoSerializer(serializers.ModelSerializer):
    class Meta:
        model = Todo
        fields = ('id', 'title', 'body',)

```

## Installation

1. Clone this repository

```bash
git clone https://github.com/mezgoodle/Todo-API.git
```

2. Use the package manager [pip](https://pip.pypa.io/en/stable/) to install required packages:

```bash
pip install -r requirements.txt
```

3. Move to `frontend` folder and install packages from `package.json` by package manager [npm](https://www.npmjs.com/):

```bash
cd frontend
npm i
```

## Fast usage

1. Run React server:

```bash
cd frontend
npm start
```

2. Run Django server:

```bash
cd backend
python manage.py runserver
```

3. Open in your browser `localhost:3000`.

## Tests

All tests are in `backend/todos/tests.py` and `frontend/src/App.test.js`.

## License

MIT © [mezgoodle](https://github.com/mezgoodle)
