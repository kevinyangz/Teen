1. make sure you have ruby install and check the version of your ruby
ruby -v
2. install rails
gem install rails
3. Make sure you have brew install
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
4.you need to install postgresql
brew install postgresql
5.clone my github branch 
https://github.com/kevinyangz/Teen.git
6.cd into Teenbuddy
7.There is problem on GemFile, you need to make sure your ruby version match the ruby version under  Teen/TeenBuddy/Gemfile
  it is in line:52, just do 'ruby -v' and modify the gemfile with your ruby version
8.then do bundle install 
bundle install 
9. If there is no error, do the migration
bin/rails db:migrate RAILS_ENV=development
10. load the pre-genearte data
rake db:setup
11.start the server
rails server
12.open http://0.0.0.0:3000/home/index
13. there are two test accounts-- click login
account name:client@ut.com
pwd:123456
or 
teenager@ut.com
123456
