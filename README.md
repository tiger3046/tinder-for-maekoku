# tinder-for-maekoku

## 環境構築
1. `git@github.com:araki-shogo/tinder-for-maekoku.git`
2. `cd Tinder-for-maekoku`
3. `docker-compose up -d --build`
4. `docker compose exec app bash`
5. `composer install`
6. `cp .env.example .env`
7. `php artisan key:generate`
8. `php artisan storage:link`
9. `chmod -R 777 storage bootstrap/cache`
10. `php artisan migrate`

### Dockerを立ち上げる
1.`docker-compose up -d`
2.`docker-compose ps` => statusがすべてUpになっていればOK

### Dockerを落とす
`docker-compose down`

### Dockerのイメージを全て削除
`docker-compose down -rmi all`

### Tips
https://qiita.com/Usuyuki/items/b235a23d516a8d6dedc6

https://qiita.com/fumi_042/items/7d1c14e335ab1c226e0f

