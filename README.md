# Less-Modular-Scale
Modular Scale for LESS CSS

A LESS mixin for creating modular scales.

# Usage

Import the mixin into a regular LESS file and use the ms() function to create modular font sizes:

    .ms(@number[, @base, @ratio])

Basic use only needs @number:

    h1 {.ms(1);}
    h2 {.ms(0);}
    h3 {.ms(-1);}
    h4 {.ms(-2);}
    h5 {.ms(-3);}
    h6 {.ms(-4);}

or, to change the parameters use your own :

    h1 {.ms(1, 2em, 1.2);}

or use the predefined ratios:

    h1 {.ms(1, 2em, @minorSecond);}

to globally override the values used:

    @msBase: 2em;
    @msRatio: @majorSixth;
    h1 {.ms(1);}
