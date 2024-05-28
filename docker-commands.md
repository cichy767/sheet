odpalenie kontenera z jakiegoś obrazu 

docker run --rm -it --entrypoint /bin/bash <image_name>


reset bazy

docker-compose down
docker-compose down -v


docker-compose run web poetry run python manage.py makemigrations
docker-compose run web poetry run python manage.py migrate

docker-compose run web poetry run python manage.py createsuperuser
