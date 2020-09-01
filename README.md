<h1>
    Veliz password Encrypt
</h1>

<h3>
    Paul Guadalupe veliz López
</h3>
<hr>
<b>1. Obtenemos la contraseña y la convertimos a mayúsculas.</b><br>

<i>Ej: QWERTY</i><br>

<b>
    2. Tomamos la length de la contraseña.
</b><br>

<i>Ej: 6</i> <br>

<b>3. Tomamos cada letra y extraemos el código ASCII (hexadecimal) de cada una.</b><br>

<i>Ej: Q = 81, W = 87, E = 69, R = 82, T = 84, Y = 89</i> <br>

<b>
    4. Multiplicamos la length por cada letra en ASCII. (Cada resultado de cada
    multiplicación se concatenará con la siguiente).
</b> <br>
<i>Ej: 6 x 81, 6 x 87, 6 x 69 …</i> <br>
<b>5. Al resultado se le añadirá un (*) al inicio.</b> <br>
<i>Ej: *481 522 414 492 504 534 (Sin espacios).</i> <br>

<b>
    6. A cada resultado concatenado se va a convertir a hexadecimal. (Se
    concatenará cada resultado al igual que el procedimiento anterior).
</b> <br>
<i>Ej: 481 = 30, 522 = 34 …</i> <br>
<b>Ultimo paso:</b> <br>
<i>
    ● Si el resultado final sobrepasa la length de 32 se recortará hasta
    tenerla en 32.
</i> <br>
<b>Resultado final:</b> <br>
<b>Antes:</b> <br> QWERTY <br>
<b>Después:</b> <br> *303404313235