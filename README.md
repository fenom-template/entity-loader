Custom tag and modifier loader for Fenom
=======

# Install

Use composer:
```json
{  
    "require": {
        "fenom/entity-loader": "1.*"
    }
}
```

# Setup

Add trait into your Fenom class:

```php

class MyFenom extends Fenom {
    use Fenom\EntityLoaderTrait;
}
```

# Use

```php

$fenom->addModifierLoader(function ($modifier_name, Fenom\Template $tpl) {});
$fenom->addTagLoader(function ($tag_name, Fenom\Template $tpl) {});
```

