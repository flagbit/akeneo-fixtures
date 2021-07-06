# akeneo-fixtures
Akeneo minimal fixture with jobs, locale de_DE and currency EUR

## Compatibility

This package supports the latest Akeneo PIM CE/EE stable versions:

* 5.0
* 4.0

## Installation
Add the repository to you `composer.json` if needed.
```
    "repositories": [
        {
            "type": "git",
            "url": "https://github.com/flagbit/akeneo-fixtures"
        }
    ],
```
<br>

#### Require into local instance:

```composer req flagbit/akeneo-fixtures```

#### Require into Akeneo 5 docker setup:

```docker-compose run -u www-data --rm fpm composer req flagbit/akeneo-fixtures```

## Setup

### Minimal configuration
- Channels: ecommerce
- Locales: de_DE
- Currencies: EUR
- Import jobs 
- Export Jobs



#### Local installation:
###### CE
```bin/console pim:installer:db --catalog vendor/flagbit/akeneo-fixtures/fixtures/ce-minimal-jobs-de```

###### EE
```bin/console pim:installer:db --catalog vendor/flagbit/akeneo-fixtures/fixtures/ee-minimal-jobs-de```


#### Installation into Akeneo 5 docker setup:
###### CE
```docker-compose run -u www-data --rm fpm bin/console pim:installer:db --catalog vendor/flagbit/akeneo-fixtures/fixtures/ce-minimal-jobs-de```

###### EE
```docker-compose run -u www-data --rm fpm bin/console pim:installer:db --catalog vendor/flagbit/akeneo-fixtures/fixtures/ee-minimal-jobs-de```
