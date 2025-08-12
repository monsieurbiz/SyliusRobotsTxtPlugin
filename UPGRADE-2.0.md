# UPGRADE FROM `1.x` TO `2.0`

## Sylius compatibility

This version is compatible with Sylius 2.0.x and requires PHP 8.2 or higher.

## Configuration structure changes

The configuration files have been moved to follow Symfony 6+ conventions:

### File structure migration

```diff
- src/Resources/config/
+ config/

- src/Resources/views/
+ templates/

- src/Resources/translations/
+ translations/
```

### Bundle changes

The main bundle class now uses the `SyliusPluginTrait` and implements the `getPath()` method:

```diff
final class MonsieurBizSyliusRobotsTxtPlugin extends Bundle
{
+   use SyliusPluginTrait;
+   
+   public function getPath(): string
+   {
+       return \dirname(__DIR__);
+   }
-   
-   public function getContainerExtension(): ?ExtensionInterface
-   {
-       return new MonsieurBizSyliusRobotsTxtExtension();
-   }
}
```

### Extension alias

The DependencyInjection extension alias has been updated to follow Sylius conventions:

```diff
public function getAlias(): string
{
-   return 'monsieurbiz_robots_txt';
+   return 'monsieur_biz_sylius_robots_txt';
}
```

## Dependencies upgrade

Update your `composer.json`:

```diff
"require": {
    "monsieurbiz/sylius-settings-plugin": "^2.0",
-   "php": "^8.1",
+   "php": "^8.2",
-   "sylius/sylius": "~1.13"
+   "sylius/sylius": "~2.0"
},
```
