## Setup

```bash
$ cp .env.example .env
$ docker-compose up -d
$ docker-compose exec app bash
# Login to the container
$ composer install
$ php artisan migrate
$ php artisan db:seed
$ npm install
$ npm run dev
# Access localhost:8010
```
