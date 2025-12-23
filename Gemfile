source "https://rubygems.org"

# Jekyll
gem "jekyll", "~> 4.3.0"

# Theme (si usas la versión instalada localmente)
# gem "jekyll-theme-hydejack", "~> 9.1"

# O usa remote theme (recomendado para GitHub Pages)
# No necesitas gem para remote_theme

# Plugins esenciales
group :jekyll_plugins do
  gem "jekyll-default-layout"
  gem "jekyll-feed"
  gem "jekyll-optional-front-matter"
  gem "jekyll-paginate"
  gem "jekyll-readme-index"
  gem "jekyll-redirect-from"
  gem "jekyll-relative-links"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  gem "jekyll-titles-from-headings"
  gem "jekyll-include-cache"
end

# Windows y JRuby no incluyen archivos zoneinfo, así que incluimos la gem tzinfo-data
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster para watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# kramdown v2 ships without the gfm parser by default
gem "kramdown-parser-gfm"

# webrick para Jekyll 4
gem "webrick", "~> 1.7"
