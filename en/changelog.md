# Changelog

All notable changes to this project will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

- [v4.0.0build1000](#v4.0.0build1000)
- [v3.4.0build1005](#v3.4.0build1005)
- [v3.4.0build1004](#v3.4.0build1004)

<a name="v4.0.0build1000"></a>

## [v4.0.0build1000] - 2020-02-11

### Changed

- `fuse template` auf Version `4.0.0` angehoben - drastische Verkleinerung des Javascript-Bundles auf nur noch 100KB (vorher 3MB)
  - [https://material-ui.com/guides/minimizing-bundle-size/#how-to-reduce-the-bundle-size](https://material-ui.com/guides/minimizing-bundle-size/#how-to-reduce-the-bundle-size)
- komplette Überarbeitung der `Folder`-Struktur - Umstellen aller Imports auf `path imports` => `import Button from '@material-ui/core/Button';`

### Fixed

- `imageRender` bei `My Playlists` korrigiert (Bilder wurden nicht richtig geladen)
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

- `imageRender` refaktoriert, damit diese Funktion nicht allzu oft dupliziert wird

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
