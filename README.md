# Middleman Template for Foundation 5

## Requirements

  * Ruby 1.9+
  * [Node.js](http://nodejs.org)
  * [middleman](http://middlemanapp.com/): `gem install middleman`
  * [bower](http://bower.io): `npm install bower -g`

## Quickstart

Either clone this repo for your new project:

```bash
git clone git://github.com/tehpeh/middleman-foundation-5.git my_new_project
```

or add it to the Middleman template directory and use the --template flag when creating a new project:

```bash
mkdir -p ~/.middleman
git clone git://github.com/tehpeh/middleman-foundation-5.git ~/.middleman/foundation-5
middleman init my_new_project --template=foundation-5
```

Then finish the set up with:

```bash
cd my_new_project
bundle install
bower install
```

When you're working on your project, just run the following command:

```bash
bundle exec middleman
```

## Upgrading

### Foundation

If you'd like to upgrade to a newer version of Foundation down the road just run:

```bash
bower update
```

Then compare and copy over any updates to _settings.scss:

```bash
diff source/stylesheets/_settings.scss bower_components/foundation/scss/foundation/_settings.scss
```
### Middleman

Middleman has it's own upgrade command:

```bash
bundle exec middleman upgrade
```

## License

This project uses open source software under the MIT license. See LICENSE.md for
details.
