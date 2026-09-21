source "https://rubygems.org"

# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!

# Using plain jekyll (pinned to the version github-pages currently ships)
# instead of the "github-pages" meta-gem. That gem drags in
# github-pages-health-check -> dnsruby -> unf_ext, a C++ extension that
# fails to compile on modern macOS/Xcode and isn't needed for local preview
# or for any feature this site actually uses. This keeps local `jekyll serve`
# equivalent to GitHub Pages for everything this site relies on.
gem "jekyll", "3.9.2"

# _config.yml sets `kramdown: input: GFM`, which requires this parser.
# Normally pulled in transitively by github-pages; needs to be explicit now.
gem "kramdown-parser-gfm"

gem "wdm", "~> 0.1.0" if Gem.win_platform?

# Matches the `plugins:` list in _config.yml
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  gem "jekyll-paginate"
  gem "jekyll-redirect-from"
  gem "jekyll-gist"
  gem "hawkins"
end

gem "webrick", "~> 1.7"

# Ruby 3.4 removed several libraries from the default gems (they now must
# be declared explicitly instead of being implicitly available). These are
# used by jekyll/liquid/safe_yaml under the hood.
gem "csv"
gem "base64"
gem "bigdecimal"
gem "logger"
