[![Four Kitchens](https://img.shields.io/badge/4K-Four%20Kitchens-35AA4E.svg)](https://fourkitchens.com/)

# Macchiato: Pattern Lab + Drupal 8

Component-driven prototyping tool using [Pattern Lab v2](http://patternlab.io/) automated via Gulp/NPM. Also serves as a starterkit Drupal 8 theme.

## Requirements

  1. [Node (we recommend NVM)](https://github.com/creationix/nvm)
  2. [Gulp](http://gulpjs.com/)
  3. [Composer](https://getcomposer.org/)
  4. Optional: [Yarn](https://github.com/yarnpkg/yarn)

## Quickstart (Macchiato Standalone)

  1. `composer create-project fourkitchens/macchiato --stability dev --no-interaction macchiato`
  2. `cd macchiato`
  3. `npm install` or `yarn install`

## Drupal-specific installation

### In a Composer-based Drupal install (recommended)

  1. `composer require fourkitchens/macchiato`
  2. `cd web/themes/contrib/macchiato/`
  3. `npm install` or `yarn install`
  4. Optional (but recommended): Create "child" theme `drush macchiato "Theme Name"` (run `drush help macchiato` for available options)
  5. Enable the components and unified twig extensions modules `drush en -y components unified_twig_ext`
  6. Enable the theme in Drupal

If you're not using a Composer-based Drupal install (e.g. tarball download from drupal.org) installation [instructions can be found on the Wiki](https://github.com/fourkitchens/macchiato/wiki/Installation).

## Starting Pattern Lab and watch task

The `start` command spins up a local server, compiles everything (runs all required gulp tasks), and watches for changes.

  1. `npm start` or `yarn start`

  ---

## Highlighted Features

<table><tbody>
<tr><td>Lightweight</td><td>✔</td><td>Macchiato is focused on being as lightweight as possible.</td></tr>
<tr><td>SVG sprite support </td><td><strong>✔</strong></td><td>Automated support for creating SVG sprites mixins/classes.</td></tr>
<tr><td>Stock Drupal templates </td><td><strong>✔</strong></td><td>Templates from Stable theme - see /templates directory</td></tr>
<tr><td>Stock Components </td><td><strong>✔</strong></td><td>with Drupal support built-in (https://github.com/fourkitchens/macchiato#macchiatos-built-in-components-with-drupal-support)</td></tr>
<tr><td>Performance Testing </td><td><strong>✔</strong></td><td>Support for testing via Google PageSpeed Insights and WebPageTest.org (https://github.com/fourkitchens/macchiato/wiki/Gulp-Config#performance-testing)</td></tr>
<tr><td>Automated Github Deployment </td><td><strong>✔</strong></td><td>Deploy your Pattern Lab instance as a Github page (https://github.com/fourkitchens/macchiato/wiki/Gulp-Config#deployment)</td></tr>
</tbody></table>

<h3 id="components">Macchiato's Built in Components with Drupal support</h3>
Forms, tables, video, accordion, cards, breadcrumbs, tabs, pager, status messages, grid

View a [demo of these default Macchiato components](https://fourkitchens.github.io/macchiato/pattern-lab/public/).

## Documentation
Documentation is currently provided in [the Wiki](https://github.com/fourkitchens/macchiato/wiki). Here are a few basic links:

#### General Orientation

See [Orientation](https://github.com/fourkitchens/macchiato/wiki/Orientation)

#### For Designers (Prototyping)

See [Designers](https://github.com/fourkitchens/macchiato/wiki/For-Designers)

#### For Drupal 8 Developers

See [Drupal Components](https://github.com/fourkitchens/macchiato/wiki/Drupal-Components)

#### Gulp Configuration

See [Gulp Config](https://github.com/fourkitchens/macchiato/wiki/Gulp-Config)
