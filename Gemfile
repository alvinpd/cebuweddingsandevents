source 'https://rubygems.org'

require 'json'
require 'open-uri'

group :development, :test do
  versions = JSON.parse(open('https://pages.github.com/versions.json').read)
  versions.delete('ruby')

  versions.each do |dep, version|
    gem dep, version
  end
end

gem 'jekyll-avatar'
