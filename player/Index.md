# Wombat Design
The Wombat player executable will be what loads and plays a project generated by Wombat Editor.

## Packages
* core
	* Description: The core package is intended to be somewhat reusable. It's job entails graphics, sound, user input, threading, and project model IO.
	* Dependencies: models
* models
	* Description: The model package handles serialization and deserialization of definitions of generated by the Editor.
* world
	* Description: Handles the overworld view and interactions with the user.
	* Dependencies: core, models