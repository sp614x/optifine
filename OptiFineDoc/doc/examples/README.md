# Resource Pack Examples

This folder contains a collection of resource packs that demonstrate OptiFine's resource pack features.

## Emissive Textures

This resource pack showcases emissive textures, making certain blocks and items glow in the dark for enhanced visibility and aesthetics.

<details>
  <summary><strong>Features</strong></summary>
  <ul>
    <li>Emissive diamond, emerald, and gold ore blocks</li>
    <li>Emissive slime block showing variable emissive brightness</li>
    <li>Zombie with glowing eyes</li>
    <li>Glowing diamond sword</li>
    <li>Glowing sentry emerald armor trim</li>
  </ul>
</details>

## Random Entity Textures

This resource pack showcases OptiFine’s Random Entity Textures feature, allowing entities to have different textures based on various conditions such as custom names or weighted randomness.

<details>
  <summary><strong>Features</strong></summary>
  <ul>
    <li>Cows use the default behaviour. With no properties file, they will show all the provided textures randomly</li>
    <li>Chickens receive unique textures based on their names. If no name is present, it will fall back to weighted randomness.</li>
    <li>Slimes have a unique texture in the jungle, bamboo jungle, and ocean biome. The texture also has a 10% chance to show up in a swamp biome.</li>
    <li>Endermen use NBT checks to change texture based on the block they are holding. When holding a grass block, they will change texture.</li>
  </ul>

  ### Chicken Name-Based Textures

  | Name Condition                  | Match Type       | Behavior                                        |
  |---------------------------------|------------------|-------------------------------------------------|
  | Cluckshroom                     | Case Sensitive   | Must be an exact match                          |
  | Amber Chicken                   | Case Insensitive | Uses `ipattern`                                 |
  | Bronzed                         | Case Insensitive | Uses `ipattern`, allows extra text before/after |
  | Gold Crested                    | Case Insensitive | Uses `iregex`, allows extra text before/after   |
  | Midnight / Midnight Chicken / 5 | Case Insensitive | Multiple name options using `iregex`            |
  | Skewbald / Skewbald Chicken / 6 | Case Insensitive | Multiple name options using `iregex`            |
  | Stormy / Stormy Chicken / 7     | Case Insensitive | Multiple name options using `iregex`            |
</details>

## CEM Animation Examples

This resource pack features a collection of useful animations for custom entity models, covering everything from basic movements to advanced, complex animations.

<details>
  <summary><strong>Animations</strong></summary>

  | Model Name               | Animation Description                                                                                                              | In-Game Effect                                                                                                   |
  |--------------------------|------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
  | **spider.jem**           | Custom leg animations, not based on any existing legs.                                                                             | Three sets of legs with different swinging animations. First are normal, second move faster, third move further. |
  | **villager.jem**         | Custom head animation, not based on an existing head.                                                                              | The head looks around normally, but uses custom animations.                                                      |
  | **allay.jem**            | Limits values using min, max, or clamp.                                                                                            | Four swinging elements, one swings freely, two are limited in different directions, one is limited in both.      |
  | **zombie.jem**           | Stores a value and uses it across multiple animations (does not work for block entities).                                          | One sine wave is defined in the model, but it is used across three different elements in different ways.         |
  | **pig.jem**              | Creates a counter independent of time or age.                                                                                      | The pigs head spins constantly.                                                                                  |
  | **panda.jem**            | Uses custom counters to create smooth transitions with boolean values.                                                             | When the panda gets wet, its head takes smoothly rotates over a couple seconds to be upside down.                |
  | **husk.jem**             | Allows an entity to have randomized animation speeds, unique per instance.                                                         | Each husk's head wobbles side to side at different random speeds.                                                |
  | **cow.jem**              | Plays an animation when the player meets certain distance requirements.                                                            | One cube rotates when player is far away, one when medium distance, and one when close by.                       |
  | **piglin_brute.jem**     | Make elements ignore entity rotation, instead always facing north.                                                                 | The piglin model will be rotated to always face north.                                                           |
  | **creeper.jem**          | Makes a 2D plane always face perpendicular to the camera view, keeping 90-degree angles to the screen regardless of viewing angle. | The plane always looks like a perfect square pointed straight at your screen.                                    |
  | **skeleton.jem**         | Makes a cube face directly at the player's in-world position.                                                                      | The cube rotates to always look at your in world player model.                                                   |
  | **wither_skeleton.jem**  | Cancels the default death animation so mobs do not fall over when they die.                                                        | The wither skeleton remains standing upon death.                                                                 |
  | **piglin.jem**           | Cancels the default death animation and applies a new one.                                                                         | The piglin floats up into the air when it gets killed.                                                           |
  | **zombified_piglin.jem** | Snaps a model to the nearest in-game block.                                                                                        | The cube aligns precisely with the block grid, snapping to the next one instead of moving smoothly.              |
  | **armor_stand.jem**      | Plays an animation, waits a random amount of time, then repeats.                                                                   | The cube does a full rotation, then waits a random amount of time before doing another full rotation.            |

<details>