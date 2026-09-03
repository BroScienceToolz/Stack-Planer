# Stack-Planer

Ein Rechenmodell, das dir ausrechnet, wie alt du wirst. Ungefaehr. Vermutlich. Wahrscheinlich nicht.

Eine einzige HTML-Datei, ca. 69 KB, laeuft im Browser, schickt nichts irgendwohin, speichert nichts, braucht kein Internet und keine Anmeldung. Doppelklick, fertig.

**➜ [Hier geht's direkt zum Rechner](https://BENUTZERNAME.github.io/stack-planer/)**

---

## Was hier liegt

| Datei | Was es ist |
|---|---|
| `index.html` | Die Webseite. Genau dieselbe Datei wie unten, nur unter dem Namen, den GitHub Pages braucht. |
| `stack-planer.html` | Die Webseite zum Herunterladen und Weitergeben. |
| `Stack-Planer_standalone.xlsx` | Dasselbe Modell als Excel-Mappe. Wer an den Parametern drehen will, macht es hier — im Blatt *Parameter* steht jede Stellschraube als Zelle, und der Planer rechnet sofort neu. |
| `Substanz-Matrix.xlsx` | Die Datengrundlage: alle 42 Substanzen mit ihren Faktoren auf die 16 Systeme, den Kopplungen und der Legende dazu. Das ist die Stelle, an der man dem Modell widersprechen kann. |

---

## Was das Ding macht

Du traegst ein, was laeuft: Testosteron-Load, Blast oder Cruise, wie lange schon, was du sonst noch nimmst. Dazu deine Blutwerte, soweit du sie hast. Unten stehen 42 Substanzen von Testosteron ueber Trenbolon und Insulin bis zu Statinen, Sartanen, Omega-3, Rauchen und Alkohol — jeweils mit zwei Schaltern: **laeuft** und **geplant**.

Oben stehen dann zwei Zahlen: das Alter, auf das du gerade zusteuerst, und das Alter, auf das du zusteuern wuerdest, wenn du die vorgeschlagenen Massnahmen umsetzt. Der Unterschied zwischen den beiden ist der eigentliche Punkt der Uebung.

### Die Kette reisst am schwaechsten Glied

Das Modell rechnet **16 Koerpersysteme einzeln** durch — Haematokrit, HDL, LDL, Triglyzeride, Lp(a), Blutdruck, Herzmuskel, Herzrhythmus, Gefaesse, Gefaesswand/Aorta/Lunge, Thrombose, Niere, Leber, Glukose, Aromatase/E2 und Psyche. Und zwar so, dass ein System am Anschlag nicht dadurch besser wird, dass die anderen fuenfzehn gruen sind.

Das ist der Unterschied zu dem ueblichen "ich addiere mal alle Risiken und teile durch die Anzahl". Ein hervorragendes LDL hilft deinem Herzmuskel genau gar nicht, wenn du Trenbolon, Clenbuterol und hGH gleichzeitig faehrst. Deine Blutfette sind dann trotzdem exzellent. Steht auch so auf dem Obduktionsbericht.

### Der Handlungsplan sortiert sich selbst

Abschnitt 3 rechnet fuer jede einzelne Massnahme aus, wie viele Lebensjahre sie dir konkret in **deiner** Konstellation bringt — nicht im Durchschnitt der Bevoelkerung. Wenn dein Haematokrit bei 57 steht, springt Aderlass nach oben. Wenn dein LDL bei 150 steht, springt das Statin nach oben. Was schon laeuft, wird nicht nochmal vorgeschlagen, und aus jeder Wirkstoffklasse kommt nur der Beste in die Top 3 — ACE-Hemmer *und* Sartan gleichzeitig zu empfehlen waere Unsinn, das eine ist die Alternative zum anderen.

Die Substanzliste unten sortiert sich beim Tippen mit: was am meisten bringt, steht oben, die Top 3 sind gruen, die drei am staerksten belasteten Systeme rot.

Jeder Abschnitt hat rechts oben einen Knopf, der genau ihn wieder leerraeumt — und einer raeumt alles. Zum Durchspielen von "was waere wenn" ist das schneller als die Seite neu zu laden.

### Die Grenzwerte sind absichtlich strenger als dein Laborbefund

Die vier Baender je Blutwert kennen die Leitlinien — Blutdruck ESC, Haematokrit Endocrine Society, LDL und Triglyzeride ESC/EAS und NCEP, Glukose ADA, Cystatin C ueber CKD-EPI auf die KDIGO-Stadien — aber sie uebernehmen deren Grenzen nicht ungeprueft. Und zwar aus zwei Gruenden.

Das oberste Band wird intern als „hier ist nichts mehr zu holen" verrechnet. Steht dort die Zahl, ab der ein Arzt einen Kranken behandeln wuerde, verschenkt das Modell die ganze Spanne darunter, in der es nachweislich noch besser wird. LDL 1,8 mmol/l ist kein Optimum, sondern eine Behandlungsschwelle; ein Neugeborenes hat rund 30 mg/dl, und eine untere Grenze, ab der das Risiko nicht mehr faellt, hat bis heute keine Studie gefunden. Dazu kommt der Zeitraum: das Ding rechnet vierzig Jahre nach vorn, und Werte wandern in dieser Zeit nach oben. Wer heute genau auf der Schwelle steht, steht in zehn Jahren darueber. „Gut" muss also Luft lassen.

Am anderen Ende dasselbe umgekehrt. Das oberste Band soll akuten Handlungsbedarf anzeigen, nicht bestaetigen, dass die Krankheit inzwischen diagnostizierbar ist. Ein Alarm, der auf die Diagnose wartet, ist keiner mehr — deshalb schlaegt der Blutdruck bei 140 an und nicht erst bei 160, die Glukose bei 110 und nicht bei 126, das LDL bei 130 und nicht bei 160.

In jedem Band steht die zweite Einheit in Klammern, damit niemand sein Blutbild im Kopf durch 38,67 teilen muss. Die offiziellen Leitlinienzahlen stehen jeweils im Hinweistext daneben, damit der Unterschied sichtbar bleibt.

### Der Rest ist Zinseszins

Der Schaden ist kumulativ und wird mit dem Alter teurer. Mit 40 kostet dich dasselbe Gramm mehr als mit 22 — die Regeneration wird langsamer, die Zeit bis zur Reparatur kuerzer. "Bis dass der Tod uns scheidet" als Dauer rechnet einfach hoch, bis das Budget alle ist. Das ist der Moment, in dem die Zahl oben aufhoert groesser zu werden.

---

## Benutzen

**Lokal:** Datei herunterladen, doppelklicken. Das war's. Kein Server, kein Build, kein `npm install`, keine 400 MB `node_modules` fuer eine Seite mit Schiebereglern.

**Im Netz:** laeuft bereits unter der Adresse ganz oben. Wer es selbst hosten will: Repo → Settings → Pages → Branch `main` → Save, zwei Minuten warten, fertig. Oder auf jeden beliebigen Webspace, jeden USB-Stick, in jedes Netzlaufwerk — es ist *eine Datei*.

**Auf dem Handy:** Am besten hosten und den Link oeffnen. Wenn du dir die Datei per Mail oder Messenger schickst und die Vorschau von iOS anguckst, siehst du zwar alle Auswahlfelder, aber keine Ergebnisse — die iOS-Vorschau fuehrt kein JavaScript aus. Ein rotes Kaestchen sagt dir das dann auch. Loesung: **In Safari oeffnen** oder eben hosten.

---

## Was das Modell nicht weiss

Ehrlichkeit vor Marketing:

**Es kennt keinen Krebs.** Es gibt keine Krebskategorie. Bei Rauchen und Alkohol — beide als eigene Substanzen drin, 10 Zigaretten bzw. 5 Bier am Tag — ist der angesetzte Schaden deshalb eher zu freundlich als zu hart.

**Es kennt dich nicht.** Es kennt Populationsdurchschnitte und die Zahlen, die du eintraegst. Wo du nichts eintraegst, nimmt es einen bevoelkerungstypischen Standardwert an. Je mehr echte Blutwerte drinstehen, desto weniger raet es. Ein gemessener Wert zaehlt deutlich schwerer als jede Schaetzung — das ist Absicht.

**Es kennt keine Genetik.** Der Stack-Planer hier ist die genetikfreie Fassung. Es gibt eine zweite, die eine DNA-Rohdatendatei auswertet und daraus eine genetische Veranlagung je System schaetzt — die ist ein eigenes Werkzeug und liegt aus gutem Grund nicht in einem oeffentlichen Repo.

**Es ist ein Modell.** Kein Orakel, kein Ersatz fuer Blutbild, Echo, Belastungs-EKG oder einen Arzt, der dich anguckt. Es macht das, was Modelle machen: es macht Groessenordnungen und Rangfolgen sichtbar. Ob es dir *48,3* oder *47,9* Jahre ansagt, ist Rauschen. Ob es dir 62 oder 81 ansagt, ist eine Ansage.

Die Rechnung selbst wurde gegen zwei unabhaengige Implementierungen geprueft (Excel-Formeln und eine separate Python-Referenz) und stimmt auf vier Nachkommastellen ueberein. Das heisst: die Arithmetik ist sauber. Ob die *Annahmen* stimmen, ist eine voellig andere Frage, und die beantwortet keine Testsuite der Welt.

---

## Datenschutz

Es gibt keinen. Weil es nichts zu schuetzen gibt.

Kein Server, keine Requests, kein Tracking, kein `localStorage`, keine Cookies, keine Analytics, keine Schriftart von einem CDN. Alles bleibt in dem Tab, in dem du es eingetippt hast, und ist weg, sobald du ihn schliesst. Du kannst das WLAN ausschalten und weiterrechnen. Du kannst auch in den Quelltext gucken — es ist *eine* Datei, da versteckt sich nichts.

Der Nachteil: Es gibt keinen Speichern-Knopf. Feature, kein Bug.

---

## Disclaimer

> **Keine Therapieempfehlung. Ein Rechenmodell zu Unterhaltungszwecken. Die Einnahme von den aufgefuehrten Substanzen muss in Absprache mit Aerzten und erfahrenen Coaches erfolgen.**

Etwas ausfuehrlicher, fuer alle, die den Kasten oben ueberlesen haben:

Diese Software gibt **keine medizinische Beratung**. Sie diagnostiziert nichts, sie behandelt nichts, sie ersetzt niemanden mit Approbation. Dass hier Substanzen aufgelistet sind, ist keine Empfehlung, sie zu nehmen — auch die Statine nicht, und die verschreibungspflichtigen erst recht nicht. Verschreibungspflichtig heisst verschreibungspflichtig.

Die angezeigten Zahlen sind **Modellergebnisse, keine Prognosen**. Niemand kann dir dein Sterbealter ausrechnen, und diese Datei kann es auch nicht. Sie kann dir zeigen, welches System in deiner Aufstellung das schwaechste Glied ist. Das ist schon ziemlich viel, aber es ist eben nicht dasselbe.

Setz nichts ab, setz nichts an und dosier nichts um, weil eine HTML-Datei dir eine Zahl gezeigt hat. Geh damit zu jemandem, der dir Blut abnehmen kann.

Benutzung auf eigenes Risiko. Keine Gewaehr, keine Haftung, kein Support-Ticket. Wenn dir dieses Werkzeug zeigt, dass du in Schwierigkeiten steckst, dann ist der naechste Schritt ein Termin und kein weiterer Klick.

---

## Kontakt

Fragen, Fehler, Widerspruch zu einem Faktor in der Matrix: **BroScienceToolz@gmail.com**

Widerspruch ist ausdruecklich willkommen. Jede Zahl in `Substanz-Matrix.xlsx` ist eine Schaetzung aus Studienlage plus Erfahrung, und ein paar davon sind bestimmt daneben. Wer eine bessere Zahl hat und sagen kann, woher sie kommt, bekommt sie eingebaut.

---

## Lizenz

MIT — siehe [LICENSE](LICENSE). Nimm's, aendere es, hoste es, bau was Besseres draus. Nur behaupte bitte nicht, es sei ein Medizinprodukt.
