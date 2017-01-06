MYSQL - change database name, username and password if there is one or delete field

development:
  adapter: postgresql
  encoding: utf8
  reconnect: false
  host: localhost
  database: ???_development
  pool: 5
  username: deploy
  password: katalyst

test:
  adapter: postgresql
  encoding: utf8
  reconnect: false
  host: localhost
  database: ???_test
  pool: 5
  username: deploy
  password: katalyst

production:
  adapter: postgresql
  encoding: utf8
  reconnect: false
  host: localhost
  database: ???_development
  pool: 5
  username: deploy
  password: katalyst


OR

default: &default
  adapter: postgresql
  encoding: utf8
  reconnect: false
  host: localhost
  database: ???_development
  pool: 5
  username: deploy
  password: katalyst

development:
  <<: *default
  database: ???_development

test:
  <<: *default
  database: ???_test

production:
  <<: *default
  database: ???_development
