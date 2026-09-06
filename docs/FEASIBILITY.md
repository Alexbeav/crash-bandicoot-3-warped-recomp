# Crash Bandicoot 3: Warped release candidate

The Wave 3 campaign produced a Windows development build. This staging record does not assert a new gameplay or save/load acceptance.

The source recipe preserves the accepted game configuration and seed bytes.
Portable paths, setup wizard support, executable naming, and explicit retail BIOS policy are release changes.
Framework provenance is recorded in [the project manifest](../project-manifest.toml) and `psxrecomp/RELEASE-SOURCE.json`.
The four-platform workflow builds setup hosts and generators without retail inputs.
First-run setup, gameplay, save/load, and native Linux/macOS acceptance remain separate checks.
No quality graduation or complete-game claim is made here.
