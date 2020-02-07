# Changelog

All notable changes to this project will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

- [v3.4.0build1004](#v3.4.0build1004)

<a name="v3.4.0build1004"></a>
## [v3.4.0build1004] - 2020-02-07

### Changed
 - `app.js` von `vendor.js`  getrennt, damit die Seite schneller geladen wird
	- `vendor.js` ändert sich nicht so oft und kann im Browser-Cache liegen
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
- `Notification` Tab hinzugefügt und erste Einstellung für Notification Email eingesetzt
	- das Speichern von den Daten im Input-Feld rekonzipiert und optimiert

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_JulRnA8im5.png)
- `ImageCropper` hinzugefügt und in ein Popup Fenster dynamisiert

![enter image description here](https://s3.eu-central-1.amazonaws.com/affekt-assets/share/2020/02/chrome_M6koulUg9g.png)
