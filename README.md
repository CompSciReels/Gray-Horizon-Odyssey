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
  Displays gameOverPanel. | 
  Stops background looping and particle effects. | 
  Pauses the camera movement. | 
  Pauses background music and updates high score.

Restart Functionality: Resets obstacleTriggered and reloads the current scene. | Resumes camera movement and unpauses background music.

References: Links to LoopingBackground, StopParticlesOnGameOver, CameraMovement, BackgroundMusic, HighScoreManager, and ScoreManager.

# Script 26 - GlobalButtonReferences: Manages Persistent Button References
This Unity script handles global references to UI buttons and ensures persistence across scenes.

Instance: Provides a global access point to the GlobalButtonReferences instance.

Button References: audioButton, controlButton, creditButton, optionButton: Public fields to assign button references in the Inspector.

Persistence: The Awake method checks if the object has the "PersistentObject" tag to prevent destruction across scene loads.

Button Recovery (Commented Out):
The RecoverButtons function is intended to find and assign button references if they are null. (Commented out in the current script.)

# Script 27 - GlobalSubstance: Global State Management
This static class maintains global state for the obstacleTriggered flag.

Purpose: Provides a global, static variable to track if an obstacle has been triggered.

Static Field: obstacleTriggered- A public static boolean that other scripts can access and modify.

# Script 28 - GlobalVolume: Volume Management
This static class manages global volume settings for button sounds.

Purpose: Provides a global static property to access and modify button volume levels.

Static Property: ButtonVolume- A public static float property that stores the volume level for button sounds.

# Script 29 - GlobalVolume1: Enhanced Volume Management
This static class manages button volume with additional functionality.

Purpose: Provides global access to button volume settings with encapsulation and storage.

Private Field: buttonVolume- A private static float that stores the button volume level.

Public Static Methods: GetVolume()- Returns the current button volume level. | SetVolume(float volume)- Sets the button volume level and saves it using PlayerPrefs.

Additional Features: The SetVolume method saves the volume level to PlayerPrefs, making it persistent across sessions.

# Script 30 - HighScoreManager: Managing and Displaying High Scores
This script manages and displays the high score for a game, using Unity's PlayerPrefs for persistent storage.

Purpose: Tracks the highest score achieved and updates the UI text accordingly.

Public Fields: highScoreText- Reference to the UI Text component that displays the high score.

Private Fields: highScore- Stores the current high score. | scoreManager- Reference to the ScoreManager script.

Start Method: Initializes highScore from PlayerPrefs. | Updates the high score display. | Finds and references the ScoreManager script.

Public Methods: UpdateHighScore(float currentScore)- Updates the high score if the current score exceeds it and saves the new high score to PlayerPrefs.

Private Methods: UpdateHighScoreText()- Formats and updates the high score text to a 5-digit string.

# Script 31 - HomeSwitch: Handling Transitions to the Home Screen
This script manages transitions to the home screen, stopping background elements and updating the high score when certain conditions are met.

Purpose: Handles the transition and management of game elements when an obstacle is triggered.

Public Fields: homeButton- Reference to the UI Button for returning to the home screen.

Private Fields:
loopingBackground- Reference to the LoopingBackground script. | 
cameraMovement- Reference to the CameraMovement script. | 
highScoreManager- Reference to the HighScoreManager script. | 
scoreManager- Reference to the ScoreManager script.

Start Method:
Initializes references to LoopingBackground, CameraMovement, HighScoreManager, and ScoreManager scripts.

Update Method:
Checks if GlobalSubstance.obstacleTriggered is true. | 
Stops background looping. | 
Stops the camera movement. | 
Updates the high score based on the current score.

Public Methods:
Restart()- Intended to reset the state (currently commented out).

Script 32 - LoadHomeMenu: Loading the Home Menu Scene
This script provides functionality to load the "HomeMenu" scene when triggered.

Purpose: Loads the "HomeMenu" scene.

Public Methods: LoadSceneHomeMenu()- Uses SceneManager.LoadScene to load the "HomeMenu" scene.

# Script 33 - LoopingBackground: Handling Background Scrolling
This script controls the movement of a looping background texture and stops the scrolling when the game is over.

Purpose: Manages the scrolling of a background texture and stops it when the game ends.

Public Variables:
backgroundSpeed- Speed at which the background texture scrolls. | 
backgroundRenderer- Renderer component used to apply the texture.

Private Variables:
isGameOver- Flag indicating whether the game is over.

Public Methods:
StopBackgroundLooping()- Sets isGameOver to true, stopping the background movement.

Private Methods:
Update()- Continuously adjusts the mainTextureOffset of the background material to create a scrolling effect if isGameOver is false.

# Script 34 - Obstacle: Handling Collision with Player and Border
This script manages interactions between obstacles and other game objects, including the player and border.

Purpose:
Handles the destruction of obstacles upon collision with specific tags and triggers game state changes when colliding with the player.

Public Variables:
scoreValue- Score awarded for an obstacle; currently unused in this script.

Private Variables:
player- Reference to the player game object.

Private Methods:
Start()- Finds and assigns the player game object at the start of the game. | 
OnTriggerEnter2D(Collider2D collision)- Detects collisions with other game objects:

If colliding with "Border": Destroys the obstacle.
If colliding with "Player": Sets GlobalSubstance.obstacleTriggered to true to signal that the player has hit an obstacle, and then destroys the player game object.

# Script 35 - Obstacle2: Handling Collision with Player and Border
This script is similar to the previous Obstacle script and handles interactions between obstacles and other game objects.

Purpose:
Manages collisions between obstacles and other tagged objects, and updates the game state accordingly.

Public Variables:
scoreValue- Represents the score awarded for the obstacle; not currently used in this script.

Private Variables:
player- Reference to the player game object.

Private Methods:
Start()- Finds and assigns the player game object when the game starts. | 
OnTriggerEnter2D(Collider2D collision)- Handles collisions with other game objects:

If colliding with "Border"- Destroys the obstacle. | 
If colliding with "Player"- Sets GlobalSubstance.obstacleTriggered to true to indicate that the player has hit an obstacle, and then destroys the player game object.

# Script 36 - Obstacle3: Collision Management
This script handles interactions between obstacles and other game objects, specifically dealing with player collisions and border interactions.

Purpose:
Manages the behavior of obstacles when they collide with the border or player.

Public Variables:
scoreValue- Represents the score value associated with the obstacle; currently unused in the script.

Private Variables:
player:- Reference to the player game object.

Private Methods:
Start()- Finds the player game object tagged as "Player" when the game starts. | 
OnTriggerEnter2D(Collider2D collision)- Handles collisions:

If colliding with "Border"- Destroys the obstacle game object. | 
If colliding with "Player"- Sets GlobalSubstance.obstacleTriggered to true to indicate that the player has collided with an obstacle and destroys the player game object.

# Script 37 - PauseMenu: Manages Game Pausing and Resuming
This script controls the pause menu functionality, including pausing and resuming the game, and managing background music.

Purpose:
Manages the display of the pause menu, game time scale, and background music during pauses.

Serialized Fields:
pauseMenu- The UI element for the pause menu.

Private Variables:
backgroundMusic- Reference to the BackgroundMusic script to control music playback. | 
gameOverScript- Reference to the GameOver script, which might be used to check or control game-over state. | 
canAccessPauseMenu- Boolean flag indicating whether the pause menu can be accessed.

Private Methods:
Start()- Initializes the game state, sets time scale to normal, hides the pause menu, and finds references to necessary scripts.

Public Methods:
Pause()- Displays the pause menu, stops game time, and pauses the background music if the pause menu is accessible. | 
Resume()- Hides the pause menu, resumes game time, and unpauses the background music. | 
Home(int sceneID)- Loads a specified scene, setting the game time back to normal. | 
SetAccessToPauseMenu(bool state)- Allows or disallows access to the pause menu based on the boolean state.

# Script 38 - PersistentObject: Ensures an Object Persists Across Scenes
This script ensures that a GameObject with this script attached will persist between scene loads.

Purpose:
Keeps the GameObject from being destroyed when a new scene is loaded.

Private Methods:
Awake()- Calls DontDestroyOnLoad on the attached GameObject, preventing it from being destroyed when a new scene is loaded.

# Script 39 - Player: Controls Player Movement and Character Management
This script manages player movement, character selection, and handles game-over scenarios.

Public Variables:
playerSpeed- Speed of the player. | 
gameOverPanel- UI panel shown when the game is over. | 
playerCharacters- Array of player character GameObjects. | 
characterDB- Reference to the CharacterDatabase. | 
artworkSprite- SpriteRenderer to display the selected character.

Private Variables:
rb- Rigidbody2D component for physics-based movement. | 
playerDirection- Direction vector for player movement. | 
selectedOption- Index of the selected character.

Methods:
Start()- Initializes the Rigidbody2D, game-over panel, and sets up the selected character based on PlayerPrefs. | Loads a character database resource.

UpdateCharacter(int selectedOption)- Updates the displayed character sprite based on the selected index.

GetCharacterIndex(string characterName)- Returns the index of the character with the specified name.

Update()- Reads vertical input to set the movement direction and shows the game-over panel if no characters are available.

FixedUpdate()- Applies movement based on the direction vector and speed.

Restart()- Reloads the current scene to restart the game.

# Script 40 - PlayerMovement: Manages Player Movement and Pause State
This script controls player movement and handles pausing and resuming the player’s movement.

Private Variables:
controller- Reference to the CharacterController component. | 
normalSpeed- Movement speed of the player when not paused. | 
pausedSpeed- Movement speed stored when the player is paused. | 
isPaused- Boolean indicating if the player is currently paused. | 

Methods:
Start()- Initializes the CharacterController component. | 
Update()- Moves the player based on normalSpeed if not paused. Movement is in the direction of transform.right. | 
PausePlayer()- Sets isPaused to true, stops movement by setting normalSpeed to 0, and stores the current speed in pausedSpeed. | 
ResumePlayer()- Resumes movement by restoring normalSpeed from pausedSpeed and sets isPaused to false. | 

# Script 41 - QuickPauseButtonToggle: Simulates Button Click for Quick Pause
This script simulates a button click to trigger a pause action shortly after the scene starts.

Public Variables:
pauseButton- Reference to the UI button component that triggers the pause action.

Methods:
Start()- Calls SimulateButtonClick after a 0.1-second delay to simulate a button click. | 
SimulateButtonClick()- Invokes the onClick event of the pauseButton if it is not null.

# Script 42 - Resetter: Scene Reset with Delayed Sound and Music Handling
This script manages scene resetting with sound effects and background music.

Public Variables:
buttonSound- Reference to the ButtonSound script to play sound effects. | 
backgroundMusic- Reference to the BackgroundMusic script to manage music.

Methods:
ResetSceneWithSound()- Initiates the scene reset process by starting the coroutine ResetSceneWithDelay().

ResetSceneWithDelay()- 
Plays a sound effect if buttonSound is not null. | 
Waits for the sound effect to finish playing (15 seconds or adjust as needed). |
Resets and unpauses the background music if backgroundMusic is not null. | 
Reloads the current scene.

# Script 43 - RestartButtonHandler: Handle Button Click to Manage GameObjects
This script handles a button click to activate a script and manage GameObjects.

Public Variables:
holder- The GameObject that will be deactivated. | 
aaaScript- Reference to the AAA script that manages the deactivation.

Methods:
Start()- Checks if aaaScript and holder are assigned; logs a warning if not. | 
Gets the Button component and subscribes to its onClick event to call ActivateAAAAndDeactivateHolder.

ActivateAAAAndDeactivateHolder(): Calls DeactivateGameObject() on aaaScript to handle the deactivation of the holder GameObject.

# Script 44 - SampleSceneController: Manage Active Characters Based on Selection
This script manages which player characters are active based on the saved selection.

Public Variables: playerCharacters- Array of GameObjects representing different player characters.

Methods:
Start()- Retrieves the selected character index from PlayerPrefs (default is 0). | 
Iterates through the playerCharacters array, disabling characters that do not match the selected index. | 
Assumes the name of each character GameObject contains its index as an integer.

# Script 45 - SceneButton: Load Scene on Button Click
This script handles loading a new scene when a button is clicked.

Public Variables:
sceneName- The name of the scene to load.

Private Variables:
button- Reference to the Button component attached to the GameObject.

Methods:

Start()- Retrieves the Button component. | Attaches the LoadSceneOnClick method to the button's click event.

LoadSceneOnClick():
Loads the scene specified by sceneName when the button is clicked.

# Script 46 - SceneLoader: Play Sound and Load Scene
This script plays a sound and then switches to a new scene after a delay.

Public Variables:
soundPlayer1- Reference to the AudioSource used for playing sound. | 
sceneNameToLoad- The name of the scene to load. | 
sceneSwitchDelay- The delay before switching the scene (default is 5 seconds). | 

Methods:
PlaySoundAndSwitchScene()-
Sets the volume of soundPlayer1 based on GlobalVolume.ButtonVolume. | 
Plays the sound and schedules SwitchScene to be called after sceneSwitchDelay seconds. | 
If soundPlayer1 is not assigned, SwitchScene is called immediately.

SwitchScene():
Loads the scene specified by sceneNameToLoad.

# Script 47 - SceneSwitcher: Play Sound and Load Scene
This script manages scene switching with sound effects. It plays a sound, waits for a specified duration, and then switches to a new scene, stopping the sound if necessary.

Public Variables:
soundPlayer1- Reference to the AudioSource used for playing the sound. | 
sceneToLoad- The name of the scene to load. | 
soundDuration- The duration to wait before switching scenes (default is 0.15 seconds).

Methods:
PlaySoundAndSwitchScene()-
Plays the sound if soundPlayer1 is assigned. | 
Schedules KillSoundAndSwitchScene to be called after soundDuration seconds. | 
Logs messages based on whether the sound is playing or not.

KillSoundAndSwitchScene()-
Stops and disables soundPlayer1 if it is still playing. | 
Calls SwitchScene to change to the new scene. | 
Logs messages about the sound status and scene switch.

SwitchScene()-
Loads the scene specified by sceneToLoad. | 
Logs a message indicating the scene switch.

# Script 48 - SceneSwitcher2: Play Sound and Delay Scene Switch
This script handles scene transitions with an optional sound effect and a configurable delay. It plays a sound effect, waits for a specified delay, and then switches to a new scene.

Public Variables:
soundPlayer1- Reference to the AudioSource for playing the sound. | 
sceneToLoad- The name of the scene to be loaded. | 
sceneSwitchDelay- The delay before switching scenes (default is 5 seconds).

Methods:
PlaySoundAndSwitchScene()-
Plays the sound if soundPlayer1 is assigned. | 
Uses Invoke to call SwitchScene after the sceneSwitchDelay. | 
If no sound is assigned, it calls SwitchScene immediately.

SwitchScene()-
Loads the scene specified by sceneToLoad.

# Script 49 - SceneSwitcher2VolumeCopy: Play Sound with Volume Control
This script plays a sound effect with volume controlled by a global variable.

Public Variables:
soundPlayer1- Reference to the AudioSource for playing the sound.

Methods:
PlaySound()-
Sets the volume of soundPlayer1 using GlobalVolume.ButtonVolume. | 
Plays the sound if soundPlayer1 is assigned.

# Script 50 - ScoreManager: Manage and Display Score
This script manages and displays the player's score, including dynamic visibility effects and continuous score increment.

Public Variables:
scoreText- UI Text component to display the score.

Private Variables:
score- Current score value. | 
scoreIncreaseRate- Rate at which the score increases over time. | 
scoreIncreaseAcceleration- Acceleration rate for the score increase. | 
isScoreIncreased- Flag to manage score visibility toggling. | 
scoreIncreaseDuration- Duration for toggling visibility of increased score. | 
scoreIncreaseTimer- Timer to track duration of visibility toggle. | 
isScoreVisible- Flag to manage score text visibility.

Methods:
Start()-
Initializes the score and updates the display.

Update()-
Increases score continuously based on time. | 
Adjusts score increase rate and manages visibility toggling. | 
Resets score if it exceeds 99999. |
Updates score text display.

UpdateScoreText(float currentScore)-
Formats and updates the score text with leading zeros. | 
Ensures score text visibility if score is zero.

GetScore()-
Returns the current score.
