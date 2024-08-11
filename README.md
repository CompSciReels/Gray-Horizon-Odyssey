# Gray Horizon Odyssey
#### Video Demo: https://youtu.be/tbmjVBqXAr0 

# Script 1 - AAA: Deactivate GameObject on Button Click

This Unity script deactivates a specified GameObject when the attached button is clicked. Make sure to assign the target GameObject in the objectToDeactivate field. If the button or GameObject isn't set, a warning will appear in the console.

# Script 2 - AASPOT: Enable Child Button on Parent Button Click

This Unity script disables a child button on start and re-enables it when the parent button is clicked. It automatically finds the parent button and subscribes to its onClick event. If the parent button isn't found, a warning is logged.

# Script 3 - ActivateButtonClick: Toggle Menu Visibility
This Unity script hides a menu on start and toggles its visibility when a button is clicked. The script references the entire menu object and switches its active state on each button click.

# Script 4 - AudioManager: Manage Audio Listeners
This Unity script disables all but the first AudioListener in the scene to prevent multiple audio sources from playing simultaneously. It automatically detects and disables additional listeners during the Awake phase.

# Script 5 - BackArrowButton1: Toggle UI Buttons and Child Elements

This Unity script toggles the visibility of child elements for multiple UI buttons when the back arrow button is clicked. It checks for references to global UI buttons, flips their visibility, and ensures they remain interactable. Additionally, the script manages a flipSwitch to track the toggle state.

# Script 6 - BackArrowButton2: Toggle UI Buttons with Child Elements

This Unity script toggles the visibility of all child GameObjects within specified UI buttons (Audio, Control, Credit, Option) when the back arrow button is clicked. It also updates the flipSwitch variable to track the toggle state and ensures that all buttons remain interactable.

# Script 7 - BackArrowButton3: Toggle UI Buttons with Child Elements

This Unity script toggles the visibility of all child GameObjects within specified UI buttons (Audio, Control, Credit, Option) when the back arrow button is clicked. It also updates the flipSwitch variable to track the toggle state and ensures that all buttons remain interactable.

# Script 8 - BackArrowButton4: Toggle UI Buttons and Manage Visibility

This Unity script manages the visibility of child GameObjects within specified UI buttons (Audio, Control, Credit, Option) when the back arrow button is clicked. It toggles the flipSwitch variable to track state changes and ensures all buttons remain interactable.

# Script 9 - BackgroundMusic: Manage Background Music Across Scenes

This Unity script handles background music management, ensuring that music persists across scenes and is appropriately played, paused, or stopped based on the scene index. It includes functionality to mute/unmute the audio and control playback state.

Singleton Pattern: Maintains a single instance of the background music across scenes using DontDestroyOnLoad.
Scene Management: Stops music in specific scenes (index 0 and 2) and plays it in others.
Playback Controls: Includes methods to play, pause, unpause, stop, and restart music.
Mute Functionality: Allows toggling the mute state and checks if the music is currently muted.

# Script 10 - BackgroundMusic1: Advanced Background Music Management

This Unity script manages background music with additional scene-specific controls and enhanced mute functionality. It ensures that music persists across scenes, handles playback based on scene conditions, and provides methods to control music playback and mute state.

Singleton Pattern: Maintains a single instance of the background music object using DontDestroyOnLoad.
Scene Management: Pauses, unpauses, or restarts music depending on the scene index or name (e.g., resets music when entering the "HomeScene").
Playback Controls: Includes methods to play, pause, unpause, stop, and restart music with checks for mute state.
Mute Functionality: Toggles mute state and provides status checks for whether music is muted.

