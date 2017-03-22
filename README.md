# LCVgSSavesExample
Example project for my UE4 Plugin: LCVgsSerializedSaves

This project requires the LCVgs Serialized Saves Plugin to work!

This plugin contains:
A Blueprint function library that provides 7 Blueprint nodes to handle all the serialization, saving and loading process.
5 Simplified Nodes more for fast load and saves in one step. Let the system handle the hard part for you.
An Interface to identify the actors you want to save, as well to call the corresponding (optional) events on each one of them when saving and loading.

Features:
Serialize, save and load any number of actors in any amount of maps into and from a single save file identified by Player Name.
The use of the provided blueprint nodes will allow you to preserve all the variables and references you consider essential for those actors without worrying about complicated steps.
Choose if you want to load/save just the data for the player, the rest of the persistent actors or everything together.
The plugin handles all the internal process for serializing and saving all the actors in complex structures to later be restored. The data for each saved map is contained into a separate structure, so only the data for the current map is loaded every time, while still keeping everything in a single file.
