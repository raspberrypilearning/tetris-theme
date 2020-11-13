## Programar el inicio

Ahora vamos a programar la primera parte de la melodía en Sonic Pi.

+ Primero vamos a elegir una velocidad y un sintetizador para la música. La velocidad normal es de 60 pulsaciones por minuto (bpm), pero eso no es lo suficientemente rápido para esta pieza.
    
    Elige un buffer vacío en Sonic Pi y añade este código:
    
    ![captura de pantalla](images/tetris-setup.png)

+ Aquí está el primer compás de Korobeiniki:
    
    ![captura de pantalla](images/tetris-notes1.png)
    
    El nombre de la nota se muestra abajo en rojo y la longitud de la nota arriba en verde.
    
    Las notas musicales tiene nombres de letras de la A-G. Para obtener más notas repite las letras para obtener más octavas (rangos de notas superiores o inferiores.) Cada octava comienza en C.
    
    En Sonic Pi el valor por defecto es la octava 4, b3 significa b de la octava debajo.
    
    Sonic Pi te permite usar nombres de letras en lugar de números. Esto es útil cuando estás trabajando con notación musical.
    
    Programa las primeras 3 notas de Korobeiniki en Sonic Pi:
    
    ![captura de pantalla](images/tetris-start.png)

+ Eso funciona, pero se necesita mucho tecleo. Hay una manera más corta de programar melodías más largas: `play_pattern`.
    
    `play_pattern` te permite programar múltiples notas en una línea.
    
    Reemplaza tu código para usar `play_pattern` para reproducir el primer compás:
    
    ![captura de pantalla](images/tetris-pattern.png)

+ Es posible que hayas notado que las notas no tienen la misma longitud. Está bien, si cambias `play_pattern` a `play_pattern_timed` entonces puedes decir cuánto dura cada nota.
    
    Los números en verde muestran cuántos tiempos dura cada nota.
    
    ![captura de pantalla](images/tetris-notes1.png)
    
    (Si lees música, esta pieza está en un compás de 4/4 y una negra dura un tiempo, una corchea dura la mitad de un tiempo y una blanca dura dos tiempos)
    
    `play_pattern_timed` toma una lista de notas y luego una lista de tiempos.
    
    Cambia tu código `play_pattern` para que se vea así:
    
    ![captura de pantalla](images/tetris-timed.png)

+ Si no le das suficientes tiempos, Sonic Pi los repetirá. Este compás repite el tiempo `1, 0.5, 0.5` (negra, corchea, corchea) para que puedas cambiar tu código a:
    
    ![captura de pantalla](images/tetris-timed2.png)

+ Añade el siguiente compás de música, el tiempo es el mismo para este compás.
    
    ![captura de pantalla](images/tetris-notes2.png)
    
    ![captura de pantalla](images/tetris-bar2.png)
    
    <div id="audio-preview" class="pdf-hidden">
      <audio controls preload> 
       <source src="resources/tetris-1.mp3" type="audio/mpeg"> Tu navegador no es compatible con el elemento <code>audio</code>. 
      </audio>
    </div>

¿La melodía empieza a sonar familiar?