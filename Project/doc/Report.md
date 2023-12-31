# Project report

### HTML5 Game : Block Game

Leevi Laitala

<br>

Fulfilled features listed in the project work google docs file:

| Feature                                   | Points | Max  | Notes           |
|-------------------------------------------|--------|------|-----------------|
| Well written PDF report                   | 3      | 3    |                 |
| Responsive application                    | 2      | 4    | Only on desktop |
| Firefox, safari and chromium              | 3      | 3    |                 |
|                                           |        |      |                 |
| Clear plot                                | 3      | 3    |                 |
| User can get their name in the scoreboard | 3      | 3    |                 |
| There is more than one map                | 3      | 3    |                 |
| Game uses physics engine                  | 2      | 2    |                 |
| There are enemies that hurt player        | 3      | 3    |                 |
| There is music and sound effects          | 3      | 3    |                 |
|                                           |        |      |                 |
| **Total**                                 | 25     |      |                 |

<br>

### Own features

List of own features and their corresponding points, with explanations
written below.

| Feature                       | Points |
|-------------------------------|--------|
| Particles                     | 3      |
| Maps                          | 2      |
| Unique minimal look and flow  | 3      |
| Leaderboard styling           | 2      |
| Good repo structure           | 3      |
| Player can change room layout | 2      |
| Scoring                       | 2      |
|                               |        |
| **Subtotal**                  | 17     |
|                               |        |
| Features in google docs       | 25     |
|                               |        |
| **Total**                     | 42     |

<br>

#### Particles

I've used the engine's own particle system on player's trail and other things. 
I also included my own physics particles, since the particle engine does not 
support interaction between particles and physics objects.

My own is not necessarily a particle system, even though is used as it. It's
only a pool of physics objects, that can be scattered by function call.

**Points:** 3

<br>

#### Maps

I created easy way to create more rooms to the game, also with tutorials. 

See `src/maps.js`

**Points:** 2

<br>

#### Unique minimal look and flow

The game uses shapes provided by phaser, instead of sprites. Only one small
image is needed for particles, since phaser does not support shapes as 
particles for some reason.

I think the game has good flow, since the player is persistent in a single 
scene, and the room itself changes it's layout upon reaching goal.

Player respawn is quick, like in *Hotline Miami*, and restarting game is 
seamless finishing the game.

**Points:** 3

<br>

#### Leaderboard styling

Leaderboard is a HTML table, which is generated by the game. Majority of 
visible HTML elements have CSS styling.

Top player is highlighed with green color.

**Points:** 2

<br>

#### Good repo structure

Assets have their directories based on their type, and code files are split into
files by their role. 

**Points:** 3

<br>

#### Player can change room layout

Even though there are not moving walls in the game, there are gates that the
player can unlock when collecting a key.

**Points:** 2

<br>

#### Scoring

Player's score is the amount of deaths occured during the playthrough. Less
is of course better.

And if player would **cheat**, eg. skipping room using '4' key, ton of deaths
would be added to not enable anyone grief the leaderboard.

**Points:** 2

