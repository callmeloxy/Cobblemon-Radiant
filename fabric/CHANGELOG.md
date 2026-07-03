# Changelog

## 1.0.2

### Summary

Minor visual compatibility update improving how the Radiant label is displayed in Cobblemon interfaces.

### Fixed

* Fixed the position of the `Radiant` text in the PC interface
* Fixed the `Radiant` label so it is now placed in the top-right corner of the Pokémon panel, below the male or female symbol
* Fixed a potential overlap with text added by some Pokémon size-related mods

### Improved

* Improved readability of the Radiant status in the PC
* Improved label placement while keeping the already validated vertical position unchanged
* No changes were made to gameplay, Radiant bonuses, particles, or commands

## 1.0.1

### Summary

This update improves the visual rendering of Radiant particles with a cleaner star texture and no unwanted halo.

### Improved

* Improved the Radiant particle texture with a cleaner redesign
* Improved Radiant stars with a cleaner transparent background
* Improved particle rendering by removing the unwanted visual halo around the stars
* Improved in-game readability with sharper and cleaner particle visuals
* Kept the purple Radiant style while making the final rendering cleaner

### Notes

* This update is mainly a visual polish release
* No gameplay changes were made

## 1.0.0

### Summary

Initial release of **CobblemonRadiants**, a Fabric / Cobblemon mod that adds a **Radiant** variant for shiny Pokémon.

A Radiant Pokémon is designed as a rarer shiny with its own visual identity, a small quality bonus, and configurable admin / testing tools.

### Added

* Added the **Radiant** variant for shiny Pokémon
* Added a configurable chance for a shiny Pokémon to become Radiant
* Added the `radiant` aspect to affected Pokémon
* Added a visual effect with purple stars around Radiant Pokémon
* Added a configurable custom sound for Radiant alerts
* Added a configurable built-in alert when a Radiant Pokémon appears
* Added compatibility with CSAR so built-in alerts can be disabled automatically when CSAR is installed
* Added a **Radiant** UI badge visible in the Pokémon summary and in the PC
* Added a Radiant icon displayed next to the Pokémon in addition to the shiny icon
* Added a configurable Radiant bonus:

  * 1 guaranteed perfect IV by default
  * small configurable EV bonus
  * bonus applied only once
  * option to prevent stacking with Alpha Pokémon
* Added a default config file in the mod resources
* Added commands:

  * `/radiant status` to display mod status
  * `/radiant reload` to reload the configuration
  * `/radiant debug make-nearest-radiant` to turn the nearest Pokémon into a Radiant
  * `/radiant debug spawn-radiant <pokemon> [level]` to spawn a Radiant Pokémon in the world
  * `/radiant debug test-alert` to test the Radiant alert
  * `/giveradiant <pokemon> [level]` to give yourself a Radiant Pokémon
  * `/giveradiantother <player> <pokemon> [level]` to give a Radiant Pokémon to another player
* Added configuration options for:

  * enabling or disabling the Radiant system
  * controlling the Radiant chance from shiny Pokémon
  * Radiant visual effects
  * alerts and sounds
  * IV / EV bonuses for Radiant Pokémon
  * CSAR compatibility
* Added config generation in `config/CobblemonRadiants/cobblemonradiants.json`

### Improved

* Improved Radiant persistence so Radiant Pokémon keep their state after disconnecting and reconnecting
* Improved compatibility with Cobblemon shiny behavior
* Improved give commands so the Pokémon is added to the party, or to the PC if the party is full
* Improved UI readability so the Radiant badge does not replace the shiny icon and both remain visible

### Notes

* A Radiant Pokémon is intended to be a rarer shiny, not a boss form
* The Radiant bonus is intentionally light so hunting remains rewarding without breaking balance
* Texts are translatable in French and English
