neo4j-examples
==============

##Create Gemfile

```sh
touch Gemfile
```

##Set the source

```ruby
source 'https://rubygems.org'
```

##Add neography gem

```ruby
gem 'neography'
```

##Run bundler

```sh
bundle or bundle install
```

##neo4j Install Method 1

```sh
sudo -s
wget -O - http://debian.neo4j.org/neotechnology.gpg.key | apt-key add - 
echo 'deb http://debian.neo4j.org/repo stable/' > /etc/apt/sources.list.d/neo4j.list
apt-get update
apt-get install neo4j
neo4j start
```

##neo4j Install Method 2

create new rails project by: rails new neo4j_examples
use rakefiile and type:

```ruby
echo "require 'neography/tasks'" > Rakefile
rake neo4j:install
rake neo4j:start
```
