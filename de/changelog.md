# Changelog

All notable changes to this project will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

- [v4.0.1build1002](#v4.0.1build1002)
- [v4.0.1build1001](#v4.0.1build1001)
- [v4.0.1build1000](#v4.0.1build1000)
- [v4.0.0build1000](#v4.0.0build1000)
- [v3.4.0build1005](#v3.4.0build1005)
- [v3.4.0build1004](#v3.4.0build1004)

<a name="v4.0.1build1002"></a>

## [v4.0.1build1002] - 2020-02-21

### Changed

- die `Playlist Overview` Page wurde komplett überarbeitet - ist nun eingebunden im `Fuse-Theme` und ist somit besser zum Warten - steht in direkter Verbindung mit dem Login-System, so dass wir an der Seite zB zusätzliche Informationen und Links für den User darstellen können - anhand von "Vorlieben" des Users, könnte man in Zukunft auf der rechten Leiste `recommended` Playlisten anzeigen lassen - eingeloggten Usern können sehr viele vorteilhafte Funktionen an der Seitenleiste präsentiert werden, so dass er die gesamte Affekt-World im Überblick hat

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_uRP5tO1Qev.png)

- das gleiche System wurde bei den `User-Profiles` eingesetzt - man kann nun die Playlisten des Users filtern
- die Anzeige der `Reputation` wurde auf die Profilseite hinzugefügt

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_HyZ4p4d5NH.png)

### Added

- für die Playlisten gibt es nun einen besseren Filter - man klickt auf das Genre und die Liste wird unten performanter sortiert - die Playliste-Ergebnisse sind in einem eigenem `Scroll-View` eingebaut, so dass das Scroll-Verhalten verbessert wurde

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_CCktAhyDTf.png)

<a name="v4.0.1build1001"></a>

## [v4.0.1build1001] - 2020-02-18

### Added

- die `Avatare` auf der rechten Leiste sind nun klickbar - die Links führen zu einer `public` Profilseite des Users - dort werden zunächst seine Submission Pages angezeigt und kann dort direkt auf die Submission Page klicken - in Planung sind `Direct-Chat` und `Releases`

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_Q2Vf3ndHK7.png)

- `Profile-Seite` - der Header-Bereich kann mit einem eigenem Titel-Bild versehen werden - in Planung sind ebenso `Activity-Log`, um anzuzeigen, wie aktiv der User auf der Plattform ist

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_ngpEpiMWks.png)

### Changed

- das `Layout-System` wurde geändert, damit die Unter-Laylouts nicht neu geladen werden müssen - für den `Audio-Player` wichtig, damit dieser bei wechsel der Page nicht unterbrochen wird

<a name="v4.0.1build1000"></a>

## [v4.0.1build1000] - 2020-02-17

### Added

- `Track-Edit` und `Track-Create` - man kann ab nun Tracks editieren und erstellen - die komplette Editierungs-Ansicht wurde überarbeitet und verbessert
- `Track-License-Overview` - eine Lizenzübersicht zum ein- und wiederausklappen

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_ndcaESN7IS.png)

- ein `ISRC-Manager` - ISRCs aus dem Root werden automatisch hochgezählt oder eine eigene ISRC kann vergeben werden und dem Track attached werden

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_r0fsXvPQ9b.png)

- `Lizenz-Verwaltung` eines Tracks pro Artist - unter jeden `Artist` wird nun angezeigt, welche `Shares` dieser besitzt - `bei Artists` ohne `Shares` bleibt die Ansicht frei

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_s2OyL0yUEP.png)

- `Last Catalog Number` - die nächste Katalog-Nummer wird automatisch berechnet und angezeigt - mit einem Button-Klick kann man die nächste Nummer automatisch ausfüllen lassen

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_K2tsyoCIax.png)

- den `Audio-Player` komplett neu rekonzipert, da das `Wavesurfer-Plugin` in einer neuen Version vorliegt - stabiler und schneller mit nativem React Code und eigene Komponente

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/0ycDINCAqF.png)

### Changed

- Routen optimiert - alle Routen haben Namen bekommen und wurde refaktoriert, so dass man einfach copy-pasten kann

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/ConEmu64_7IpiTLJvoY.png)
![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/phpstorm64_wRyUNsM8vW.png)

- Update auf das neue `fuse v4.0.1` - Lizenz um ein weiteres Jahr verlängert

### Fixed

- das Vorlesen von eingehenden neuen `Playlist-Submissions` wieder korrigiert - dazu wird es bald ein Quick-Setting zum Abschalten geben (auf der rechten Seite)
- `vapor deploy` korriegiert, da Symlinks nicht mehr funktioniert haben
- Dashboard Items limitiert, damit die Datenmenge nicht zu groß wird

<a name="v4.0.0build1000"></a>

## [v4.0.0build1000] - 2020-02-11

### Changed

- `fuse template` auf Version `4.0.0` angehoben - drastische Verkleinerung des Javascript-Bundles auf nur noch 100KB (vorher 3MB)
  - [https://material-ui.com/guides/minimizing-bundle-size/#how-to-reduce-the-bundle-size](https://material-ui.com/guides/minimizing-bundle-size/#how-to-reduce-the-bundle-size)
- komplette Überarbeitung der `Folder`-Struktur - Umstellen aller Imports auf `path imports` => `import Button from '@material-ui/core/Button';`

### Fixed

- `AvatarImageComponent` bei `My Playlists` korrigiert (Bilder wurden nicht richtig geladen)
- `PrismCode` korrigiert, da `window.Prism` nicht definiert war - `styles/prism.css` zum Index hinzugefügt
- `Auth0 invalid state` für `Audio Management`-Logins versucht zu beheben
- `Request-Authorizations` für `Playlist-Exchange` gefixed

### Added

- `MusicTrackEdit` hinzugefügt
- `Edit/Create` für folgende Module hinzugefügt - Accounts - Artists - Contributors - Labels

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_Bxu6SJjk2Z.png)

- `react-helment` hinzugefügt, damit die Meta-Angaben von den Pages dynamisch geswitched werden können

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_PChQtQeqxv.png)

<a name="v3.4.0build1005"></a>

## [v3.4.0build1005] - 2020-02-10

### Changed

- `AvatarImageComponent` refaktoriert, damit diese Funktion nicht allzu oft dupliziert wird

### Fixed

- `CORS-Headers` hinzugefügt, damit einige Javascript-Funktionen als `XHR` funktionieren
- `Left-Side-Panel` Links zu den einzelnen `Audio-Managements` als `window.open` definiert, weil sie durch die Auth0 Routinen durchgehen müssen
- `ImageUploader` für die `Audio-Managements` konfiguriert

### Added

- `Labelcopy`-Download für einen Track hinzugefügt
- `Excel`-Exports neu definiert und eingestellt
- `getID3`-Library hinzugefügt, damit die ID3-Tags in neuster `id3v2.4`-Version gespeichert werden können
- Track-File-Downloads hinzugefügt und AWS Lambda fähig gemacht
- `Accounts` - Index and Edit, only-super-admins
- `Labels` - Index and Edit, only-super-admins
- `Artists` - Index and Edit, only-super-admins
- `Contributors` - Index and Edit, only-super-admins
- `Tracks` - Index, only-super-admins

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_LlUIetLOp3.png)

<a name="v3.4.0build1004"></a>

## [v3.4.0build1004] - 2020-02-07

### Changed

- `app.js` von `vendor.js` getrennt, damit die Seite schneller geladen wird - `vendor.js` ändert sich nicht so oft und kann im Browser-Cache liegen
- aus `Customer` Daten herausgenommen, die nicht gebraucht werden auf dem Dashboard
- `webpack.mix` Image-Optimierer installiert, damit die Bilder kleiner werden (zB PNGs zu JPGs wenn es sich anbietet)
- `My-Landing-Page` aus dem Maintenance-Modus herausgenommen, da die `Media-Library` nun gefixed ist
- `react-app-polyfill` entfernt, damit das Bundle-Paket kleiner wird
- `n+1-Problem` bei `customer-online` gelöst
- `searchForApplications` gecached damit die Seitenladezeit sich drastisch verringert

### Fixed

- die `Media-Library` Url gefixed, damit Dateien richtig auf die `Amazon S3` hochgeladen werden
- `Echo Pusher Service` wurde mehrfach initialsiert; liegt nun in `app.js` und wird einfach geladen
- `tickInterval` vom `Repuation-Render` erhöht, damit `devextreme` es richtig anzeigen kann
- den `Playlist Overview`-Link korrigiert, der auf dem `Playlist-Exchange Dashboard` unten zu sehen ist
- `facebook`-Sign-Ups gefixed, weil kein Username vergeben wird

### Added

- `Change Username` sowie `Change profile picture` Button hinzugefügt

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_sIJUopxwSo.png)

- `Account Settings Tab` hinzugefügt und eigene URL gegeben sowie `Account` löschen möglich gemacht

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_T0yas5yNqj.png)

- `Notification` Tab hinzugefügt und erste Einstellung für Notification Email eingesetzt - das Speichern von den Daten im Input-Feld rekonzipiert und optimiert

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_JulRnA8im5.png)

- `ImageCropper` hinzugefügt und in ein Popup Fenster dynamisiert

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_M6koulUg9g.png)
