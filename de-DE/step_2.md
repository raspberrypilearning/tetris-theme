## Code den Anfang

Lassen Sie uns nun den ersten Teil des Songs in Sonic Pi codieren.

+ Zuerst wählen wir eine Geschwindigkeit und einen Synth für die Musik. Die normale Geschwindigkeit beträgt 60 Schläge pro Minute (BPM), aber das ist für dieses Stück nicht schnell genug.
    
    Wählen Sie einen leeren Puffer in Sonic Pi und geben Sie diesen Code ein:
    
    ![Screenshot](images/tetris-setup.png)

+ Hier ist die erste Bar von Korobeiniki:
    
    ![screenshot](images/tetris-notes1.png)
    
    Es zeigt den Namen der Note unten in rot und die Länge der Note oben in Grün.
    
    Noten haben Buchstaben von AG. Um mehr Noten zu erhalten, wiederholen Sie die Buchstaben, um mehr Oktaven (Bereiche mit höheren oder niedrigeren Noten) zu erhalten.
    
    In Sonic Pi ist der Standardwert die Oktave 4, b3 bedeutet b aus der darunterliegenden Oktave.
    
    Mit Sonic Pi können Sie Buchstabennamen anstelle von Zahlen verwenden. Dies ist nützlich, wenn Sie mit Notationen arbeiten.
    
    Codiere die ersten 3 Noten von Korobeiniki in Sonic Pi:
    
    ![Screenshot](images/tetris-start.png)

+ Das funktioniert, aber man muss ziemlich viel tippen. Es gibt eine kürzere Möglichkeit, längere Titel zu programmieren: `play_pattern`.
    
    `play_pattern` können Sie mehrere Noten in einer Zeile programmieren.
    
    Ersetzen Sie Ihren Code, um `play_pattern` zu verwenden, um den ersten Takt zu spielen:
    
    ![Screenshot](images/tetris-pattern.png)

+ Sie haben vielleicht bemerkt, dass die Notizen nicht alle gleich lang sind. Wenn Sie `play_pattern` in `play_pattern_timed` ändern, können Sie sagen, wie lange jede Note dauert.
    
    Die Zahlen in Grün zeigen viele Schläge, die jede Note hält.
    
    ![Screenshot](images/tetris-notes1.png)
    
    (Wenn Sie Musik lesen, ist dieses Stück im 4/4-Takt und ein Schritt dauert einen Takt, ein Achtel dauert einen halben Takt und ein Minimum dauert zwei Taktschläge.)
    
    `play_pattern_timed` nimmt eine Liste von Notizen und dann eine Liste von Zeiten.
    
    Ändern Sie Ihren `play_pattern` Code wie folgt:
    
    ![Screenshot](images/tetris-timed.png)

+ Wenn Sie nicht genug Zeit geben, wiederholt Sonic Pi sie. Dieser Balken wiederholt das Timing `1, 0,5, 0,5` (Schrittzange, Quaver, Quaver), sodass Sie Ihren Code folgendermaßen ändern können:
    
    ![screenshot](images/tetris-timed2.png)

+ Fügen Sie den nächsten Takt hinzu, das Timing ist für diesen Takt gleich.
    
    ![Screenshot](images/tetris-notes2.png)
    
    ![Screenshot](images/tetris-bar2.png)
    
    <div id="audio-preview" class="pdf-hidden">
      <audio controls preload> <source src="resources/tetris-1.mp3" type="audio/mpeg"> Ihr Browser unterstützt das <code>Audio-</code> Element nicht. </audio>
    </div>

Beginnt die Melodie vertraut zu sein?