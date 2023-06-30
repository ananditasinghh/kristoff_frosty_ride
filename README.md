# kristoff_frosty_ride

Kristoff_frosty_ride is a playable snow boarding game project that takes players on a thrilling journey through snowy cliffs and fields. It is built in Unity Hub 2021, and coded in C#. 

The game mechanics that are involved in this game are :

- Player Dynamics - rotation, speed, torque, smooth track with jumps
- Finish line that restarts the level
- Crash detection that restarts the level
- Audio and Sound 

The game Design is :

Player experience - Smooth and relaxing
Core Mechanic - Don't Crash 
Game loop - Reach the end to win

How to Play?

This project can be opened in Unity and is playable.



The development of this game is divided as follow :
 
Player and Mechanics:

The player's character, Kristoff, is the main focus of the game. The Sprite Shapes feature is ingeniously utilised to create the cliff and snow field environments, for adding a visually appealing touch to the gameplay.

To enhance the realism of snowboarding, the Surface Effector 2D is implemented to govern the mechanics of Kristoff's body during the gameplay. The AddTorque() function is utilised when the player jumps from one cliff to another, creating a natural rotation effect in mid-air.

Namespace And Management - used classes and methods from SceneManagement namespace, although because this is one player game so it won't be difficult to accommodate  and manage. But Namespace And Management is important for games where there are two or more players. 

The Invoke() function manages the timing after a hit, ensuring the game flows smoothly without abrupt interruptions. The arguement of how long the delay is to be passed in Invoke()

AngularDrag() plays a crucial role in maintaining player control by slowing down Kristoff's rotation, allowing for precise movements during critical moments.


<img width="500" alt="Screenshot 2023-06-29 at 8 45 43 PM" src="https://github.com/ananditasinghh/kristoff_frosty_ride/assets/97512151/79904034-2ee6-4c13-89a8-943a1809ee32">

<img width="500" alt="Screenshot 2023-06-29 at 8 43 22 PM" src="https://github.com/ananditasinghh/kristoff_frosty_ride/assets/97512151/6f9955a8-6529-4219-8d0d-f22ecc9b06fc">

Particle System and Crash Detection in the game :

Players will observe visual cues signalling Kristoff's interaction with the environment, whether it's  crossing the finish line flawlessly or experiencing a less fortunate encounter with the ground. (I know it's sad, but sometimes even the best of us happen to hit our heads on the ground, and for Kristoff its his first game :) )

The CrashDetector() function discreetly provides on-screen messages, whenever the player's character collides with the ground or crosses the finish line. 

Audio and Sound Effects:

The game has a soundscape with audio and sound effects. AudioSource is attached to a GameObject to ensure seamless playback of in-game sounds. In this game, we have used two sound effects(SFX), crash and finish.


<img width="500" alt="Screenshot 2023-06-29 at 1 46 44 PM" src="https://github.com/ananditasinghh/kristoff_frosty_ride/assets/97512151/35a84566-9654-4417-926e-d600a489b98f">

<img width="500" alt="Screenshot 2023-06-29 at 1 59 51 PM" src="https://github.com/ananditasinghh/kristoff_frosty_ride/assets/97512151/00d6f7bc-871a-4521-b030-18381e1fffd4">

Camera and View:

Cinemachine, a Unity plugin, plays a pivotal role in enhancing the overall gaming experience. With its following features :

-Virtual Cameras are strategically used to focus on the background scenery while smoothly following Kristoff's path throughout the game.

-Dynamic Tracking ensures that the camera automatically follows and adapts to the speed of various objects in the game environment, intensifying the sense of speed and thrill during high-octane segments.

-Camera Transitions provide seamless transitions between different curves in the game space, maintaining visual continuity and ensuring an uninterrupted snowboarding 


<img width="500" alt="Screenshot 2023-06-29 at 8 41 54 PM" src="https://github.com/ananditasinghh/kristoff_frosty_ride/assets/97512151/a171d6f2-379a-4c94-9a31-a106d001c065">

<img width="500" alt="Screenshot 2023-06-29 at 8 42 19 PM" src="https://github.com/ananditasinghh/kristoff_frosty_ride/assets/97512151/236e887e-f24b-43fe-8a0c-157762cf1049">




