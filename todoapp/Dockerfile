FROM python:3.9-slim-buster

WORKDIR /app

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
ENV PIP_NO_CACHE_DIR off
ENV PIP_DISABLE_PIP_VERSION_CHECK on
# ENV PIP_ROOT_USER_ACTION=ignore
# ENV PIP_DISABLE_ROOT_WARNING on

RUN apt-get update && apt-get install -y \
    build-essential \
    libpq-dev \
    && rm -rf /var/lib/apt/lists/*


COPY ./requirements.txt ./

RUN pip install -r ./requirements.txt

COPY . .

# EXPOSE 8000

# RUN python manage.py migrate
# CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
