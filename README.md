# Components

[![Build Status](https://travis-ci.org/silbinarywolf/silverstripe-components.svg?branch=master)](https://travis-ci.org/silbinarywolf/silverstripe-components)
[![Latest Stable Version](https://poser.pugx.org/silbinarywolf/silverstripe-components/version.svg)](https://github.com/silbinarywolf/silverstripe-components/releases)
[![Latest Unstable Version](https://poser.pugx.org/silbinarywolf/silverstripe-components/v/unstable.svg)](https://packagist.org/packages/silbinarywolf/silverstripe-components)
[![Total Downloads](https://poser.pugx.org/silbinarywolf/silverstripe-components/downloads.svg)](https://packagist.org/packages/silbinarywolf/silverstripe-components)
[![License](https://poser.pugx.org/silbinarywolf/silverstripe-components/license.svg)](https://github.com/silbinarywolf/silverstripe-components/blob/master/LICENSE.md)

This module allows you to use special <:TemplateName> syntax to include templates. This allows you to pass inner HTML into a template, much like you can do in React with the children properties. Using the <:TemplateName> syntax will not automatically pass variables in the current scope like <% include %>.

```
<:MyButtonTemplate 
  icon="fa fa-icon"
  title="$Title"
>
    <span class="text">
        Look at me! Passing HTML in here!
    </span>
</:MyButtonTemplate>
```

```
<:SelfClosingTag passvariable="hey" />
```

## Composer Install

```
composer require silbinarywolf/silverstripe-components:0.4.0
```

## Requirements

* PHP 5.4+
* SilverStripe 3.6+

## Documentation

* [Quick Start](docs/en/quick-start.md)
* [Advanced Usage](docs/en/advanced-usage.md)
* [License](LICENSE.md)
* [Contributing](CONTRIBUTING.md)

## Credits

* [Cam Spiers](https://github.com/camspiers) for his [SilverStripe Compose Parser module](https://github.com/heyday/silverstripe-composeparser/). This utilizes and builds upon his work from half a decade ago!
