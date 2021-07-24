# frozen_string_literal: true

source "https://rubygems.org"

gem "jekyll", "~> 4.2.0"

gem "webrick"
gem 'execjs'

# If you have any plugins, put them here!
group :jekyll_plugins do
  gem "jekyll-seo-tag"
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-datapage-generator", "~> 1.3.0"
  gem "jekyll-last-modified-at"
  gem 'jekyll-minifier'
  gem 'jekyll-optional-front-matter'
  gem 'jekyll-paginate-v2'
  gem 'jekyll-redirect-from'
  gem 'jekyll-sitemap'
  gem 'jekyll-titles-from-headings'
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]
