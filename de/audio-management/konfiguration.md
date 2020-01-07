# Konfiguration

---

- [Übersicht](#uebersicht)
- [Allgemeine Einstellungen](#allgemeine-einstellungen)
- [Module an- und abschalten](#module-an-und-abschalten)
- [E-Mail Einstellungen](#email-einstellungen)
- [Sales Einstellungen](#sales-einstellungen)
- [Distributoren Einstellungen](#distributor-einstellungen)
- [ISRC-Root definieren](#isrc-root)

<a name="uebersicht"></a>
## Übersicht

### Wo finde ich die Einstellungen?
Die Einstellungen von Deinem Affekt-System findest Du an zwei Stellen.
* Klicke das Einstellungen-Symbol auf der Linken Quick-Panel Leiste
* Klicke auf dein User-Avatar-Bild oben rechts und dann auf SETTINGS

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/Ud4ObNc277.png" width="500">
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/k4mWHhXsXG.png" width="500">

### Auswahl Deines Audio Managements / Record Labels
Wähle auf der farbigen Tab-Leiste dein Record Label, welches Du einstellen möchtest.
Es werden hier hintereinander, alle Audio Managements aufgelistet, die zu Deinerm Kunden bei Affekt zugehörig sind.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/GvFZYZ4QFh.png" width="500">

<a name="allgemeine-einstellungen"></a>
## Allgemeine Einstellungen
### Exklusivitäts-Typen
Wir haben für jeden Record Label Start 4 Exklusivitäts-Typen standardmäßig festgelegt.
1. exclusive - für alle Tracks, die exklusiv zu Deinem Repertoire im Label gehören, für Compilations jedoch einen gesonderten Vertrag benötigen
2. non-exclusive-full - für alle Tracks, die zu exklusiv zu Deinem Repertoire gehören und eine Lizenz für die Verkompilierung vorhanden ist
3. non-exclusive - für alle Tracks, die non-exklusive zu Deinem Repertoire gehören
4. not-available - für Tracks, die keine Lizenz zur Veröffentlichung auf Deinem Label mehr haben, zum Beispiel ältere abgelaufene Lizenzen (diese Tracks müssen jedoch in der Datenbank wegen Abrechnungen bleiben)

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/PDU2CrSxJw.png" width="500">

### Dokumenten-Typen

> {warning} Diese Funktionen implementieren wir derzeit.

<a name="module-an-und-abschalten"></a>
## Module an- und abschalten
Wir entwickeln jeder Zeit an coolen neuen Funktionen für Record Labels, stellen Dir jedoch die Möglichkeit zur Verfügung einzelne Module wieder abzuschalten. Wenn Du ein Modul nicht benötigst, dann stelle es ab. Im Hintergrund löschen wir jedoch keine Daten, solltest Du ein Modul schon eimmal benutzt haben. Wir blenden es nur aus.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/jyBnoCaIHY.png" width="500">

### Überblick der Entwicklung von Modulen
| # | Name   | Status |
| : |   :-   |  :  |
| 1 | Remixes | experimental - in development |
| 2 | Demos / Preview Tracks | experimental - in development |
| 3 | DJ-Sets | experimental - in development |

<a name="email-einstellungen"></a>
## E-Mail Einstellungen
Für ausgehende E-Mails kannst Du hier bestimmte CC Adressen angeben. Bitte trage hier Deine gewünschten Adressen ein.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/4nT1bAprgq.png" width="500">

### Überblick von derzeitigen Outgoing-Emails
| # | Name   | Beschreibung |
| : |   :-   |  -:-  |
| 1 | Release Info Email | Eine Release Information, die an Deinen Künstler geht. Unter RELEASES haben wir ein Tool eingebaut, mit dem Du Deinen Künstler über den Status seines Releases auf Deinem Label benachrichtigen kannst. |
| 2 | Royalty Email | Diese Email beinhaltet das Royalty-Statement, das Du an Deine Künstler verschickst. Unter ACCOUNTS und dem jeweiligen abzurechnenden Künstler findest Du diese Tools. |

<a name="sales-einstellungen"></a>
## Sales Einstellungen
### Systemübergreifende Währung
Bitte definiere Deine Grund-Währung, mit der Du in Deinem Record Label arbeitest. Wir supporten derzeit nur eine einzige Währung pro **Audio Management**. Diese Währung wird für Deine Künstler in ihren eigenen Übersichten angezeigt und ebenso auf den Royalty Statements.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/HAMATsZ0Bs.png" width="500">

### Abrechnungs-Basen
Es gibt 3 Standard-Abrechnungsarten.
1. Über digitale Einzel-Verkäufe - Digital Single NET
2. Über digitale Bundle-Verkäufe - Digital Bundle NET
3. Über Streams - Digital Stream NET

Du kannst weitere spezielle Arten der Abrechnung dazuschalten, wenn Du sie brauchst.

> {info} An- und Abschalten blendet die Abrechnungsart auf den jeweiligen Editoren nur ein und aus. Du verlierst keine Daten, wenn Du hier eine Art abschaltest. Die eingestellten Shares auf Deinen Lizenzen bleiben im Hintergrund bestehen.

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/o3r9JiD7e7.png" width="800">

### Abrechnungsarten
| # | Name   | Beschreibung |
| : |   :-   |  -:-  |
| 1 | Retail NET | CD / Retail Verkauf |
| 2 | Retail Dealer Selling Price | Abzug/Share nach Handeslabgabepreis |
| 3 | Retail Distribution Selling Price | Abzug/Share nach Distributorenpreis |
| 4 | Digital Single Distribution Selling Price | Digitaler Einzel-Verkauf mit Abzug/Share nach Distributorenpreis |
| 5 | Digital Bundle Distribution Selling Price | Digitaler Bundle-Verkauf mit Abzug/Share nach Distributorenpreis |
| 6 | Digital Stream Distribution Selling Price | Stream mit Abzug/Share nach Distributorenpreis |
| 7 | Digital Single NET on Compilations | Digitaler Einzel-Verkauf auf einer Compilation |
| 8 | Digital Bundle NET on Compilations | Digitaler Bundle-Verkauf auf einer Compilation |
| 9 | Digital Stream NET on Compilations | Stream auf einer Compilation |

<a name="distributor-einstellungen"></a>
## Distributoren Einstellungen
Du findest hier unseren bisher unterstützten Distributoren mit ihren FTP-Einstellungen wider. Bitte gebe hier die FPT-Zugangsdaten ein, die dein Distributor auf dem jeweiligen Backend zur Verfügung stellt. Unser System ist in der Lage, automatisch alle WAV Dateien eines Releases während des PUBLISHING Vorgangs auf den FTP-Servers des Distributors hochzuladen.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/YS3Ty4N6H7.png" width="800">

<a name="isrc-root"></a>
## ISRC-Root definieren
Bitte gebe hier Deine ISRC-Roots an, die Du für ein Record Label verwendest. Wir haben einen integrierten ISRC-Manager gebaut, der Dir dabei hilft, keine fortlaufenden Nummern zu überspringen oder noch schlimmer Duplikate entstehen zu lassen.

> {primary} Ohne ISRC-Root wirst Du selbst alle ISRC-Codes manuell für jeden Track angeben müssen. Ansonsten wird das Abrechnungs-System nicht zuweisen- und funktionieren können.

<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/WswJqcmrmZ.png" width="800">

> {info} Der ISRC Code ist ein 12-stelliger Code und steht für International Standard Recording Code. Die ersten beiden Buchstaben stehen für das Land, in dem der Titel veröffentlicht wurde. Die nächsten drei Stellen stehen für das Label, das die Titel veröffentlicht. Die nächsten beiden Zahlen stehen für das Veröffentlichungsjahr. Mit den letzten fünf Zahlen werden die einzelnen Titel durchgezählt. Jeder Titel und jede Version eines Titels erhalten einen eigenen ISRC Code. Der ISRC Code wird in den TOC (Table of Contents) einer Master-CD codiert. Er identifiziert jeden Titel bei der GEMA und wird von den Rundfunk- und Fernsehanstalten ausgelesen, um die GEMA-Abrechnung zu erleichtern. Die ISRC Codes werden von dem Label, welches das Album veröffentlicht, festgelegt. Die Vergabe des Codes kann bei der IFPI beantragt werden.

### TRACK EDIT - ISRC-Manager
Hier ein Ausblick auf den ISRC-Manager bei einem TRACK EDIT. Wie Du siehst, kannst Du bei Angabe eines Roots, diesen auswählen und das System gibt Dir einen nächsten ISRC-Code vor. So entstehen keine Lücken in der fortlaufenden Nummerierung und auch keine Duplikate.
<img src="https://affekt-assets.s3-eu-central-1.amazonaws.com/docs/I9xLWerFWX.png" width="800">
