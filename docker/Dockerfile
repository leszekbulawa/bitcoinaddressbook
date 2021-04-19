FROM python:3.9

WORKDIR /app

COPY poetry.lock pyproject.toml /app/

RUN python -m pip install --upgrade pip poetry && \
    poetry config virtualenvs.create false && \
    poetry install --no-dev

COPY src/ /app/

CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8000"]