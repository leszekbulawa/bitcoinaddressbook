# bitcoinaddressbook

# req
* docker
* docker-compose

for manual run:
* python 3.9
* poetry

# how to run
```bash
docker-compose up
```

# how to run manually
```bash
poetry init
poetry install
poetry shell
cd src
uvicorn app:app --reload
```

then navigate to http://127.0.0.1:8000/
