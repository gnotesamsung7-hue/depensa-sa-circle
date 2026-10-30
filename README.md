# Depensa sa Circle — Android APK

3D tower defense set in Quezon Memorial Circle. Ang laro ay nasa `app/src/main/assets/www/index.html`
at tumatakbo offline sa loob ng app (kasama na ang three.js at fonts).

## Paano gawin ang APK (GitHub lang, walang install sa laptop)
1. Gumawa ng bagong repository sa github.com (hal. `depensa-sa-circle`).
2. I-unzip ang file. Sa repo page, i-click ang **uploading an existing file** at i-drag ang LAHAT ng laman ng folder
   (kasama ang `.github` folder). I-commit sa `main`.
3. Pumunta sa **Actions** tab. Kusang tatakbo ang "Build APK" (mga 3–6 minuto).
4. Pagkatapos, buksan ang **Releases** (sa kanan ng repo page) sa phone at i-download ang `DepensaSaCircle.apk`.
5. I-install. Kung magtanong ang phone, payagan ang "Install unknown apps" para sa browser.

Kung hindi na-upload ang `.github` folder: **Add file → Create new file**, pangalanan na
`.github/workflows/build-apk.yml`, at i-paste ang laman ng file na iyon.

Para mag-update ng laro: palitan lang ang `app/src/main/assets/www/index.html` at i-commit. Tataasan ang build number
nang kusa. (Kung gusto mong mag-update nang hindi binubura ang lumang install, taasan ang `versionCode` sa `app/build.gradle`.)
