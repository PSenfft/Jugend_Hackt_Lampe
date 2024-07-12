# Mein erstes Programm 2

> **Voraussetzung**: In dieser Anleitung lernst du, wie du dein Taschenlampenprogramm aus [03 Mein erstes Programm](./03%20Mein%20erstes%20Programm.pdf) erweitern kannst. Daher solltest du dieses natürlich bereits schon haben!

</br>

> **Ziel**: Weitere Prinzipien des Programmierens kennen lernen.

## Anleitung

> Vielleicht dachtest du schon beim Programmieren der Taschenlampe, dass normale Taschenlampen nur einen Knopf haben anstatt zwei. Bei einer herkömmlichen Taschenlampe schaltet der selbe Schalter die Lampe(n) an und aus. Genau das setzen wir nun in deinem Taschenlampenprogramm um:

</br>

> **Überlegung:** Unser Programm muss sich nun verändern. Zunächst darf nur ein Taster verwendet werden. Das Programm muss sich auch merken, ob die LEDs an oder aus sind, und sich entsprechend verhalten.

### 1. Variablen

> Um sich zu merken, ob die LEDs an sind, benötigen wir eine sogenannte "Variable". In Variablen können wir unsere Daten speichern, wie zum Beispiel den Status unserer LEDs.

1. Erstellen einer Variable: Klicke in deiner Entwicklungsumgebung auf das "Variablen" Menu und dann auf "Erstelle eine Variable".

    ![new_variable](./images/05%20Mein%20erstes%20Programm%202/neue_variable.png)

2. Danach öffnet sich ein Menu, um unserer Variable einen Namen zu geben. Da wir damit den Status unserer LEDs speichern wollen, nennen wir sie "Licht" und drücken auf "OK".

    ![variable_name](./images/05%20Mein%20erstes%20Programm%202/neue_variable_name.png)

> Perfekt! Du hast deine erste Variable erstellt!

### 2. Logik

> Damit jetzt unsere Variable zum Einsatz kommen kann, brauchen wir Logik! Wir bauen Logik in unser Programm ein, damit es sich "Verzweigen" kann. Mit "Verzweigen" ist gemeint, dass unser Programm unterschiedliche Dinge unter unterschiedlichen Umständen tut. In unserem Fall ist es der Status der Variable aus Schritt 1 "Licht". Ist das Licht an, soll das Programm beim nächsten Knopfdruck diese ausschalten und anders herum!

1. Zuerst müssen wir alte Funktionen entfernen: Lösche also den "setze alle Pixel auf rot" Block aus dem "wenn Knopf A geklickt" Block. Das tust du, indem du mit rechter Maustaste auf ihn drückst und danach mit der linken Maustaste die Option "Block löschen" auswählst.

    ![delete_block](./images/05%20Mein%20erstes%20Programm%202/led_on_delete.png)

2. Fügen wir nun an der Stelle einen Logik-Block hinzu! Dazu wählst du unter dem Logik-Menu den zweiten Block aus. Dieser ist mit "wenn wahr dann ... ansonsten" beschriftet. Danach ziehst du ihn in den "wenn Knopf A geklickt" Block.

    ![if_else_block](./images/05%20Mein%20erstes%20Programm%202/if_else_block.png)

    ![if_else_in_button_a](./images/05%20Mein%20erstes%20Programm%202/if_else_block_button_a.png)

> Dieser Block macht so ziemlich genau das, was auf ihm steht. Wenn eine Variable "wahr" ist führt er dass aus, was im oberen Teil des Blockes hinzugefügt wurde, ansonsten führt er den unteren Teil aus (die Variable hat den Wert "falsch").
In unserem Fall wollen wir also wenn das Licht an ist es ausschalten, und es anschalten, wenn es ausgeschaltet ist.

</br>

> **Wichtig:** Gerade steht noch "wahr" als Variable in unserem Logikblock. Das führt dazu, dass nur der erste Blockteil ausgeführt werden würde.

### 3. Kombinieren

1. Anstatt "wahr" fügen wir jetzt unsere "Licht" Variable ein, um unseren Logik-Block abhängig von dieser zu machen. Das machst du, indem du unter "Variablen" den ovalen "Licht" Block an die Stelle von "wahr" ziehst.

    ![light_bool_var](./images/05%20Mein%20erstes%20Programm%202/licht_var.png)

2. Fügen wir nun unsere Funktionen hinzu: Wenn das Licht an ist, wollen wir es ausschalten, wenn es ausgeschaltet ist, wollen wir es anschalten:

    ![logic_1](./images/05%20Mein%20erstes%20Programm%202/logik_without_var_update.png)

> **Ausprobieren:** Starte den Simulator und steuere deine Taschenlampen nur über den A-Knopf.

</br>

> **Beobachtung:** Die Taschenlampe geht zwar an, aber jedoch nicht aus. Das liegt daran, dass der Wert deiner "Licht" Variable immer auf "falsch" bleibt und immer der zweite Block in deinem Logik-Block ausgeführt wird.

### 4. Variablenwerte ändern

1. Damit unsere Taschenlampe korrekt funktioniert, musst du den Wert der "Licht" Variable ändern. Das tust du, indem du den Block "setze Licht auf 0" zwei Mal in deinen Logik-Block einfügst. Du findest diesen Block im "Variablen" Menu.

    ![change_var](./images/05%20Mein%20erstes%20Programm%202/change_var.png)

2. Jedoch soll der Wert nicht auf "0" geändert werden, sondern auf "wahr" oder "falsch". Dafür benötigen wir die diamantförmigen Wahr- und Falsch-Blöcke aus dem Logik-Menu.

    ![change_var_bool](./images/05%20Mein%20erstes%20Programm%202/change_var_bool.png)

> **Ausprobieren:** Starte den Simulator und steuere deine Taschenlampen nur über den A-Knopf.

</br>

> **Fertig:** Deine Taschenlampe sollte nun alleine über den A-Knopf steuerbar sein. (Falls nicht, vergleiche dein Code mit dem letzten Bild.)

Weiter geht es nun mit "Ideen und Aufgaben" Teil, in dem du für dein eigenes Projekt Inspiration und Ideen sammeln kannst: [Nächster Schritt](./06%20Ideen%20und%20Aufgaben.pdf)
