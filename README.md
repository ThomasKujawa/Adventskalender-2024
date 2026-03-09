# Adventskalender 2024

Ein interaktiver PHP-basierter Adventskalender, der täglich vom 1. bis 24. Dezember neue Inhalte freischaltet.

## Beschreibung

Dieser Adventskalender zeigt täglich neue Inhalte, die erst ab dem jeweiligen Dezember-Tag zugänglich werden. Die Anwendung prüft das aktuelle Datum und gibt entsprechende Inhalte frei. Bereits vergangene Tage bleiben weiterhin zugänglich.

## Features

- Automatische tagesbasierte Freischaltung der Inhalte
- 24 verschiedene Türchen für jeden Tag im Dezember
- Responsive Design
- Spendenaufruf für das selfHTML-Projekt
- Bildergalerie mit Detailansichten

## Technologie

- **Backend**: PHP 7.x/8.x
- **Frontend**: HTML5, CSS (inline), JavaScript (inline)
- **Struktur**: Modularer Aufbau mit separaten Dateien für Daten, Styling und Logik

## Dateistruktur

```
├── index.php          # Haupteinstiegspunkt
├── data.php           # Datenarray mit 24 Einträgen
├── css.php            # Stylesheet-Definitionen
├── js.php             # JavaScript-Funktionen
├── images/            # Bilddateien für die Türchen
└── paar.png          # Titelbild
```

## Installation

1. Repository klonen:
   ```bash
   git clone https://github.com/ThomasKujawa/Adventskalender-2024.git
   ```

2. Dateien auf einen Webserver mit PHP-Unterstützung hochladen

3. Sicherstellen, dass der `images/`-Ordner die erforderlichen Bilder enthält

4. Im Browser aufrufen (z.B. `http://localhost/Adventskalender-2024/`)

## Konfiguration

Die Inhalte können in der `data.php` angepasst werden. Jeder Tag enthält:
- `href`: Link oder Pfad zum Inhalt/Bild
- `heading`: Überschrift des Türchens
- `author`: Autor (optional)
- `teaser`: Beschreibungstext

Das Jahr kann in der `index.php` angepasst werden:
```php
$year = 2024;
```

## Funktionsweise

- **Vor dem jeweiligen Tag**: Türchen zeigt "Dieses Türchen öffnet sich erst am X. Dezember"
- **Ab dem jeweiligen Tag**: Inhalt wird freigeschaltet und ist klickbar
- **Tag 23 und am Folgetag**: Spendenaufruf für selfHTML

## Lizenz

Dieses Projekt steht unter der [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.de.html).

Sie dürfen:
- ✓ Das Projekt kommerziell nutzen
- ✓ Das Projekt modifizieren
- ✓ Das Projekt verteilen
- ✓ Das Projekt privat nutzen

Bedingungen:
- → Änderungen müssen dokumentiert werden
- → Der Quellcode muss offengelegt werden
- → Ableitungen müssen unter der gleichen Lizenz stehen
- → Copyright- und Lizenzhinweise müssen erhalten bleiben

## Autor

Thomas Kujawa

## Hinweise

Dieses Projekt wurde für das Jahr 2024 entwickelt. Für andere Jahre muss die Jahreszahl in `index.php` angepasst werden.