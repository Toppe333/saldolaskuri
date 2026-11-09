# Saldolaskuri

Lenkki- ja punttisaldojen laskuri puhelimeen.

- **Lenkit**: katto 3 h, slideri 0–2 h minuutin tarkkuudella.
- **Puntit**: katto 1 h, slideri 0–1 h minuutin tarkkuudella.
- Saldot voivat mennä katon yli. Katon yläpuolinen osa näkyy palkissa tiivistyvällä asteikolla.
- **Lunasta** aukeaa, kun molemmat saldot ovat katossa. Lunastus vaatii 2,3 sekunnin yhtäjaksoisen painalluksen ja vähentää katot saldoista, joten ylijäämä jää talteen.
- Jokaisen lisäyksen, lunastuksen ja nollauksen voi kumota viiden sekunnin ajan.
- Tiedot tallentuvat selaimen local storageen (`saldolaskuri.v1`).

## Käyttö puhelimessa

Avaa https://toppe333.github.io/saldolaskuri/

- **iPhone (Safari):** Jaa → Lisää Koti-valikkoon.
- **Android (Chrome):** ⋮ → Lisää aloitusnäytölle / Asenna sovellus.

Kotinäytöltä avattuna sovellus toimii koko näytön tilassa ja myös ilman verkkoyhteyttä.

Huom: iPhonella kotinäytön sovelluksella on oma tallennustilansa. Safarissa kerätyt saldot eivät siirry sinne, joten käytä sovellusta alusta asti kotinäytön kuvakkeesta.

## Haptiikka

- Android: Vibration API (eri värinäkuviot lisäykselle, katolle ja lunastukselle).
- iPhone (iOS 18+): kevyt napautus piilotetun `<input switch>` -kytkimen kautta. Värinäkuvioita ei voi säätää.

## Tiedostot

- `index.html` – koko sovellus (HTML, CSS ja JS samassa tiedostossa)
- `manifest.webmanifest`, `icons/` – kotinäytön asennus
- `sw.js` – offline-tuki
