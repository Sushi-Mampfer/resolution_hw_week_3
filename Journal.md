# Monday, 30 March
I tried to understand a 555, but I was unable to, even with many YouTube videos. I just lacked the general understanding of electronics.
**Time spend: 1h**
# Tuesday, 31 March
I traveled and watched ~~some~~ a lot of videos about electronics on the go.
**Time spend: 0h**

# Wednesday, 1 April
With my newly gained knowledge I was finally able to understand some of the ICs(NE555/CD4017B/CD4022B) and started adding them to my ICs.md file.
But following logic diagrams still took forever. Especially because I couldn't find any truth table for the D Flip Flop with a reset.
I asked ChatGPT a few times, but most of the time it just produced nonsense, for example: I asked it about the CARRY OUT pin and it just said some nonsense that wouldn't even have worked in it's own example.

**Time spend: 2h**

# Thursday, 2 April
I finished up the CD4017B and continued with the CD4020B (and CD4024B/CD4040B), they went rather smooth as I started getting the hang of reading logic diagrams, except for the reset logic which just didn't make sense at first, but overall it was way easier than the CD4017B.
**Time spend: 1h**

# Friday, 3 April
I added the NE555 which was pretty easy, because I already understood most of it from Wednesday. After that I started working on the CD4060B, but eventually gave up on it, because the examples didn't make much sense to me and I didn't think that I would need it for my circuit. After that I started working on my circuit. My first idea was to make a digital clock, but since other IC's([sn7447a](https://www.ti.com/lit/ds/symlink/sn7447a.pdf)) aren't allowed it was pretty hard to use a 7 segment display, I tried some things with diodes, but using 49 diodes per 7 segment display, which there'd be at least 4 of if I don't add seconds(although some numbers would never be displayed, because there is no reason to show 90 minutes on a clock). After struggling a bit with KiCad I gave up on that(mainly because I couldn't figure out how to place such a large amount of components efficiently).
After that I did some brainstorming about what I could do and decided on an adjustable alarm. And then I did some more brainstorming on how I could do that.
**Time spend: 2h**

# Thursday, 9 April
After some more brainstorming between the last time I've worked on it I came to the conclusion that the CD4060B would be quite practical for my circuit and after watching some videos I finally understood it(wasn't that hard after all).
Then I got to work on the circuit, which was more or less smooth sailing, because I already had a pretty good plan in mind, there were only two things that took some time, finding the resistor values(which I did by trying some values in Falstad and after that asking ChatGPT if I missed anything that would fry it, which it luckily denied). And finding a toggle switch, I think I've got it right now(with some help from ChatGPT), it still shows as a push button, but I'm sure there is a toggle button with the same footprint.
After that I spend some time organizing the schematic and moved on to the PCB. Again it was pretty smooth sailing, except for some of the wiring, I still haven't fully understood the wiring tool, but CTRL+Z works wonders. The GND filled zone definitely made the wiring way easier and cleaner and I'm actually happy with it(although it could be a bit compacter).
I still don't know if it works, but I don't see why it wouldn't.
Turns out the reset switch wasn't connected on the schematic, so it would not have worked.

**Time spend: 5h** 
