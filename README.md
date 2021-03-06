[![Codacy Badge](https://api.codacy.com/project/badge/Grade/58d7eedeb5694fda93ceb2240308b54e)](https://app.codacy.com/app/shem-speck/matchy?utm_source=github.com&utm_medium=referral&utm_content=sebastiaanspeck/matchy&utm_campaign=Badge_Grade_Dashboard)
[![BCH compliance](https://bettercodehub.com/edge/badge/sebastiaanspeck/sportmonks?branch=master)](https://bettercodehub.com/)

# Laravel Sportmonks Website

Laravel website that uses [Sportmonks](https://www.sportmonks.com/sports/soccer) (live)score API calls. 
Documentation for the API can be found [here](https://www.sportmonks.com/sports/soccer)

## Installation

**1-** Require the laravel-sportmonks-soccer-package via Composer.
```bash
$ composer require kirill-latish/laravel-sportmonks-soccer
```

**2-** Run Composer to install or update the new requirement.

```bash
$ composer install
```

or

```bash
$ composer update
```

**3-** Publish the configuration file

```bash
$ php artisan vendor:publish --provider="Sportmonks\SoccerAPI\SoccerAPIServiceProvider"
```

**4-** Review the configuration file and add your token in your .env file: `'api_token' => env('API_TOKEN')`

***If you don't have a API-token, you can get a free one [here](https://www.sportmonks.com/register) This should be enough to experiment with the code.***

```
config/soccerapi.php
```

**5-** Review the configuration file and change the `'without_data' => 'false' to `true`:

```
config/soccerapi.php
```

**6-** Review the configuration file and add your timezone in your .env file: `'timezone' => config('app.timezone')`

```
config/soccerapi.php
```

**7--** Copy the folder [soccerapi/laravel-sportmonks-soccer](https://github.com/sebastiaanspeck/sportmonks/blob/master/soccerapi) to `vendor/kirill-latish` and overwrite the existing folder.

## Special thanks to
[kirill-latish](https://github.com/kirill-latish/laravel-sportmonks-soccer)
