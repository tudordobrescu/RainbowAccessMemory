# RainbowAccessMemory
The RainbowAccessMemory arcade game generates random audio-visual patterns that players must replicate when prompted.

By using the DaisySeed microcontroller, the Adafruit MPR121 and the Adafruit NeoTrellis, we envisioned a fairly addictive
pocket arcade-game that uses a light-and-sound matrix. The large button generates a series of patterns using an oscillator
algorithm and the NeoTrellis leds. The player must then replicate the exact pattern, and he will be rewarded with green 
lights. Otherwise, the NeoTrellis becomes entirely red and flashy, while the player must introduce a correct pattern. 
The game can always be restarted by using the big arcade button. Originally, the game was meant to be multiplayer, and will
most likely be further developed in this direction.

The DaisySeed, Adafruit NeoTrellis and Afafruit MPR121 are all connected to a breadboard. Wires are used to connect the 
Arcade Button to the breadboard, the touch sensors to the additional buttons and the NeoTrellis to the breaboard as well. 
The code then connects each touch pad to a certain sound and a certain NeoTrellis Light. The Arcade Button generates patterns
of four audio-visual outputs that are remembered in an array. The array is then compared to another array that keeps the 
information typed in by the player. Finally, it compares the two and flashes all the green leds if they match and all the red
ones if the player typed in incorrectly.
