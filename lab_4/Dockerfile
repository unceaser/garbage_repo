FROM python:3.7-slim

<<<<<<< HEAD
LABEL author="Stasyan"
LABEL version=1.0

# оновлюємо систему
RUN apt-get update && apt-get upgrade -y

# Встановлюємо потрібні пакети
RUN apt-get install git -y && pip install pipenv

# Створюємо робочу папку
WORKDIR /lab

# Завантажуємо файли з Git
RUN git clone https://github.com/nukedope/garbage_repo.git

# Створюємо остаточну робочу папку з Веб-сайтом та копіюємо туди файли
WORKDIR /app
RUN cp -r /lab/garbage_repo/lab_3/* .

# Інсталюємо всі залежності
RUN pipenv install

#
EXPOSE 8000

# Це команда яка виконається при створенні контейнера
ENTRYPOINT ["pipenv", "run", "python", "manage.py", "runserver", "0.0.0.0:8000"]
=======


LABEL author="Stasyan"

LABEL version=1.0



# оновлюємо систему

RUN apt-get update && apt-get upgrade -y



# Встановлюємо потрібні пакети

RUN apt-get install git -y && pip install pipenv



# Створюємо робочу папку

WORKDIR /lab



# Завантажуємо файли з Git

RUN git clone https://github.com/nukedope/garbage_repo.git



# Створюємо остаточну робочу папку з Веб-сайтом та копіюємо туди файли

WORKDIR /app

RUN cp -r /lab/devops_course/lab_3/* .



# Інсталюємо всі залежності

RUN pipenv install



#

EXPOSE 8000



# Це команда яка виконається при створенні контейнера

ENTRYPOINT ["pipenv", "run", "python", "manage.py", "runserver", "0.0.0.0:8000"]


>>>>>>> e2c620ab41c8b45602ff57a8ec0b6f8c40ff06cd
