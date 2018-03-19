# Bootstrap Patterns

[UI Patterns](https://www.drupal.org/project/ui_patterns) showcase theme based on the
[Bootstrap](https://www.drupal.org/project/bootstrap) Drupal 8 theme.
 
## Usage

Run:

```
$ composer install
```

Thanks to the integration with [Drupal Component Scaffold](https://github.com/nuvoleweb/drupal-component-scaffold)
you'll find a fully functional Drupal 8 site under ``./build``.

After that proceed with the site installation and setup:

```
$ cd build
$ drush si standard -y --db-url=mysql://username:password@host/database
$ drush en ui_patterns_library -y
$ drush then bootstrap_patterns -y
$ drush config-set system.theme default bootstrap_patterns -y
$ drush cr
```

Then visit the Patterns Overview page at `/patterns`.
