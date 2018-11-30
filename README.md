To build containers run:
docker-compose build

To start mysql:
docker-composer up

To execute composer install
docker-compose run php php /bin/composer.phar install -d tidio-test-task

To start symfony dev server:
docker-compose run --service-ports php php tidio-test-task/bin/console server:run 0.0.0.0:8000

To execute any other symfony command
docker-compose run --service-ports php php tidio-test-task/bin/console COMMAND_NAME