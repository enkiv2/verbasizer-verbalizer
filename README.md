# verbasizer-verbalizer
Column-based cutups with speech synthesis

Based on descriptions of David Bowie's "verbasizer" script, which he used in generating the lyrics for Outside.

Verbasizer reads text from stdin, and cuts it into *n* columns (by default, 5; the first arg to the script overrides this). It then reorders the contents of each column randomly and pastes the columns back together.

The verbalizer script is a helper for picking a speech synthesizer (out of several common ones for unix-like systems). The verbasizer-verbalizer script composes these two programs.

Sample usage:

```
$ echo "No live organism can continue for long to exist sanely under conditions of absolute reality; even larks and katydids are supposed, by some, to dream. Hill House, not sane, stood by itself against its hills, holding darkness within; it had stood for eighty years and might stand for eighty more. Within, walls continued upright, bricks met neatly, floors were firm, and doors were sensibly shut; silence lay steadily against the wood and stone of Hill House, and whatever walked there, walked alone." | ./verbasizer

 and of  had shut conditions
 eighty steadily  might continued upright
 walked itself  sanely larks to
 long absolute  even under stood
 eighty met  the were for
 darkness more  can hills whatever
 bricks doors  its some silence
 by to  alone wood for
 No there  House continue and
 dream Hill  sensibly stand for
 of within  by sane and
 katydids live  walls stood firm
 stone are  not and holding
 lay years  floors  

$ echo "No live organism can continue for long to exist sanely under conditions of absolute reality; even larks and katydids are supposed, by some, to dream. Hill House, not sane, stood by itself against its hills, holding darkness within; it had stood for eighty years and might stand for eighty more. Within, walls continued upright, bricks met neatly, floors were firm, and doors were sensibly shut; silence lay steadily against the wood and stone of Hill House, and whatever walked there, walked alone." | ./verbasizer 3

 dream by  are
 continue whatever  and
 No silence  there
 sane absolute  can
 larks for  years
 neatly might  firm
 walked of  even
 darkness more  holding
 stood stood  steadily
 supposed alone  met
 against sanely  not
 of Hill  walls
 and and  to
 exist upright  House
 and doors  conditions
 continued within  itself
 against live  sensibly
 shut floors  for
 and for  to
 stone its  had
 eighty the  
```
