Act as an expert Game Developer. I want to build a "bullet heaven" web game (similar to Vampire Survivors) using HTML5 Canvas and vanilla JavaScript (or Phaser.js if you prefer). 

### Core Game Specs:
1. **Movement:** WASD or Arrow keys. The player is always at the center of the screen; the world/enemies move around them.
2. **Combat:** Automatic weapons that fire at the nearest enemy based on a cooldown.
3. **Enemy Logic:** Endless waves of enemies that track the player's position. Different enemy types have different colors and "abilities" (e.g., a fast dash, a projectile, an area-of-effect pulse).

### Unique Mechanic: "The Ability Swap"
- Remove the traditional "Level Up" menu where you pick static upgrades.
- When an enemy dies, it has a 10% chance to drop a "Soul Orb."
- When the player touches a Soul Orb, the game pauses and shows a "Swap?" prompt.
- The player must choose to either:
    a) Keep their current ability.
    b) DISCARD their current primary weapon/ability to take the signature ability of the enemy that dropped the orb.
- Visuals: If I swap with a "Fire Bat," my projectiles should now be fireballs. If I swap with a "Frost Slime," I now leave a freezing trail.

### Technical Architecture:
- Please provide a single-file solution (index.html) including CSS and JS for simplicity.
- Use a simple Entity Component System (ECS) pattern so adding new enemy types and weapon types is easy.
- Include a basic HUD showing "Kills" and "Current Ability Name."

Start by scaffold out the basic engine, the player movement, and the spawning system for three basic enemy types.