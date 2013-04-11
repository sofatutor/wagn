source 'http://rubygems.org'
#source "http://gems.github.com"

# DEFAULT
gem 'smartname',    '0.1.7'

gem 'rails',        '~> 3.2.9'
gem 'htmlentities', '~> 4.3'
gem 'uuid',         '~> 2.3'
gem 'paperclip',    '~> 2.8'
gem 'rmagick',      '~> 2.13'
gem "recaptcha",    "~> 0.3"

gem 'xmlscan',      '~> 0.3'
# the following two could be safely excluded on a local install (but are not known to cause problems)

gem "rubyzip",      "~> 0.9" # only required in module.  should be separated out.
gem "airbrake",     "~> 3.1"
gem 'heroku'
gem 'aws-s3', :require => 'aws/s3'
gem 'pg'

# DATABASE

# need at least one of the following

group :mysql do
  gem "mysql2", "~> 0.3"
end

gem 'dalli', :group => :memcache

group :profile do
  gem 'ruby-prof', '~>0.12.1'                              # profiling
  #gem 'test-unit' #was causing errors after cucumber runs.
end

group :test, :development do
  gem 'rspec-rails', "~> 2.6"                  # behavior-driven-development suite
  gem 'rails-dev-tweaks', '~> 0.6'             # dramatic speeds up asset loading, among other tweaks
end

group :test do
  gem 'cucumber-rails', '~> 1.3', :require=>false # feature-driven-development suite
  gem 'capybara', '~> 1.1'                     # note, selectors were breaking when we used 2.0.1
  gem 'launchy'                                # lets cucumber launch browser windows

  gem 'timecop', '=0.3.5'                      # not clear on use/need.  referred to in shared_data.rb 
  # NOTE: had weird errors with timecop 0.4.4.  would like to update when possible
  
  gem 'spork', '>=0.9'
                                               
  gem 'rr'#, '=1.0.0'

  gem 'email_spec'                             # 
  gem 'database_cleaner', '~> 0.7'             # used by cucumber for db transactions
  
  gem 'turn', "~>0.8.3", :require => false      # Pretty printed test output.  (version constraint is to avoid minitest requirement)
  gem 'minitest'
  
  #windows stuff
  gem 'win32console', '~> 1.3', :platforms => ['mingw', 'mswin']
  gem 'win32-process', '~> 0.6', :platforms => ['mingw', 'mswin']
end

group :debug do
  gem 'rdoc'
  if RUBY_VERSION =~ /^1\.9\.3-p0/
    gem 'linecache19', '~>0.5.13'
    gem 'ruby-debug-base19x', '~> 0.11.30.pre4'
  end
  if RUBY_VERSION =~ /^1\.9/
    gem 'ruby-debug19', :require => 'ruby-debug'
  else
    gem 'ruby-debug'
  end
end


# ~~~~~~~ #
# HOSTING #
# ~~~~~~~ #

#group :hosting do
#  gem 'newrelic_rpm', '>=2.14.1'
#end

