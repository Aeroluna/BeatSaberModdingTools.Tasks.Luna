# BeatSaberModdingTools.Tasks.Luna
A fork of [BeatSaberModdingTools.Tasks](https://github.com/Zingabopp/BeatSaberModdingTools.Tasks) with a few additions, mostly to help with setting up a project to target multiple Beat Saber versions.

* .pdb files are no longer zipped on releases. This can be reenabled using the `ZipPDB` property.
* Condition for zipping now looks for the `RELEASE` constant rather than for a configuration named `Release`.
* Added the `AppendGameVersion` property to the `GenerateManifest` task. When set to true, the generated manifest will have the game version added to the end of the plugin version, e.g. `0.0.1+1.29.1`.
* Added `Visible="False"` to `GenerateManifest` item groups to stop IDEs from throwing warnings when looking for files that don't exist.
