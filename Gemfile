source 'https://rubygems.org'

gemspec

gem 'minitest', '< 7'
gem 'mocha', :require => false
gem 'rake', '< 14'
gem 'json', :platform => :ruby_18

if RUBY_VERSION >= '2.6'
  group :release, optional: true do
    gem 'faraday-retry', '~> 2.1', require: false
    gem 'github_changelog_generator', '~> 1.16.4', require: false
  end
end
