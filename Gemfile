source "https://rubygems.org"

gem "github-pages", group: :jekyll_plugins

install_if -> { ENV["GITHUB_ACTIONS"] != "true" } do
    gem "webrick", "~> 1.8"
end
