### Less-Rails
---
https://github.com/metaskills/less-rails

```
bundle
bundle exec appraisal install
bundle exec appraisal rake

bundle exec rake appraisal:rails40 test

rails g less:assets posts

```

```ruby
config.app_generators.stylesheet_engine :less

gem 'less-rails', '~> 4.0.0'
gem 'therubyracer'
gem 'therubyrhino'

MyProject::Application.configure do
  config.less.paths << "#{Rails.root}/lib/less/protractor/stylesheets"
  config.less.compress = true
end

@import "frameworks/bootstrap/mixins";
#leftnav { .border-radius(5px); }

Rails.application.config.less.raw.relativeUrls = false

assets-path(@relative-asset-path)
assets-path("rails.png")
assets-url(@relative-asset-path)
asset-url("rails.png")

asset-data-url("rails.png")

```

```
```

