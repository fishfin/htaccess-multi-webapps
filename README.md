# htaccess-multi-webapps
Hosting multiple WebApps from same DocRoot, keeping one WebApp the default

Assuming "htdocs" is document root:
```
+ file_system
  |_ [D] htdocs
      |_ .htaccess                      <= * see notes
      |_ [D] main_web_app_like_drupal
      |   |_ [D] config
      |   |_ [D] drush
      |   |_ [D] scripts
      |   |_ [D] web                    <= this is the main drupal user-facing interface
      |   |_ [D] vendor
      |   |_ .env
      |   |_ .gitattributes
      |   |_ .gitignore
      |   |_ .htaccess                  <= * see notes
      |   |_ .travis.yml
      |   |_ composer.json
      |   |_ composer.lock
      |   |_ LICENSE
      |   |_ load.environment.php
      |   |_ phpunit.xml.dist
      |   |_ README.md
      |_ [D] other_web_app
```
