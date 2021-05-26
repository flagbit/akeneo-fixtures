# akeneo-fixtures
Akeneo minimal fixture with jobs, locale de_DE and currency EUR

## Installation
Add the repository to you `composer.json`
```
    "repositories": [
        {
            "type": "git",
            "url": "https://github.com/mbraeuner/akeneo-fixtures"
        }
    ],
```
<br>

#### Require into local instance:

```composer req mbraeuner/akeneo-fixtures```

#### Require into Akeneo 5 docker setup:

```docker-compose run -u www-data --rm fpm composer req mbraeuner/akeneo-fixtures```

## Setup

### Minimal configuration
- Channels: ercommerce
- Locales: de_DE
- Currencies: EUR
- Import jobs 
- Export Jobs

#### Local installation:

```bin/console pim:installer:db --catalog vendor/mbraeuner/akeneo-fixtures/fixtures/minimal-jobs-de```

#### Installation into Akeneo 5 docker setup:

```docker-compose run -u www-data --rm fpm bin/console pim:installer:db --catalog vendor/mbraeuner/akeneo-fixtures/fixtures/minimal-jobs-de```
