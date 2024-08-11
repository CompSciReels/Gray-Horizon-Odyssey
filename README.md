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

# Script 11 - ButtonSound: Manage Sound Effects for Buttons

This Unity script handles playing sound effects when a button is interacted with. It uses an AudioSource to play sounds and tracks whether the sound has been triggered using the soundTriggered variable.

Sound Playback: Plays a sound effect if GlobalVariables.Checkmark is true.
Sound Tracking: Updates the soundTriggered variable to track if the sound has been triggered.
Debugging: Provides debug logs to track the state of sound playback.

# Script 12 - ButtonSound2: Control Sound Effects with Additional Checks

This Unity script manages sound effects for button interactions, using an AudioSource to play sounds. It includes a soundTriggered1 variable to track if the sound has been triggered and checks a global variable to determine if the sound should play.

Sound Playback: Plays a sound effect if GlobalVariables1.newCheckmark is true.
Sound Tracking: Monitors the playback state of the sound with soundTriggered1.
Debugging: Logs messages to indicate if the sound is still playing or has been stopped.

# Script 13 - ButtonSoundPlayer: Play Button Click Sound

This Unity script plays a button click sound using an AudioSource component. The AudioClip for the button click sound is assigned through the Inspector.

Sound Playback: Plays the assigned buttonClickSound when the PlayButtonClickSound method is called.
Setup: Retrieves the AudioSource component at the start to handle playback.

# Script 14 - CameraMovement: Control Camera Movement

This Unity script controls the movement of the camera along the x-axis. It allows for camera movement with a set speed and provides methods to start or stop the movement.

Camera Movement: Moves the camera along the x-axis based on cameraSpeed when canMoveCamera is true.
Control Methods: StopCamera and ResumeCamera methods toggle the ability to move the camera.


# Script 15 - CandleStickControl: Play Sound Based on Condition

This Unity script plays a sound using an AudioSource when a specific condition from SoundManager4 is met. It checks if SoundManager4.candleStick is true and plays the sound accordingly.

Condition Check: Plays the sound if SoundManager4.candleStick is true.
Sound Playback: Uses soundPlayer1 to handle the audio playback.

# Script 16 - ChangeScene: Switch to a Specified Scene

This Unity script handles scene transitions, loading a specified scene when the MoveToHomeMenu method is called.

Scene Loading: Loads the scene specified by the sceneToLoad variable.
Debugging: Logs messages indicating the scene has been switched and loaded.

# Script 17 - ChangeScene2: Load Selector Scene

This Unity script switches to the "Selector" scene when the MoveToSelector method is called.

Scene Transition: Loads the "Selector" scene, replacing the current scene using LoadSceneMode.Single.

# Script 18 - Character: Define Character Attributes

This Unity script defines a Character class with a serializable attribute for character customization.

Character Attributes: Contains a public Sprite field named characterSprite to hold the character's visual representation.

# Script 19 - Character2: Define Character Names

This Unity script defines a Character2 class with a serializable attribute for identifying character names.

Character Attributes: Contains a public string field named characterGameObjectName for specifying the character's name.

# Script 20 - CharacterDatabase: Manage Character Data
This Unity script defines a CharacterDatabase as a ScriptableObject to manage an array of Character objects.

Character Array: Stores a list of Character objects.
Character Count: Provides a property to get the number of characters.
Get Character: Retrieves a specific Character by index.

