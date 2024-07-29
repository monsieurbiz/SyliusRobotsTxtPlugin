<h1 align="center">Sylius Robots TXT</h1>

[![Robots TXT Plugin license](https://img.shields.io/github/license/monsieurbiz/SyliusRobotsTxtPlugin?public)](https://github.com/monsieurbiz/SyliusRobotsTxtPlugin/blob/master/LICENSE.txt)
[![Tests Status](https://img.shields.io/github/actions/workflow/status/monsieurbiz/SyliusRobotsTxtPlugin/tests.yaml?branch=master&logo=github)](https://github.com/monsieurbiz/SyliusRobotsTxtPlugin/actions?query=workflow%3ATests)
[![Recipe Status](https://img.shields.io/github/actions/workflow/status/monsieurbiz/SyliusRobotsTxtPlugin/recipe.yaml?branch=master&label=recipes&logo=github)](https://github.com/monsieurbiz/SyliusRobotsTxtPlugin/actions?query=workflow%3ASecurity)
[![Security Status](https://img.shields.io/github/actions/workflow/status/monsieurbiz/SyliusRobotsTxtPlugin/security.yaml?branch=master&label=security&logo=github)](https://github.com/monsieurbiz/SyliusRobotsTxtPlugin/actions?query=workflow%3ASecurity)

Manage your robots.txt from your Sylius admin pannel

## Compatibility

| Sylius Version | PHP Version |
|---|---|
| 1.12 | 8.1 - 8.2 |
| 1.13 | 8.1 - 8.2 |

## Installation

If you want to use our recipes, you can configure your composer.json by running:

```bash
composer config --no-plugins --json extra.symfony.endpoint '["https://api.github.com/repos/monsieurbiz/symfony-recipes/contents/index.json?ref=flex/master","flex://defaults"]'
```

```bash
composer require monsieurbiz/sylius-robots-txt-plugin
```

Then remove your `robots.txt` file from your public directory.
```
rm public/robots.txt
```

## Contributing

You can open an issue or a Pull Request if you want! 😘  
Thank you!
