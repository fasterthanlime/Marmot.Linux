
## The goal

Provide a smooth upgrade path for Linux desktop apps, just like on [Windows](https://github.com/Squirrel/Squirrel.Windows)
and [macOS](https://github.com/Squirrel/Squirrel.Mac).

## The plan

  * Ship a static executable (use golang)
  * Use [.xz for full packages](https://github.com/fasterthanlime/go-xz)
  * Create cgo wrapper around [Pickle](https://github.com/electron/node-chromium-pickle/tree/master/src) for asar diffing
  * Use [wharf](https://itch.io/docs/wharf/) patches for diff packages (if [butler](https://itch.io/docs/wharf/) is available, app says where)
  * Mimic [Update.exe](https://github.com/electron/electron/blob/64ae5cf5a1d30158a79c386abe3bf3f5f0dcdc82/lib/browser/api/auto-updater/squirrel-update-win.js) CLI interface
  * Ship it :squirrel:
  * Contact other projects and consider renaming to something official
  (name will remain 'Marmot' as long as it's vaporware)

## The progress so far

26-07-2016: Adopted the `go-xz` project, cleaned up its interface, added it to Travis CI:

