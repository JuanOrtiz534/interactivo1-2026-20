

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
