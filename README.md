# Away Strength

A standalone, installable bodyweight workout tracker for air squats, push-ups, and glute bridges.

- [Open Away Strength](https://lordofblackwood.github.io/away-strength/)
- [Powerlevel dashboard](https://lordofblackwood.github.io/gamify-gym/)

## Install and connect

Open Away Strength in Safari, choose Share → Add to Home Screen, and open the installed app online once to prepare it for offline workouts. In the app’s Sync tab, paste your existing Powerlevel connection code. Workouts save on your device immediately and upload encrypted summaries when the app is open online.

If moving from the original /gamify-gym/bodyweight/ installation, export its backup before removing it. Import that backup in the new installation’s Sync tab and reconnect with the same dashboard code. Use one Away Strength installation per connection.

## Progression

Each exercise and variation advances independently: 1×10 → 2×10 → 3×10 → 1×12, up to 3×20. Comfortable completion can advance or repeat; hard completion repeats; stopping early lowers the next prescription. Adjust lets you choose an easier variation or fewer starting reps. Log actual reps, including partial sets, and use rest days when needed. Daily logging does not require daily hard training.

History includes undo, backup export/import, and recovery of the data saved before an import. Bodyweight reps count toward the dashboard’s training days and appear separately from barbell strength.

## Development

Node 22 or newer. Run npm ci, then npm run dev. Run npm test and BASE_PATH=away-strength npm run build before publishing. GitHub Actions builds and deploys this repository’s main branch to its own Pages site.

The app has no build-time dependency on the dashboard repository. Compatible bodyweight validation and encrypted transport modules are included under public/shared. The relay is operated separately; connection codes and personal histories are never committed here.

See [behavior and verification](docs/behavior.md).
