# Bekannte Bugs

**Hauptspiel:**

- Die vier neuen Produkte (Biokost, Sushi, Nahrungspacks und Thermalhüllen) können nicht auf dem Weltmarkt gehandelt werden.
- Es gibt fünf Quests, die euch anleiten, bestimmte Forschungen durchzuführen, um bestimmte Gebäude freizuschalten, da der Tooltip "Bedingung freischalten" nur mit Bevölkerungsmeilensteinen funktioniert. Leider werden diese Quests in allen Sessions sichtbar sein, nicht nur in denen, in denen sich die Gebäude befinden.
- Bestimmte Sekundärmodul-Tooltips zeigen nicht die korrekte Tooltip-Beschreibung an (z.B. Energiemodul auf Energieproduktionsgebäuden, die +15% Output geben, oder Mars-Forschungslabor-Module)
- Der Bevölkerungsübersichtsfilter in der strategischen Ansicht funktioniert nicht richtig mit der neuen Arktis Stufe 3. Es wird nicht das richtige Porträt neben der Zahl angezeigt. Dasselbe gilt für die Marssynthetiks.
- Dienstleistungen sind ein neues "Produkt". Der Bestand kann nicht im "normalen" Bestandsmenü angezeigt werden, sonst wären sie über Handelsrouten handelbar. Stattdessen findet man sie in der Baustoffleiste oben oder man klickt auf ein beliebiges öffentliches Gebäude und fährt mit dem Mauszeiger über das "Globus"-Symbol, um die aktuelle Sektorbilanz zu sehen.
- Der Infotipp "Firmensitz" am unteren Bildschirmrand scheint hardgecoded zu sein und zeigt öffentlichen Bedarf der Stufen 2, 3 und 4 an, obwohl diese aus dem Spiel entfernt wurden.
- Fabriken, die Urbanisierung als Nebnprodukt erzeugen, können nicht mehr pausiert werden.
- Die Auswahl eines Bergbauplatzes auf dem Mond zeigt nur 5 mögliche Einträge in der Benutzeroberfläche an. Da es nun insgesamt 6 Minen gibt, kann der Regolith-Sammler nur noch über das Baumenü gebaut werden.
- Erhöhter Lagerplatz für Seltene Ressourcen-Generatoren wird erst nach einmaligem Einsammeln der Ressourcen wirksam. Wartet daher immer, bis die erste Einheit generiert wurde und sammelt sie sofort nach dem Bau ein, um die Speichermenge auf den modifizierten Wert zu setzen.

**Mars:** Aufgrund der Art und Weise, wie der Mars-Sektor als Teil der Mond-Region programmiert ist, ergeben sich hieraus einige spezielle Probleme:

- Der Mars-Sektor braucht länger zum Laden als andere Sektoren.
- Die Freischaltbenachrichtigung für neue Gebäude auf dem Mond wurde geändert, so dass alle neu freigeschalteten Mondgebäude in der Benachrichtigung als "Neue Mondgebäude" angezeigt werden.
- Um das Bau-Menü zu verwalten und die Mars-Gebäude auf den Mars-Sektor zu beschränken, musste ich einen Workaround verwenden, indem ich die Mond-Gebäude beim Betreten der Mars- Session gesperrt habe. Wenn man die Mars- Session verlässt (z.B. um Handelsrouten anzupassen), bekommt man eine Benachrichtigung, dass wieder " Neue Mond-Gebäude" freigeschaltet worden sind. Ich habe die Benachrichtigung bereits verkürzt, indem ich den " Neue Mondgebäude"-Pool verwendet habe, aber wenn ich sie komplett deaktiviere, erhält man beim ersten Freischalten keine Benachrichtigung.
- Nachdem man den Mars-Sektor betreten und das Bau-Menü geöffnet hat, muss man regelmäßig den Reiter "Mars-Synthetiks" erneut auswählen, um die verfügbaren Gebäude zu sehen.
- Das Drücken des Hotkeys für " Straße bauen" auf dem Mars führt zu den Mondwegen anstelle der erwarteten Marswege. Pipettieret oder benutzt den Bau-Menüeintrag, um stattdessen Mars- Straßen zu bauen.
- Die Verwendung des Gebäude-Filter-Reiters neben der Minimap (die Bevölkerungs-Schaltfläche) in der Mars- Session führt zu einem Einfrieren des Spiels, das nur durch Beenden der Task behoben werden kann.
- Der Mars-Sektor verfügt über einige einzigartige Sektor-Eigenschaften. Beachtet, dass beim Betreten des Sektors die Begrüßungsoberfläche eine zufällige Mondeigenschaft anstelle der Marseigenschaft anzeigt. Diese Eigenschaft wird dem Sektor nur beim ersten Betreten zugewiesen. Ihr könnt die Sektoreigenschaft neu vergeben, indem ihr eine spezielle Quest absolviert. Dazu muss man bestimmte Produkte an seinen Raumhafen liefern. Beachtet, dass der übliche Weg, Sektoreigenschaften neu zu würfeln, zu einer zufälligen Eigenschaft des Mondes führt!
- Mars-Meteore verwenden die Bodentexturen des Mondes.
- Während des Ladevorgangs ändert sich das Symbol des Mars-Sektors in ein weißes Rechteck. Sobald der Ladevorgang läuft, klickt man erneut auf eine beliebige Stelle der strategischen Ansicht, um das Symbol wieder zu sehen.
- Immer wenn sich die Mars-Jahreszeit ändert und man sich in einem anderen Sektor befindet, wechselt die Tageszeit von selbst zu derjenigen, die vom Mars-Jahreszeit-Effekt verwendet wird. Man kann die Uhrzeit über das Kameramenü neben der Minimap einstellen.
- Wenn man die Quest "Geo-Engineering" auf dem Mars verwendet, kann das Skript zufällig die gleiche Eigenschaft auswählen, die bereits aktiv ist. Dies führt dazu, dass der Sektor seine Eigenschaft komplett verliert. In diesem Fall könnt ihr die Konsole benutzen, um den Effekt wieder zu bekommen. Die GUIDs können [hier](/de/Anno2205/SectorTraits.md) gefunden werden. Als erstes müsst ihr den Mars-Sektor betreten. Drückt dann Shift+F1, um die Konsole zu öffnen und gebt `debug.toggleSectorEffect(GUID)` mit der entsprechenden GUID des gewünschten Traits ein. Drückt Enter und schließt die Konsole wieder mit Shift+F1.
- Manchmal können die Effekte der Mars-Jahreszeiten zufällig auf dem Mond auftreten. Dies ist ein Problem, da sie sehr lange andauern und nicht durch eine Quest gelöst werden können. Auch hier müsst ihr die Konsole benutzen, um sie loszuwerden. Betretet zunächst die betreffende Mond-Session. Drückt nun Shift+F1, um die Konsole zu öffnen und gebt `debug.toggleSectorEffect(GUID)` ein. Ersetzt nun den Platzhalter „GUID“ durch die entsprechende GUID des gerade aktiven Jahreszeiteneffekts (siehe unten). Drückt die Enter-Taste und schließt die Konsole wieder mit Shift+F1. Der Effekt sollte nun verschwunden sein.
- Sometimes, Martian Season effects can end up mismatched with the current season quest. If you currently suffer from mismatched season effect to the shown season quest in the quest tracker on the left side of the screen, you have to use the console to fix this:
> 1. Drücke Shift+F1, um die Konsole zu öffnen.
> 2. Gib ein (ohne Tippfehler, achte auf Groß- und Kleinschreibung!), ersetze "CurrentSeasonGUID" mit der korrekten Zahl aus der Tabelle unten:
`debug.startSectorEffect(CurrentSeasonGUID,19990093)`
> 3. Drücke die Eingabetaste
> 4. Gib ein (ohne Tippfehler, achte auf Groß- und Kleinschreibung!), , ersetze "CorrectSeasonGUID" mit der korrekten Zahl aus der Tabelle unten:
`debug.startSectorEffect(CorrectSeasonGUID,19990093)`
> 5. Drücke Shift+F1, um die Konsole zu schließen.
> 6. Der Sektoreffekt sollte nun mit der aktuellen Jahreszeitenquest übereinstimmen.

  |Jahreszeit|Sommer|Herbst|Winter|Frühling|
  |---|---|---|---|---|
  |GUID|19990307|19990378|19990370|19990374|
