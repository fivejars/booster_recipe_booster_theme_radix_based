## Booster theme (Radix based) recipe

Sets up Booster (Radix based) theme as the default theme.

### Installation:
Add recipe repository reference to the repositories section to override "drupal_recipe/booster_theme" package:

```json
{
  "repositories": {
    "booster_theme_recipe": {
      "type": "git",
      "url": "https://github.com/fivejars/booster_recipe_booster_theme_radix_based.git",
      "only": ["drupal_recipe/booster_theme"]
    }
  }
}
```
Run composer commands:

```bash
composer require --dev drupal_recipe/booster_theme
composer unpack drupal_recipe/booster_theme
```

If the composer install ran successfully, you can enable the recipe with the following commands:

```bash
fin recipe-apply path/to/recipe/from/docroot
```

## Maintainers

Sponsored and developed by [Five Jars](https://www.drupal.org/five-jars).
