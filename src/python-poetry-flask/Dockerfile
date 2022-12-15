FROM python:3.9

WORKDIR /app

COPY . .

RUN pip install poetry

RUN poetry install --only main

ENV FLASK_APP="app"

#ENV FLASK_DEBUG=true

ENV FLASK_RUN_HOST="0.0.0.0"

CMD ["poetry", "run", "flask", "run"]
