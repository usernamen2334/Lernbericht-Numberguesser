# Lern-Bericht-Numberguesser
Marku

## Einleitung

Ich habe ein Numberguesser Spiel programmiert, indem man nur Zahlen zwischen 1 und 100 generiert.

## Was habe ich gelernt?

Ich habe gelernt wie man die Try und catch funktionen anwendet.

## Beschreibung

✍️ Verwenden Sie drei verschiedene Medien, um zu zeigen, was Sie gelernt haben. Zum Beispiel:
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

<img width="675" alt="image" src="https://user-images.githubusercontent.com/110892575/189845043-6b8d8c0c-62c6-465e-b715-aff891bf2094.png">
Dieses Bild zeigt eine Demonstration einer Fehlereingabe.



## Verifikation

✍️ Erklären Sie kurz und bündig, inwiefern die von Ihnen verwendeten Medien zeigen, was Sie gelernt haben.

# Reflektion zum Arbeitsprozess

👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief; 

👎 und etwas, was nicht gut lief.

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.
