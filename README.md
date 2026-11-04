# Tamagotchi Clone

<img width="704" height="739" alt="2026-11-04-000819_hyprshot" src="https://github.com/user-attachments/assets/13d8eb7e-fdc3-4a37-bbde-a67f673f0200" />

my project for week... 4? of hackclub halflife.

the theme this week was display, and I rather like working with displays, so obviously my first thought was "how can I fix that?" I decided that the situation in which displays are the most annoying is battery critical electronics, and also small displays are a pain in the ass, so why not make it tiny? then I remembered this tamagotchi bag that I got after being scammed out of an actual tamagotchi by a gatcha machine and that's how this project was born.

# Components

for the display I use a crystalfontz CFAG12864T3-NFH, which is a LCD that has transflective coating behind it instead of a backlight making it super duper power efficient and also giving it the cool retro aesthetic of the display from the original tamagotchi and gameboy, but you cant see it in the dark

for the microcontroller I use a msp430g2553in20 because it is super power effecient and has the most RAM of any msp430 in a DIP package, which makes it easy to swap between the dev board (the MSP-EXP430G2ET) and the actual board

the battery is just a CR2450 coin cell

and the rotary encoder is just some adafruit something I had laying around.

# PCB

the main difficulty with this PCB was getting the shape right, I had to make the outline first in an onshape sketch and then record the positions of each circle and use those as the offsets for arcs in kicad, and then do some snapping shenanigans. kicad really wasn't meant for that kind of thing. after that it was pretty much just connect the dots. Also fitting in the battery was pretty gnarly. I am yet to do the flower pattern on the silkscreen and copper mask, I will tell you how that goes when I finish it!

also there are no manufacturing files yet because I'm gonna make those when I finish the board and this week dident require them

<img width="545" height="536" alt="2026-11-04-001146_hyprshot" src="https://github.com/user-attachments/assets/2eaf7e0a-93dd-4ea7-ab5a-b0c6091d77ce" />
<img width="558" height="559" alt="2026-11-04-001116_hyprshot" src="https://github.com/user-attachments/assets/2f5f6884-1288-4663-8478-583bb8daa021" />

# Firmware

I haven't done the firmware yet because I don't have a microcontroller to test on.

I'm sure it will be very interesting though! I get to deal with a microcontroller I'm new to at a low level with the added difficulty of giving it narcolepsy and having the working memory of a goldfish.
