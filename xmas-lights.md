Winter is coming, and you are programming a simple Xmas lights gadget for your niece.

The lights can be switched on an off, and if it is on, its color can be switched by a color switcher. The color rotates through a given color list.

The `Lights` class should implement this behavior.

1. There is a default constructor which creates an RGB lights: starting as RED, then can be switched to GREEN and then BLUE. A next switch wil turn the color to RED, and the cycle starts again.

2. There is another constructor which receives a list of strings (holding colors) and creates a lights: it starts as the first color in the list, then it can be switched along the list. At the end the color starts again

3. A method called `switchPower` turns the lights on and off. The lights always starts as the first color in its list, whatever happened before. A method called `isTurnedOn` checks if the lights is on.

4. A method called `switchColor` picks the next color from the list (only if the lights is on). A method called `getColor` returns the color name as a string. It should return `"RED"`, `"GREEN"`, or `"BLUE"` in the case of the default lights. `getColor` should return `null` if the lights is switched off.

5. A method called `reverse` turns the direction of color rotation.
