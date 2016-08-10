##An ode to Piet

[Piet](http://www.dangermouse.net/esoteric/piet.html) is a language that instantly captured my attention when
I discovered it ages ago.  It endeared itself to me firstly because Mondrian has long been one of my
favorite artists.  But more than that, the central conceit of the language - navigating a two-dimensional
image, entering and exiting blocks of color according to rules based on the state of the program - introduces
a dynamic that makes any programming challenge a delicious puzzle that hits all of my favorite elements.

I've always been absorbed by these kinds of iterative puzzles, where you pick a place to start and strike out
in a direction, but eventually your starting decisions come back into play, and you have to alter your initial
plan, which inevitably cascades into further changes and compromises.  It reminds me of my favorite of
Simon Tatham's puzzle collection, [Galaxies](http://www.chiark.greenend.org.uk/~sgtatham/puzzles/js/galaxies.html).

Programming in Piet - especially if you take the additional step of trying to fit your program in a small space,
or otherwise have secondary goals in mind - is delightful, infuriating, and pointless, and I love it.  It gets
my brain going in a way that few other things do.

On that note, if you enjoy the spatial and programming elements of Piet but wish it were more text-based,
I highly recommend the delightful [TIS-100](http://www.zachtronics.com/tis-100/).  It's a game about programming
in assembly.  Yes, that does exist, and it's a blast.

##The programs

So far, it's just the one...time will tell if I get sucked into more.

###Tabula Recta

![Tabula Recta](https://github.com/cincodenada/piet_projects/blob/master/tabularecta_large.png)

This began with an accidental stumbling across a [post on the CodeGolf StackExchange](http://codegolf.stackexchange.com/questions/86986/print-a-tabula-recta)
with a simple challenge: output the following text, a "Tabula Recta", used in basic cryptography, such as the Vigenere cipher:

```
ABCDEFGHIJKLMNOPQRSTUVWXYZ
BCDEFGHIJKLMNOPQRSTUVWXYZA
CDEFGHIJKLMNOPQRSTUVWXYZAB
DEFGHIJKLMNOPQRSTUVWXYZABC
EFGHIJKLMNOPQRSTUVWXYZABCD
FGHIJKLMNOPQRSTUVWXYZABCDE
GHIJKLMNOPQRSTUVWXYZABCDEF
HIJKLMNOPQRSTUVWXYZABCDEFG
IJKLMNOPQRSTUVWXYZABCDEFGH
JKLMNOPQRSTUVWXYZABCDEFGHI
KLMNOPQRSTUVWXYZABCDEFGHIJ
LMNOPQRSTUVWXYZABCDEFGHIJK
MNOPQRSTUVWXYZABCDEFGHIJKL
NOPQRSTUVWXYZABCDEFGHIJKLM
OPQRSTUVWXYZABCDEFGHIJKLMN
PQRSTUVWXYZABCDEFGHIJKLMNO
QRSTUVWXYZABCDEFGHIJKLMNOP
RSTUVWXYZABCDEFGHIJKLMNOPQ
STUVWXYZABCDEFGHIJKLMNOPQR
TUVWXYZABCDEFGHIJKLMNOPQRS
UVWXYZABCDEFGHIJKLMNOPQRST
VWXYZABCDEFGHIJKLMNOPQRSTU
WXYZABCDEFGHIJKLMNOPQRSTUV
XYZABCDEFGHIJKLMNOPQRSTUVW
YZABCDEFGHIJKLMNOPQRSTUVWX
ZABCDEFGHIJKLMNOPQRSTUVWXY
```

Obviously, Piet wasn't going to win on size, but it seemed like a problem that was fairly doable in it,
and I'd been itching for an excuse to play with it anyway.

It took far longer than I had anticipated, partially because along the way I discovered and fixed
[a bug in the interpreter I was using](https://github.com/cincodenada/bertnase_npiet/commit/0701d07cbfb06c321293fb982ddae3f9805eccc5),
and added a few features to the [Piet IDE I was using](https://github.com/cincodenada/PietCreator/commits/master).
