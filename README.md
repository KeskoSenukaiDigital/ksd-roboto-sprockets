# Fork
This repository is a fork. You can find original here:
https://github.com/jerrysdesign/roboto-fontface-pre-css

yarnpkg.com:
https://yarnpkg.com/en/package/roboto-fontface-pre-css

# Roboto fontface

## Prerequisites
- Ruby on Rails
- Sprockets

##  How to use
First, create `app/assets/roboto.scss`:

```
$roboto-font-path: "ksd-roboto-sprockets/assets/fonts";
@import "ksd-roboto-sprockets/assets/stylesheets/roboto-fontface.scss";
```

Then, import newly created stylesheet into `app/assets/application.scss`:

```
@import "roboto";
```

Ensure your `config/application.rb` or `config/initializers/assets.rb` contain these entries:

```
config.assets.paths << Rails.root.join('node_modules')
config.assets.precompile += %w(.svg .eot .woff .ttf)
```

That is it ⚙️
