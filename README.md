# Puppet Pals Releases
Releases Page for Puppet Pals

## Puppet Pals Changelog
### 15 May 2022
* **[FEAT]** Global Input System
	* Select inputs will now trigger when Puppet Pals is not the active window
		* This can be toggled on a per keybind basis as well as being disabled entirely
* **[FEAT]** Added a new `config.xml` file to configure Puppet Pals. This adds a number of new settings to Puppet Pals:
	* `PreloadBackgrounds` - Loads 
	* `EnableGlobalKeybinds` - Toggles the new global input system
		* When this is set to false the keybind will not trigger unless Puppet Pals is in focus, even if global is set to true on the keybind itself.
	* `HostOnStart` - Automatically host a server when you start Puppet Pals
	* `Keybinds` - The list of keybinds
		* A keybind has 3 properties:
		* `id` - the id of the action the keybind is linked to
		* `key` - the key or combination of keys to trigger the action, with each key separated by a space
		* `global` - whether the key should listen when Puppet Pals is not in focus. Defaults to `true`
* **[FEAT]** Keybind system
	* Adds a system for configuring keybinds, as well as adding additional keybinds for actions that previously could only be triggered via the UI
		* A key combination for a keybind can currently be a maximum of 2 inputs to work correctly. This is intended to be increased in a future version.
* **[FEAT]** Prop Properties Menu
	* Replaces the old "Advanced Settings" menu that showed the settings for Under Mouth, Under All, and Jiggle Talk when you held ALT
	* Now only accessible via right clicking on a prop
	* Has the options that were previously provided by the older menu, as well as new options for Flip Horizontal, Flip Vertical, the Tint Color and a Delete button
