# frozen_string_literal: true

source "https://rubygems.org"
gemspec

gem "jekyll", "~> 3.6.0"
gem "webrick"
gem "rexml"
# gem "jekyll"
# fixing error: bundler: failed to load command: jekyll (/usr/local/lib/ruby/gems/3.0.0/bin/jekyll)
# loads from ruby version 3.0.0 but cannot find jekyll!
# according to: https://github.com/jekyll/jekyll/issues/5423
# still does not fix it!
gem "json", "~> 2.0.2" 

# gem "jekyll" , "4.2.2" # does also not fix the problem!

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.6"
  gem "jekyll-paginate", "~> 1.1.0"
end

require 'rbconfig'
  if RbConfig::CONFIG['target_os'] =~ /darwin(1[0-3])/i
    gem 'rb-fsevent', '<= 0.9.4'
  end
