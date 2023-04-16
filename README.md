# Basic Lando D10
Basic lando/composer start

## Installation

### Create directory
`mkdir my-first-drupal10-app \
  && cd my-first-drupal10-app`
  
### Copy repo files
Copy .lando and composer.json files into directory

### Initiate lando
`lando init \
    --source cwd \
    --recipe drupal10 \
    --webroot web`
    
### Start Lando
`lando start`

### Install Drush
`lando composer require drush/drush`

### Start Drupal
`lando drush site:install --db-url=mysql://drupal10:drupal10@database/drupal10 -y`

## Next steps

Review [more advanced configuration](https://github.com/hatuhay/lando_d10)
