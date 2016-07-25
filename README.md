
## The goal

Provide a smooth upgrade path for Linux desktop apps, just like on [Windows](https://github.com/Squirrel/Squirrel.Windows)
and [macOS](https://github.com/Squirrel/Squirrel.Mac).

## The plan

  * Ship a static execurable (use golang)
  * Use [.xz for full packages](https://github.com/danielrh/go-xz)
  * Use [wharf](https://itch.io/docs/wharf/) patches for diff packages (if [butler](https://itch.io/docs/wharf/) is available, app says where)
  * Mimic [Update.exe](https://github.com/electron/electron/blob/64ae5cf5a1d30158a79c386abe3bf3f5f0dcdc82/lib/browser/api/auto-updater/squirrel-update-win.js) CLI interface
  * Ship it :squirrel:
  * Contact other projects and consider renaming to something official
  (name will remain 'Marmot' as long as it's vaporware)