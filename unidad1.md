

Voy a documentar mi primer código de strudel
Solo intente ver que Pasaba si inscribia algo random

``` js
setcpm(24.5)

let drum = stack(
  s("oh:1").beat("0,1,2,4,5,7,10,12,14",16),
  s("hh").beat("0,2,4,8,9,11,13,15",16),
  s("cp").beat("0,1,2,5,8,9,12,14",16),
  s("bd").beat("0,4,5,7,10,13",16),
).bank("RolandTr909");


$drum: drum
```

¿Qué es un stack? 
¿Esto realmente cómo funciona?
stecpm son los ciclos por minuto que determina el timing
----------------------------------------------------------------------------------------------------------
Intente hacer "Aris of the soul" pero no me salio, igual esta bien

``` js
setcpm(15)
let melody = note("[[e4,a4] [c4][d4][g4][e4][c4][d4][g4][e4][c4][d4][g4][e4][a4][c4]]").sound("piano").legato(1);
$melody: melo
```
------------------------------------------------------------------------------------------------------------
Ok,intente un buen tiempo pero después de muchos intentos y que el net no cooperara no cree la canción que queria pero con mis intentos fallidos y curiosidad cre esto que me quedo gustando.
``` js
setcpm(15)


$: note(`[
  [eb2,eb3]  [gb3,bb3,eb4] [db2,db3] [f3,ab3,db4]
  [eb2,eb3] [gb3,bb3,eb4] [db2,db3] [f3,ab3,db4]
  [eb2,gb3,bb3,eb4] eb5 [db2,f3,ab3,db4] db5
  [eb2,gb3,bb3,eb4] bb4 [db2,f3,ab3,db4]
  [eb2,gb3,bb3,eb4] gb5 [db2,f3,ab3,db4] f5
  [eb2,gb3,bb3,eb4] eb5 [db2,f3,ab3,db4]
  [cb2,eb3,gb3,cb4] cb5 [bb1,d3,f3,bb3] bb4
  [cb2,eb3,gb3,cb4] ab4 [bb1,d3,f3,bb3] g4
  [ab1,c3,eb3,ab3] [c5,eb5] [bb1,d3,f3,bb3] [d5,f5]
  [eb2,gb3,bb3,eb4] eb5 [db2,f3,ab3,db4] db5
  [eb2,gb3,bb3,eb4] bb4 [db2,f3,ab3,db4]
]`)
  .s("piano")
  .legato(1)
  .slow(2.3) 


$: stack(
  s("oh:1").beat("0,1,2,4,5,7,10,12,14",16),
  s("hh").beat("0,2,4,8,9,11,13,15",16),
  s("cp").beat("0,1,2,5,8,9,12,14",16),
  s("bd").beat("0,4,5,7,10,13",16)
).bank("RolandTr909")
  .gain(0.6)


$: chord("E@4 F@4 Am@4 Am@4")
  .voicing()
  .s("gm_epiano1")
  .gain(0.8)


$: note("<[f3,g3,a4,c4] [a3,c3,d4,b4] [ed,b3,b2,a4] [g3,e4,g4,e4]>")
  .sound("piano")
  .attack(0.6)
  .lpf(859.3)
  .room(2)
  .gain(0.6)
```
