InnoceadCaptchaBundle
=====================

The InnoceadCaptchaBundle adds support for a captcha in Symfony 2.1.* and later.

Features include:

- Constraints Validator
- Form type
- Flexible configuration
- Uses translations (ru, en)


Installation
------------

[Resources/doc/configuration.md](https://github.com/innocead/CaptchaBundle/blob/master/Resources/doc/installation.md)

Usage
-----

You can use the "innocead_captcha" type in your forms this way:

```php
<?php
    // ...
    $builder->add('captcha', 'innocead_captcha'); // That's all !
    // ...
```

And Constraints Validator in model:

```php
<?php

namespace ..\Model;

use Innocead\CaptchaBundle\Validator\Constraints as CaptchaAssert;

class RecoverAccount
{
    /**
     * @CaptchaAssert\Captcha
     */
    public $captcha;
}
```

Configuration
-------------
See the settings in the documentation:

[Resources/doc/configuration.md](https://github.com/innocead/CaptchaBundle/blob/master/Resources/doc/configuration.md)
    

License
-------

This bundle is under the MIT license. See the complete license in the bundle:

    Resources/meta/LICENSE