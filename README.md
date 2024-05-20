# Car Drifting Adventure

## Introduction
Welcome to the Car Drifting Adventure project, developed in Unity, where you can experience the thrill of car drifting, nitro boosts, coin collection, and competing against other cars. In this game, you drive a black car, gather coins, avoid obstacles, and compete against red competitor cars. The game features a scoring system that rewards players for collecting coins and staying on the road while penalizing collisions and off-road driving.

![image](https://github.com/YousraBarhmi/CarGameUnity/assets/138295122/8503d771-5d27-4dbc-ab21-9d6c9b2659ea)


## Prerequisites
- Unity 2020.3 or later
- Basic knowledge of C# and Unity scripting

## Setting Up the Scene

### Building the Road
1. **Road Creation:** In Unity Editor, create a new Plane object to serve as the road. Adjust its position and scale to achieve the desired dimensions for the road.

### Creating Vehicles

#### Player Vehicle
1. **Player Car Creation:** Create cube to represent the player's car, or import a car prefab from the Unity Asset Store.
2. **Physics Simulation:** Attach a Rigidbody component to the player’s car to handle physics.

#### Competitor Vehicles
1. **Competitor Car Creation:** Create red cubes to represent competitor cars or import red car prefabs.
2. **Physics Simulation:** Attach a Rigidbody component to each competitor car for physics handling.

## Adding Game Objects

### Roadside Elements
1. **Roadside Boxes:** Create boxes to be placed randomly along the roadsides, ensuring they do not obstruct the road.

### Collectible Items
1. **Coin Prefabs:** Design and position coin prefabs strategically along the road for the player to collect.

## Implementing Behavior

### Competitor Behavior
1. **Instantiation:** Randomly place a fixed number of red competitor cars on the road, ensuring they stay within road boundaries.

### Coin Interaction
1. **Coin Animation:** Add simple animations or rotations to coins for visual effect.
2. **Coin Collection:** Destroy the coin and update the score when the player collects it.

## Scoring and Penalties
1. **Score Management:** Decrease the player's score if:
   - They leave the road.
   - They collide with any object other than coins.

## Drifting and Nitro Mechanics

### Drifting Simulation
1. **Drifting:** Use the Rigidbody component’s velocity and angularVelocity to simulate drifting. Adjust friction and steering for a realistic drifting experience.

### Nitro Boost
1. **Nitro Activation:** Allow nitro boosts once the player reaches a certain score. Temporarily increase the car's speed when nitro is activated. Reset the nitro availability upon collision.

## Camera Setup
1. **Camera Following:** Configure the camera to follow the player's car, ensuring it always focuses on the player.

## Additional Features

1. **Object Interaction:** Any road, box, or coin passed by the player will be destroyed.
2. **Future Enhancements:**
   - Improve graphics and car models for a more immersive experience.
   - Develop AI for competitor cars.
   - Add new levels and challenges.
   - Incorporate sound effects and background music.

## Running the Game

1. **Setup:** Clone or download the repository and open the project in Unity.
2. **Loading:** Load the main scene (`Samplescene.unity`).
3. **Playing:** Press the Play button in the Unity Editor to start the game.

## Game Controls

- **Steering:** Use the arrow keys or left and right arrows to steer.
- **Acceleration:** Press the up arrow or W to accelerate.
- **Braking/Reverse:** Press the down arrow to brake or reverse.
- **Nitro Boost:** Keep pressing the up arrow to activate nitro boost.

## License
This project is licensed under the MIT License. Refer to the LICENSE file for more details.
