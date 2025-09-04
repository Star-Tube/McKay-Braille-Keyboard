# Abstract

A keyboard input device designed to allow braille users to input to computer devices using a single hand.
Using 6 buttons to represent the six dots in braille characters, a confirm button, a backspace button and a newline button the user of this device could type any text that can be typed with braille with a single hand.
7 buttons for braille characters which use 5 or 6 dots are also provided for ease of entry as those characters may be difficult for some users to achieve with the main six buttons.
An escape button is also present for navigation purposes.

***

# The McKay Braille Keyboard

This device represents an innovation in the field of assistive technology and input devices.

When investigating the meaning of some braille text I stumbled upon an image of a braille keyboard (Figure 2) which I found to be ridiculous. It was the width of a standard keyboard but instead of the conventional five or even six rows it had seven rows. It must have had at least fifty buttons and, upon seeing it, I thought to myself "That would be difficult for me to use... and I can see it properly. I couldn't imagine trying to use it with impaired vision." I now know that that keyboard was far from the norm, but it did set me down an attempt to design my own solution which I hope will help people. This design stands in contrast with the conventional solutions, a normal keyboard with braille bumps added which still required two hands to conveniently and quickly type on, and the 6 button or 8 button braille keyboards which, while effective, also requires both hands to use and prevents the user from touching other material, preventing them from effectively transcribing or monitoring their input without use of an auditory output method.

The design I have landed upon, on the other hand, allows the user to input braille characters using only one hand. I hope this allows some braille users to use braille output devices while they type, similar to how people who touch type can look at their screen while they type, and allow braille users to transcribe braille text.

It achieves this using 6 input keys in a two by three grid on which the users index, middle and ring finger will rest. The user can then use those three fingers, with the optional assistance of their fourth finger, input the braille character as if it were rotated ninety degrees. Then, once the correct buttons are pressed, they can confirm that character using their thumb on the confirm key, situated like a spacebar on conventional keyboards. This design would allow the user to input any braille character using only one hand, excepting that characters with five or more dots may prove difficult to input as one finger would have to press two buttons at once. I have solved that problem by including seven additional keys, one for the case of six dots and 6 for the cases of five dots. This allows the user to quickly input both simple and more complex characters.

Operating system navigation buttons such as escape, control, alt and insert can easily be added to this design on the periphery and I have included an escape button in the design to demonstrate this. A complete implementation including some or all navigation keys is trivial to create either adding the extra keys above the highest row of keys, to the right or left of the board or replacing some or all of the seven keys assigned for characters with five or six dots for users who do not need them, or any combination of the above solutions.

Figure 1 is a diagram showing an implementation of my design in a layout showing the six main input buttons labeled 1 and the confirm button labeled 6. Surrounding the six main input buttons are the seven buttons for inputing characters with greater than four dots labeled 2. It also shows a newline button labeled 4 and a backspace button labeled 5 as well as an escape button labeled 3.

In order to implement this design, one can design a PCB which connects a switch matrix covering all switches to a controller such as an Arduino Pro Micro and configure it using a keyboard library such as Arduino's community Keypad library to behave as intended. Then manufacture a case and install keycaps.
