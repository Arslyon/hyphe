# Hyphe corpus's web pages text indexation


## develop environment

### use docker for the rest of hyphe

```bash
cd hyphe
docker-compose -f ./docker-compose-text-indexation-dev.yml  up
```

### prepare deps

```bash
pyenv virtualenv 3.7.6 hyphe_text_indexation
pyenv activate hyphe_text_indexation
bash install_deps.sh
```

### outside docker usage

```bash
$ python text_indexation.py --help
usage: text_indexation.py [-h] [--batch-size BATCH_SIZE]
                          [--nb-indexation-workers NB_INDEXATION_WORKERS]
                          [--delete-index] [--reset-mongo]

optional arguments:
  -h, --help            show this help message and exit
  --batch-size BATCH_SIZE
  --nb-indexation-workers NB_INDEXATION_WORKERS
  --delete-index
  --reset-mongo
  ```