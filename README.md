# Lern-Bericht-Numberguesser
Marku

## Einleitung

Ich habe ein Numberguesser Spiel programmiert, indem man nur Zahlen zwischen 1 und 100 generiert.

## Was habe ich gelernt?

Ich habe gelernt wie man die try und catch funktionen anwendet.

## Beschreibung
Man verwendet die try und catch Funktion, um Fehler abzufangen. Man definiert, was eine gültige/ungültige Eingabe ist. Die try Funktion wird verwendet, wenn die Eingabe gültig ist. Das Spiel geht dann wie geplant weiter. Wenn aber eine ungültige Eingabe eingegeben wird, wird die catch Funktion verwendet. Diese Funktion versucht, den Abbruch des Programmes umzugehen. Dem Spieler wird dann noch eine Chance gegeben, eine gültige Eingabe zu machen.

<img width="675" alt="image" src="https://user-images.githubusercontent.com/110892575/189845043-6b8d8c0c-62c6-465e-b715-aff891bf2094.png">
Dieses Bild zeigt eine Demonstration einer ungültigen Eingabe.

```
 try
                    {
                        Console.Clear();
                        Console.WriteLine("                                                   The Numberguesser");
                        double ZufalsZahl = Convert.ToDouble(new Random().Next(1, 100));
                        Console.WriteLine("Geben sie eine zufällige Zahl zwischen 1 und 100 ein");
                        double eingabe = Convert.ToDouble(Console.ReadLine());
                        while (eingabe != ZufalsZahl)
                        {

                            if (eingabe > ZufalsZahl)
                            {
                                Console.WriteLine("Die Zufalszahl ist kleiner als ihre eingabe");
                            }
                            else
                            {
                                Console.WriteLine("Die Zufallszahl ist grösser als ihre eingabe");
                            }
                            Console.WriteLine("Geben sie eine neue Zahl ein");
                            eingabe = Convert.ToDouble(Console.ReadLine());
                            versuche++;
                        }


                        Console.WriteLine("Du hast die Zahl erratten");
                        Console.WriteLine("Versuche gebraucht um die Zahl zu eratten" +
                            "" +
                            "" +
                            ": " + versuche);

                        Console.WriteLine("Willst du nochmals Spielen?(Ja/Nein)");
                        Restart = Console.ReadLine();

                        if (Restart == "Ja")
                        {
                            Console.WriteLine("Geben sie eine neue Zahl ein");
                        }

                        if (Restart == "Nein")
                        {
                            Console.WriteLine("Schade!");
                        }

                    }
                    catch
                    {
                        Console.WriteLine("Deine Eigabe ist ungültig");
                        Console.WriteLine("Willst du nochmals spielen?(Ja/Nein)");
                        Restart = Console.ReadLine();
                        if (Restart == "Ja")
                        {
                            Console.WriteLine("Geben sie eine neue Zahl ein");
                        }

                        if (Restart == "Nein")
                        {
                            Console.WriteLine("Schade!");
                        }

                    }

```
Die Funktion try überprüft, ob eine gültige Eingabe eingegeben wurde (Zahl von 1 bis 100), wenn nicht, wird die catch Funktion hervorgerufen. In der catch Funktion wird dem Spieler gesagt, dass seine Eingabe ungültig ist. Daraufhin wird der Spieler gefragt, ob er noch eine Zahl eingeben möchte.

## Verifikation
*Mein Text ist eine kurze Zusammenfassung, welches beschreibt, was eine try und catch Funktion überhaupt ist.
*Mein Bild zeigt wie mein Programm reagiert, wenn eine ungültige Eingabe eingegeben wird
*Mein Code zeigt, wie ich die try und catch Funktion angewendet habe.

# Reflektion zum Arbeitsprozess
*Ich habe während meines Projektes meine Pausen sehr gut eingeplant.
*Ich habe mich nicht ablenken lassen und habe konstruktiv gearbeitet.
*Ich habe meine Ziele für dieses Projekt erreicht.
 
*Ich habe meine Arbeitspakete für mein Projekt nicht gut geplannt.

**VBV**: Ich kann jetzt besser einschätzen, wie lange ich brauche für die verschiedenen Arbeitspakete und werde sie nächstes Mal besser einplanen.
