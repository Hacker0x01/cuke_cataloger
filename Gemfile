source 'http://rubygems.org'

# Specify your gem's dependencies in cuke_cataloger.gemspec
gemspec

# The Coveralls gem can't handle more recent versions of the SimpleCov gem
gem 'simplecov', '<= 0.16.1'

# cuke_cataloger can play with pretty much any version of these but they all play differently with Ruby
if RUBY_VERSION =~ /^1\.8/
  gem 'cucumber', '< 1.3.0'
  gem 'gherkin', '< 2.12.0'
  gem 'mime-types', '< 2.0' # The 'mime-types' gem requires Ruby 1.9.x on/after this version
  gem 'rainbow', '< 2.0' # Ruby 1.8.x support dropped after this version
  gem 'rake', '< 11.0' # Rake dropped 1.8.x support after this version
elsif RUBY_VERSION =~ /^1\./
  gem 'cucumber', '< 2.0.0'
  gem 'mime-types', '< 3.0.0' # The 'mime-types' gem requires Ruby 2.x on/after this version
  gem 'rainbow', '< 3.0' # The 'rainbow' gem requires Ruby 2.x on/after this version
  gem 'rake', '< 12.3.0' # The 'rake' gem requires Ruby 2.x on/after this version
  gem 'rest-client', '< 2.0' # The 'rainbow' gem requires Ruby 2.x on/after this version
else
  # TODO: Upgrade to a Cucumber 4.x once it works completely
  gem 'cucumber', '2.2.0'
  # Generally, develop against the most recent supported version of stuff
  gem 'rake', '~> 13.0'
  gem 'thor', '~> 1.0'
  gem 'cql', '~> 1.0'
  # Locking < 3 given that cuke_modeler ~> 3.0
  # requires cucumber 4 
  # https://github.com/enkessler/cuke_modeler/issues/6
  gem 'cuke_modeler', '< 3.0'
end

if RUBY_VERSION =~ /^1\./
  gem 'ffi', '< 1.9.15'  # The 'ffi' gem requires Ruby 2.x on/after this version
  gem 'tins', '< 1.7'    # The 'tins' gem requires Ruby 2.x on/after this version
  gem 'json', '< 2.0'    # The 'json' gem drops pre-Ruby 2.x support on/after this version
  gem 'simplecov-html', '< 0.11.0' # The 'simplecov-html' gem requires Ruby 2.x on/after this version
  gem 'term-ansicolor', '< 1.4' # The 'term-ansicolor' gem requires Ruby 2.x on/after this version
end


# Generally, develop against the most recent supported version of stuff
