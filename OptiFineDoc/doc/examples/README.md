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