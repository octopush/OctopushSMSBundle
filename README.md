# OctopushSMSBundle

Integrates the [Octopush SMS API client](https://github.com/octopush/sms-api-php) with Symfony.

## Installation

The recommended way to install OctopushSMSBundle is through composer:

```bash
$ composer require octopush/sms-bundle
```

Then enable it in your kernel:

```php
<?php

public function registerBundles()
{
    $bundles = [
        //...
        new Octopush\Bundle\SMSBundle\OctopushSMSBundle(),
    ];
}
```

## Configuration

```yaml
octopush_sms:
    user_login: "**********@*******"
    api_key: "****************"
```

## Usage

You can obtain Octopush SMS API client from Symfony container using:

```php
<?php

$container->get('octopush_sms.api.client');
```

## Examples

There is bundle [setup example](https://github.com/umpirsky/symfony-standard/tree/feature/octopush) using Symfony Standard Edition available.

For more information about using the client, check [Octopush SMS API](https://github.com/octopush/sms-api-php).
