# Less-Modular-Scale
Modular Scale for LESS CSS

A LESS mixin for creating modular scales.

# Usage

Import the mixin into a regular LESS file and use the ms() function to create modular font sizes:

    .ms(@number[, @base: 1em, @ratio: @majorSecond])

Basic use only needs @number:

    h1 {.ms(6);}
    h2 {.ms(5);}
    h3 {.ms(4);}
    h4 {.ms(3);}
    h5 {.ms(2);}
    h6 {.ms(1);}

or, to change the parameters use your own :

    h1 {.ms(6, 2em, 1.2);}

or use the predefined ratios:

    h1 {.ms(6, 2em, @minorSecond);}

to globally override the values used:

    @msBase: 2em;
    @msRatio: @majorSixth;
    h1 {.ms(6);}
