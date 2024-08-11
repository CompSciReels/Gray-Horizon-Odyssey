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

# Script 21 - CharacterDatabase2: Manage Character2 Data
This Unity script defines a CharacterDatabase2 as a ScriptableObject to manage an array of Character2 objects.

Character2 Array: Stores a list of Character2 objects.
Character Count: Provides a property to get the number of Character2 items.
Get Character: Retrieves a specific Character2 by index.

# Script 22 - CharacterManager: Handle Character Selection and Display
This Unity script manages character selection and display, allowing users to cycle through characters and persist their choice.

Character Selection: Uses CharacterDatabase to manage and display character options.
Option Navigation: Includes methods NextOption and BackOption to navigate through available characters.
Persistence: Saves and loads the selected character option using PlayerPrefs.

# Script 23 - CharacterSelector: Select and Save Character Index
This Unity script handles the selection and saving of a character index when the play button is clicked.

Character Selection: Retrieves the currently selected character from PlayerPrefs.
Slot Index Finding: Determines the index of the selected character within the CharacterDatabase.
Persistence: Saves the selected character's slot index to PlayerPrefs.

# Script 24 - EventSystemManager: Singleton for EventSystem Management
This Unity script ensures that an EventSystem exists in the scene and is managed as a singleton.

Singleton Pattern: Ensures only one instance of EventSystemManager exists.
EventSystem Creation: Creates and configures an EventSystem if none exists in the scene.
Persistence: Makes sure the EventSystemManager persists across scene loads.

# Script 25 - GameOver: Manages Game Over State
This Unity script handles the game-over state by managing UI, game mechanics, and background music.

Game Over Actions:

Displays gameOverPanel.
Stops background looping and particle effects.
Pauses the camera movement.
Pauses background music and updates high score.
Restart Functionality:

Resets obstacleTriggered and reloads the current scene.
Resumes camera movement and unpauses background music.
References:

Links to LoopingBackground, StopParticlesOnGameOver, CameraMovement, BackgroundMusic, HighScoreManager, and ScoreManager.

# Script 26 - GlobalButtonReferences: Manages Persistent Button References
This Unity script handles global references to UI buttons and ensures persistence across scenes.

Singleton Pattern:

Instance: Provides a global access point to the GlobalButtonReferences instance.
Button References:

audioButton, controlButton, creditButton, optionButton: Public fields to assign button references in the Inspector.
Persistence:

The Awake method checks if the object has the "PersistentObject" tag to prevent destruction across scene loads.
Button Recovery (Commented Out):

The RecoverButtons function is intended to find and assign button references if they are null. (Commented out in the current script.)

# Script 27 - GlobalSubstance: Global State Management
This static class maintains global state for the obstacleTriggered flag.

Purpose:

Provides a global, static variable to track if an obstacle has been triggered.
Static Field:

obstacleTriggered: A public static boolean that other scripts can access and modify.

# Script 28 - GlobalVolume: Volume Management
This static class manages global volume settings for button sounds.

Purpose:

Provides a global static property to access and modify button volume levels.
Static Property:

ButtonVolume: A public static float property that stores the volume level for button sounds.

# Script 29 - GlobalVolume1: Enhanced Volume Management
This static class manages button volume with additional functionality.

Purpose:

Provides global access to button volume settings with encapsulation and storage.
Private Field:

buttonVolume: A private static float that stores the button volume level.
Public Static Methods:

GetVolume(): Returns the current button volume level.
SetVolume(float volume): Sets the button volume level and saves it using PlayerPrefs.
Additional Features:

The SetVolume method saves the volume level to PlayerPrefs, making it persistent across sessions.

# Script 30 - HighScoreManager: Managing and Displaying High Scores
This script manages and displays the high score for a game, using Unity's PlayerPrefs for persistent storage.

Purpose:

Tracks the highest score achieved and updates the UI text accordingly.
Public Fields:

highScoreText: Reference to the UI Text component that displays the high score.
Private Fields:

highScore: Stores the current high score.
scoreManager: Reference to the ScoreManager script.
Start Method:

Initializes highScore from PlayerPrefs.
Updates the high score display.
Finds and references the ScoreManager script.
Public Methods:

UpdateHighScore(float currentScore): Updates the high score if the current score exceeds it. Saves the new high score to PlayerPrefs.
Private Methods:

UpdateHighScoreText(): Formats and updates the high score text to a 5-digit string.



