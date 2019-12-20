# Talented

> Newest release available at: https://github.com/Siarkowy/Talented

Fork of Talented r291 by Jerry, with Action Bar Saver integration.


## Improvements

- [x] Automatically perform Action Bar Saver restore after successful Talented respec.
  ABS profile that matches Talented template name will be used.


## Installation

- Hit the `Clone or Download` button above and choose `Download ZIP`, then open the archive.
- Extract all folders under `Talented-master\` directory to your `Interface\AddOns\` location.
  You may safely overwrite your existing Talented installation.
- You should also [download](https://www.wowace.com/projects/action-bar-saver/files/350733) & install Action Bar Saver if you don't have it yet.


## Configuration

1. Make sure both Talented and Action Bar Saver are enabled in add-ons.
2. Configure Action Bar Saver to your liking.
    - Toggle missing macro recreation: `/abs macro`
    - Toggle using max spell ranks only: `/abs rank`
3. Suppose you have an already existing Talented template called "Mage Fire".
    - Arrange the action bars to your liking.
    - Save in ABS with `/abs save Mage Fire` (names must match except for character case).
4. In Talented > Options, make sure "Restore bars with ABS" is enabled.

Now whenever you go to the trainer, wipe your talents and apply the "Mage 
Fire" template from Talented, ABS will automatically restore the bars if
all talents were applied successfully.


### Multiple builds with single ABS profile

You can share ABS action bar configuration between multiple Talented builds.
When looking for a matching ABS profile, Talented template name will be
trimmed to first dash, so the following builds will all finish with automatic
`/abs restore Warlock Destro Shadow`, ignoring the Healthstone part:

- Warlock Destro Shadow - 0/2 HS
- Warlock Destro Shadow - 1/2 HS
- Warlock Destro Shadow - 2/2 HS
