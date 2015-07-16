source 'https://rubygems.org'

group :test do
  # Pin rspec on Ruby 1.8.7
  # https://github.com/rspec/rspec-core/issues/1864
  gem 'rspec', '< 3.2.0', {"platforms"=>["ruby_18"]}

  # Rake 10.2.0+ requires Ruby >= 1.9
  gem 'rake', '< 10.2.0' if RUBY_VERSION < '1.9.0'
  gem 'puppet', ENV['PUPPET_VERSION'] || '~> 3.0.1'
  gem 'puppet-lint'
  gem 'rspec-puppet', :git => 'https://github.com/rodjek/rspec-puppet.git'
  gem 'puppet-syntax'
  gem 'puppetlabs_spec_helper'
end

group :development do
  gem 'travis'
  gem 'travis-lint'
  gem 'beaker'
  gem 'beaker-rspec'
  gem 'vagrant-wrapper'
  gem 'puppet-blacksmith'
  gem 'guard-rake'
  gem 'serverspec'
end
