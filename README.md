# Game-UI-concept-and-logic
Projekt-Einblick: UI/UX-Design und Logik-Architektur

Dies ist eine Übersicht meines methodischen Ansatzes und zeigt die Gedankengänge, wie ich das Interface schrittweise verbessere und benutzerfreundlicher gestalte.

# Menu Concept 1.0
Die erste Idee des Menüs.

<img width="442" height="264" alt="Screenshot 2026-10-12 121706" src="https://github.com/user-attachments/assets/1dd0a127-6e48-4cd8-b27b-d0879190f8c9" />

Schwachstellen:
1. Die Menüpunkte sind weit voneinander entfernt. Das Auge braucht zu lange zum Suchen und die Navigation dauert unnötig lange.
2. Die Schriftart ist schwer lesbar.

Fazit: Das Menü muss so gestaltet werden, dass der User das Menü deutlich schneller und intuitiver bedienen kann.

# Menu Conept 1.1

<img width="240" height="306" alt="Screenshot 2026-10-12 121720" src="https://github.com/user-attachments/assets/a6145057-1941-4a5f-b6df-e812892ce96f" />

Neues Konzept und Optimierungen:
1. Die Buttons sind nun untereinander angeordnet. Dies ermöglicht eine angenehmere Tastatur-/Gamepad- Steuerung (hoch/runter) und fokussiert den Blick.
2. Einstellungen wie „Sprache“ und „Steuerung“ wurden im Menüpunkt „Settings“ zusammengefasst, um das Menü übersichtlicher zu gestalten.
3. Das Bild wurde an die Seite gerückt, um nicht von den Menüpunkten abzulenken. Falls es den Spielfluss weiterhin stört (wird getestet), wird es im finalen Design komplett entfernt.
4. Einsatz einer lesbaren Schriftart, die den visuellen Stil des Spiels beibehält.

# Menu Concept 1.2 (final)

<img width="688" height="1062" alt="Illustration" src="https://github.com/user-attachments/assets/01c17dfa-3e9a-4712-ab4c-8a94cd36a575" />

Finale Version:
1. Einsatz von Icons: Jeder Menüpunkt besitzt ein passendes, leicht verständliches Icon. Das hilft Spielern, Inhalte visuell schnell zu erfassen.
2. Vertikale Anordnung: Die Buttons sind übersichtlich in einer vertikalen Liste angeordnet, was eine natürliche und flüssige Blickführung garantiert.
3. Font: Für eine bessere Lesbarkeit wurde die Schriftart komplett ausgetauscht.
4. Charakter-Integration: Das kleine Charakter-Bild oberhalb des Menükastens ist visuell ansprechend, ohne dabei von den funktionalen Elementen abzulenken.
5. Reduzierung von Klicks: Wichtige Aktionen sind direkt erreichbar, was den Weg zum gewünschten Ziel verkürzt. Load Save File, Language und Controls sollen nicht tief in den allgemeinen Einstellungen verschwinden.
   + Barrierefreiheit: Wenn der Spieler versehentlich die falsche Sprache auswählt, dann ist es extrem schwierig durch ein verschachteltes Settings-Menü zu navigieren.
   + Steuerung: Am Anfang eines Spiels schauen Spieler mehrfach in die Steuerung, um Tastenbelegung zu überprüfen. Ein direkter Zugriff spart hier unnötige Unterbrechungen.
  
# Spiellogik & Event-Steuerung

<img width="744" height="246" alt="Screenshot 2026-10-12 121734" src="https://github.com/user-attachments/assets/7affc9ec-9619-4be0-befb-45dda84a45b6" />

1. Interaktions-Zähler:
Nutzung von Variablen als Zähler, um Spielerinteraktionen mit der Spielwelt zu verfolgen.
• Beim Interagieren mit dem NPC erhöht sich die Variable.

Ergebnis: Das Event reagiert dynamisch auf das Verhalten des Spielers und sperrt weitere
Aktionen (hier: Maximalanzahl an Bestellungen erreicht).

2. Lokalisierung: Globale Zustandsvariable zur dynamischen Sprachumschaltung:
• Language = 1 → Englisch
• Language = 2 → Deutsch

Ergebnis: Sämtliche Dialoge und Textelemente passen sich anhand des gewählten Werts
automatisch an die bevorzugte Sprache des Nutzers an.

# Zustands-Steuerung via Booleans

<img width="918" height="118" alt="Screenshot 2026-10-12 121751" src="https://github.com/user-attachments/assets/c1714a14-0261-44b5-811b-43404fba465e" />

1. Nutzung von Schaltern (Booleans : True / False, in der Engine 'Ein/Aus') zur Ereignis-Steuerung. Wenn beispielsweise ein Schlüssel (trash key) aktiv ist, werden neue
Interaktionen freigeschaltet und Menü-Steuerungen angepasst (Menu Control = AUS →
Menüaufruf wird blockiert, wenn dieses Event aktiv ist)
2. Einsatz von Community-Plugins, um Standard-Funktionen der Engine gezielt zu erweitern
und anzupassen.

# Projekt-Evolution: Von Spiel 1 zu Spiel 2
Anstatt die Spiele nur einzeln vorzustellen, zeigt dieser Vergleich direkt, wie sich meine Fähigkeiten
weiterentwickelt haben.

<img width="751" height="500" alt="Screenshot 2026-10-12 131925" src="https://github.com/user-attachments/assets/6700a7ac-06df-4adc-a611-2c6660608dbc" />

Am Ende zählt für mich der Fortschritt. Mehr Routine bedeutet für mich mehr Mut zu neuen Ideen
und spürbar mehr Vielfalt im Gameplay.
