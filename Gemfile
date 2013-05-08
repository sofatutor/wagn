source 'http://rubygems.org'
#source "http://gems.github.com"

# DEFAULT
gem 'smartname',    '0.1.8'
gem 'rails',        '~> 3.2.9'
gem 'htmlentities', '~> 4.3'
gem 'uuid',         '~> 2.3'
gem 'paperclip',    '~> 2.8'
gem 'rmagick',      '~> 2.13'
gem "recaptcha",    "~> 0.3"
gem 'xmlscan',      '~> 0.3'
gem "rubyzip",      "~> 0.9" # only required in module.  should be separated out.
gem "airbrake",     "~> 3.1"
gem 'heroku'
gem 'pg'

# DATABASE

group :mysql do
  gem "mysql2", "~> 0.3"
end

gem 'dalli', :group => :memcache

group :test, :development do
  gem 'rspec-rails', "~> 2.6"                  # behavior-driven-development suite
  gem 'rails-dev-tweaks', '~> 0.6'             # dramatic speeds up asset loading, among other tweaks
end
