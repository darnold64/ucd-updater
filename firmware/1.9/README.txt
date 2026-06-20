Ultimate Computer Deck
v1.9  - Initial Release
by: Dean Arnold
date: 07-Jun-2026
hardware: XIAO ESP32C3
          6x10 NeoPixel LED Matrix
          DFPlayer - Mini MP3 Player (DFR0299)

The firmware on the MCU controls a 6x10 LED Matrix allowing the performer to present Del Ray's wonderful 
card effect The Computer Deck.  The basic effect involves a freely selected card which is 
returned to the deck and the deck then split into four face-up piles. The computer card case 
is placed on the piles one at a time and the lights start flashing when it lands on one particular 
pile. The computer continues to work and finally stops at the number “8” on the digital display. 
On counting down, the selection is located at the eighth position.

The computer can be set to one of three modes: 1) Classic: where the performer can cause the 
computer to come alive on each pile scanning for the card.  If it is not in the pile, an 'X' 
appears.  When placed on the correct pile, the performer can cause the computer to indicate 
this by a check mark, and then the position of the card is displayed (user configurable).  This 
mode also allows the Ultimate Computer Deck (UCD) to display any selected card the performer wishes 
to show.  2) Reveal: where the UCD verifies that the card has been found with a checkmark then 
indicates the card's value followed by its suit.  The performer can then indicate its position 
(user configurable) in the deck. 3) Stack: if using a stacked deck (user configurable) the UCD can
display a card at a given position or the position of a card entered.  The performer can have the
deck/stack cut and still determine the correct position or card by first entering either the top or 
bottom card (user configurable) of the stacked deck.  

The card location sequence can be activated by either a 12-button remote transmitter (using ESP-NOW) 
or by a magnet which closes a reed switch located on the custom Card Computer PCB.  If no activity
is initiated by the performer the computer will go into deep sleep in order to conserve battery 
after a user defined period of time.  Once in deep sleep mode, the computer can be woken-up by 
placing the deck(board) vertically. 

This version also supports the ability to play MP3 and WAV sound files using the DFPlayer Mini MP3 
Player Module.  The DFPlayer module stores audio clips on a micro SD card (upto 32G), supports 
MP3/WAV formats, and offers features like looping and volume adjustments.  With this module when 
the selected card is revealed on the LED matrix it is also announced.  Other special sound effects 
are played accompanying the various animations. Note: The order you copy the mp3 onto the micro SD 
card will affect the order mp3 played, which means play(1) function will play the first mp3 
copied onto the micro SD card regardless of track name/title.
