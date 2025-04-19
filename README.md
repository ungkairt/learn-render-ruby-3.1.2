compile assets
RAILS_ENV=production bundle exec rake assets:precompile

test on local
RAILS_ENV=production bundle exec rails s

docker-compose up -d --build

logs
docker-compose logs web
