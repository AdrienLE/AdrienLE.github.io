source "https://rubygems.org"

# Keep the GitHub Pages-compatible Jekyll series without installing its unused
# theme/import plugins (including the old rubyzip dependency).
gem "jekyll", "~> 4.4.1"
gem "kramdown-parser-gfm", "~> 1.1"
# Jekyll's dependencies use libraries no longer bundled by default with Ruby 3.4.
gem "base64", "~> 0.3"
gem "bigdecimal", "~> 3.3"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"
  gem "jekyll-paginate", "~> 1.1"
  gem "jekyll-redirect-from", "~> 0.16"
  gem "jekyll-sitemap", "~> 1.4"
end

group :development do
  gem "bundler-audit", "~> 0.9", require: false
end
