## Installation

1. Download or clone this resource into your server `resources` folder.

2. Ensure the folder name is correct, for example:

```txt
resources/[vorp]/vorp_weapons
```

3. Add the resource to your `server.cfg` **after** its required dependencies:

```cfg
ensure vorp_core
ensure vorp_menu
ensure vorp_weapons
```

4. Import the included SQL file into your server database.

5. Open the configuration files and set up:

* Weapon shop locations
* Shop opening and closing hours
* Weapon prices
* Customization prices
* Camera and preview settings
* Prompt keys and interaction distances

6. Restart the resource or restart your server:

```cfg
restart vorp_weapons
```

## Requirements

This resource requires a working VORP Core installation.

Make sure the following resources are started before this one:

```cfg
ensure vorp_core
ensure vorp_menu
```


## Credits

This resource is a modified derivative project built using the following open-source resources:

* **[VORPCORE / vorp_weaponsv2](https://github.com/VORPCORE/vorp_weaponsv2)**
  Original base weapon-shop and weapon-customization code structure for VORP Core.

* **[TPZ-CORE / tpz_weapons](https://github.com/TPZ-CORE/tpz_weapons)**
  Data-binding weapon store system and related store implementation reference/code.

## Modifications and Integration

Modified, converted, and expanded by **Tucan**:

* Converted the original WarMenu-based interfaces to **`vorp_menu`**.
* Integrated and adapted the data-binding weapon-store system.
* Added weapon-customization camera handling and preview improvements.
* Added native interaction prompts and shop interaction flow.

