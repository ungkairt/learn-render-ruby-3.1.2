sudo apt install -y libpq-dev postgresql-client

ruby 3.1.2
rbenv install 3.1.2
sudo apt install ruby-railties
gem install bundler
bundle install
EDITOR="code --wait" rails credentials:edit
compile assets
RAILS_ENV=production bundle exec rake assets:precompile

test on local
RAILS_ENV=production bundle exec rails s

docker-compose up -d --build

logs
docker-compose logs web
