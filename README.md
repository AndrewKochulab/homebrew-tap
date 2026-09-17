# AndrewKochulab's Homebrew tap

```sh
brew install andrewkochulab/tap/sim-mirror
```

| Formula | What it is |
| --- | --- |
| [sim-mirror](Formula/sim-mirror.rb) | [SimMirror](https://github.com/AndrewKochulab/sim-mirror): mirror and drive the iOS Simulator from AI agents and the browser |

SimMirror is built from its PyPI release, so the first install compiles a few Python extensions and takes a few
minutes. Driving a simulator needs Xcode; touching its screen needs idb_companion
(`brew install facebook/fb/idb-companion`). Then run `sim-mirror doctor`.

## Updates

[bump.yml](.github/workflows/bump.yml) runs every day. When PyPI has a newer SimMirror that has been out for at least a
day, it updates the formula's URL, checksum and Python resources, builds and tests it on macOS, and commits it. To run
it now, start the workflow by hand.

[tests.yml](.github/workflows/tests.yml) checks every pull request and push with `brew test-bot`.
