source "https://rubygems.org"

# Jekyll
gem "jekyll", "~> 4.3.0"

# Plugins
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-sitemap", "~> 1.4"
  gem "jekyll-seo-tag", "~> 2.8"
  gem "jekyll-paginate", "~> 1.1"
  gem "jekyll-archives", "~> 2.2"
  gem "jekyll-sass-converter", "~> 3.0"
  gem "kramdown-parser-gfm", "~> 1.1"
end

# Windows support
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Development
group :development do
  gem "jekyll-admin", "~> 0.11"
  gem "html-proofer", "~> 5.0"
end
