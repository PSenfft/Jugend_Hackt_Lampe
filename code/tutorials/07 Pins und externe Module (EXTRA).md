# Pins und externe Module

> **Voraussetzung:** Du kennst die Grundlagen bei der Programmierung mit dem Adafruit Playground Board.

> **Ziel** hier ist, dass du am Ende einen Einstieg zur Benutzung der Pins deines Boards hast und dein erstes externes Modul angeschlossen hast.

## Tutorial

> **Was wollen wir machen?** Wir möchten eine externe LED anschließen, damit wir ein stärkeres Licht erzeugen können.

### Material

1. Dein Adafruit Playground Board
2. Das "Keyes LED" Modul
3. 3 Kabel mit jeweils einem female Header
4. 3 Schrauben mit jeweils einer Mutter um die Kabel auf das Board zu klemmen

### Verkabelung

![Verkabelung](./images/07%20Pins%20und%20externe%20Module/verkabelung.png)

#### **Pinbelegung**

Pin auf Board | Pin auf Modul
:------- | -------:
VOUT | +
GROUND | GROUND
SDA | S

### Programm

![Programm Code](./images/07%20Pins%20und%20externe%20Module/programm.png)

#### **Erklärung**

1. **Beim Start**

    > Die Variablen bekommen alle einen Standardwert.

2. **wenn Knopf B geklickt**

    > Wenn die LEDs an sind, wird die Farbe gewechselt.

3. **wenn Knopf A geklickt**

    > Macht die LEDs aus und an.
    > Setzt auch den SDA Pin auf LOW oder HIGH. (Aktiviert oder deaktiviert die externe LED)

### Ergebnis

![LED AN](./images/07%20Pins%20und%20externe%20Module/led_module_on.png)
