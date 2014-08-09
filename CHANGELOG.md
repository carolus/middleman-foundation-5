# Changelog

## 2014-08-09

Run `foundation new middleman-foundation-5`, then merge in `middleman init middleman-foundation-5` (.gitignore and config.rb will conflict, merge by hand). Add bower_components to sprockets.append_path in config.rb.

Split `index.html` into `source/layouts/layout.erb` and `source/index.html.erb`. Change stylesheet link to "app", and javascript includes to "modernizr" (head) and "app" (end of body).

Move `humans.txt` to `source/humans.txt`

Move `robots.txt` to `source/robots.txt`

Move `scss/app.scss` to `source/stylesheets/app.scss` correct Sass path for `@import "foundation/scss/foundation";`

Delete `source/stylesheets/all.scss`

Merge `js/app.js` with `source/javascripts/all.js`. Name `source/javascripts/app.js`.

Merge `scss/_settings.scss` with `source/stylesheets/_settings.scss` correct Sass path for `@import "foundation/scss/foundation/functions";`

Create `source/javascripts/modernizr.js`

Create `source/images/.gitkeep`. Delete middleman images.
