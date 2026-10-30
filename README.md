# Bomberman World — [your game title]

**Student:** Arad Jamali Moghadam


## How to play

- **Controls:** WASD arrows to move, space to place a bomb , G to detonate the bombs
- Enter to start, Space to restart after gameover, Q / Esc to quit

- **Objective and rules:** rach to 100 points by killing enemies , each enemy gives 10 points. Lose when health <19 , each hit is 20. win has piroty if both happens.Dead enemies drop a +1 range pick up, max is 8. Max 3 Bombs . 
- **Configurations / demo setup:** default
## Features and validation


| Feature | Check, observed result, and expected behaviour |
| --- | --- |
| 1. Player damage and death | Died once by blast, once by enemy; standing next to an enemy did no damage. As expected. |
| 2. Round states and objective | Won one round and lost one; gameplay stopped on the end screen both times.  Lose if time runs out. As expected. |
| 3. Safe restart | Died with a bomb still ticking and restarted; no old explosion appeared and the layout was the same. As expected. |
| 4. Solid bombs with owner escape | Placed a bomb, walked out, could not walk back in; pressing Space twice on one tile gave one bomb. As expected. |
| 5. Blast-range pickup | Bomb before pickup had range 3, bomb after had 4; walking back over the spot gave nothing. As expected. |
| #6 Multiple bombs | Placed 3, the 4th was rejected; after one exploded I could place again. As expected. |
| #11 Scoring and combos | Two quick kills gave x2; after 5 s it went back to x1; restart cleared both. As expected. |
| #13 Remote detonation | G exploded my bombs; G with no bombs did nothing; it worked again after. As expected. |



**Known issues:**  One GameOVER state instead of separate Won/Lost,Knockback can push the player into a crate

## Sources and assistance
This project builds on the shared Kotte foundations. No collaborators.

I used AI for learning and debugging, using the suggested prompts like “Give me a hint”. For some small parts I got the code / 10 different ways of doing it. I tested all features myself in the Release build.

In my experience it helped me more when I started writing the code and sometimes asked for guidance, instead of asking it to explain the given code to me line by line. 
