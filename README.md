### Hexlet tests and linter status:
[![Actions Status](https://github.com/forward32/devops-for-programmers-project-74/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/forward32/devops-for-programmers-project-74/actions)

### Build github action status:
[![Actions Status](https://github.com/forward32/devops-for-programmers-project-74/actions/workflows/build.yml/badge.svg)](https://github.com/forward32/devops-for-programmers-project-74/actions)

## Описание
Для работы потребуется установленный `docker`, `docker-compose`. Для простоты запуска в репозитории лежит `Makefile`, для использования потребуется `make`. Никакие другие зависимости не требуются, вся работа происходит внутри контейнеров, в которых устанавливаются доп. зависимости.

## Команды запуска
- `make test` - запуск тестов локально, под капотом используется файл `docker-compose.yml`
- `make run` - запуск приложения локально, под капотом используются оба файла - `docker-compose.yml` и `docker-compose.override.yml`

## Dockerhub
Во время CI, который выполняется через Github Actions (воркфлоу описан в `.github/workflows/build.yml`) происходит сборка и пуш образа в Докархаб по пути `forward32/devops-for-programmers-project-74:latest`.
