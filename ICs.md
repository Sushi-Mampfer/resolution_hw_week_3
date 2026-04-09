# Important
- VCC/VDD: plus pole
- VEE/VSS: ground
# NE555

An IC that makes it easier to build consistent RC circuits. Can also be used as a flip flop.

> [!tip]
> Also available as a 2 in 1 IC under the name [NE556](https://www.ti.com/lit/ds/symlink/ne556.pdf).
### [Datasheet](https://www.ti.com/lit/ds/symlink/ne555.pdf)

### Pins(name in datasheet):
- **RESET**: Forces OUT to LOW and connects DISCH to GND when LOW
- **DISCH**: Connected to GND when OUT is LOW
- **TRIG**: When under 1/3 of input voltage sets out to HIGH and disconnects DISC from GND
- **THRES**: When over 2/3 of input voltage sets out to low and connects DISC to GND
- **CONT**: Can be used to change the required voltages, THRES > CONT and TRIG < 1/2 CONT

# CD4017B

A basic wrapping counter to 10 that changes by on each rising edge of the clock.

> [!tip]
> Also available to 8 instead of 10 under the name CD4022B
### [Datasheet](https://www.ti.com/lit/ds/symlink/cd4017b.pdf)
### Pins(name in datasheet):
- **CLOCK**: Advances the counter on the rising edge
- **CLOCK INHIBIT**: Blocks the clock, when clock is HIGH can be used to advance on falling edge
- **CARRY OUT**: LOW when 5-9 are HIGH, else HIGH
- **RESET**: Forces counter to 0 while HIGH
- **0-9**: Current count, wrapping, only one can be HIGH at a time

# CD4020B

A 14 stage ripple carry binary counter.

> [!tip]
> Also available as 7 and 12 stage under the name CD4024B and CD4040B respectively.

### [Datasheet](https://www.ti.com/lit/ds/symlink/cd4020b.pdf)

### Pins(name in datasheet):
- **INPUT**: Triggers the counter on it's falling edge
- **RESET**: Forces counter to 0 on HIGH
- **Q1-Q14**: Bits of the counter

# CD4060B

An oscillator with a 14 stage ripple carry binary counter.
### [Datasheet](https://www.ti.com/lit/ds/symlink/cd4060b.pdf)
### Pins(name in datasheet):
- **Q4-Q10**, **Q12-Q14**: Bits of the counter
- **R**: Forces counter to 0 and stops oscillator on HIGH
- $\emptyset _I$: input
- $\overline{\emptyset}_o$: Not of $\emptyset I$
- $\emptyset _o$: Not of $\overline{\emptyset}_o$
