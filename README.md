# docker-config

Для настройки необходимо скопировать файл .env.example  
(**cp .env.example .env**) и ипоменять конфиги на свои.
- WWW_PATH - путь к директории со всеми проектами (к конкертному проекту указать через конфиг nginx)
- DB_DIR - директория для БД, если конечной папки не будет docker сам ее создаст.

_собрать проект:_ **docker-compose build**
_запустить:_ **docker-compose up** или **docker-compose up -d** для демона
_потушить:_ **docker-compose down**
