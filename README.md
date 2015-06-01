# Styleguided

A curated list of UI styleguides deployed to [http://kevinwuhoo.github.io/styleguided/](http://kevinwuhoo.github.io/styleguided/). Styleguides contain some combination of UI components, design patterns, icon sets, JS components, and brand guidelines.


## Todos
  * make mobile friendly
  * clean up css


## Contributing

Styleguided.io is a static site generated using [middleman](https://middlemanapp.com/), a ruby gem. You'll need ruby, rubygems, and bundler to install middleman and other dependencies. Selenium (specifically [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/downloads)) is used to screenshot the styleguides.

To suggest an additional styleguide, either open an issue with the url of the site, or create a pull request by adding the following fields in `data/styleguides.yml`:
  * name (site or company name)
  * url (https preferred)
  * color (primary brand color)
  * description (list of attributes; any combination of UI Components, JS Components, Design Patterns, and Icons)

Then run the following rake tasks to fill in remaining required fields and re-screenshot all sites:

```
bundle exec rake fill_data
bundle exec rake screenshot_guides
```
