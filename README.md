SVG Crossword maker
===================

Use this to generate SVG crossword grids and puzzles.

    - From prefab ascii grids for example:

        open
        g**o
        r**o
        eats
        ***e

        Execution pattern:

         $ python make-crossword.py input.txt > crossword.svg


If you want to just supply a list of words and have it generate the layout for you, you can also do that!

For example:

    - From ascii word lists.

        Execution pattern:

        $ python make-crossword.py --generate 20x20 sample_generate.txt > crossword-generated.svg

        command line argument:
        --generate WxH where W is the number of columns and H is the number of rows. 

This will generate a filled-in crossword.

The output looks like this:

![Sample output](http://i.imgur.com/NaAoY1R.png)

If there are words that couldn't fit, they are printed to standard error.
We can alternatively save the board to a file to finish it by hand using

        command line argument:
        --save_generate <file name>.

![Sample generated output](http://i.imgur.com/cMR0X2R.png)

