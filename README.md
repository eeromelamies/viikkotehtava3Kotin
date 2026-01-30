# Viikkotehtava2Kotlin
---

## Tämä sovellus käyttää MVVM (Model-View-ViewModel) -mallia, joka jakaa sovelluksen selkeisiin osiin
- Model: Data (tehtävät)
- View: Käyttöliittymä (Compose-funktiot)
- ViewModel: Sovelluslogiikka ja tilan hallinta.

---

## Miksi MVVM on hyödyllinen Compose-sovelluksissa
- Tilan hallinta (State Management): Jetpack Composen käyttöliittymä rakentuu tilan (state) ympärille. ViewModel säilyttää tilan, vaikka näyttö käännettäisiin tai sovelluksen prosessi käynnistettäisiin uudelleen.
- Logiikan eriyttäminen: Käyttöliittymäkomponentit (@Composable) pysyvät siisteinä, kun monimutkainen logiikka, kuten suodattaminen (filterByDone) tai järjestäminen (sortByDueDate), siirretään ViewModeliin.
- Yksisuuntainen tietovirta (UDF): ViewModel tarjoaa tilan, jota View lukee. View lähettää tapahtumia (kuten painikkeiden klikkaukset) takaisin ViewModelille. Tämä tekee koodista ennakoitavampaa.

---

## Projektin toiminnot
- Lisääminen: Uusien tehtävien luominen listaan.
- Muokkaaminen: Tehtävän nimen ja kuvauksen muuttaminen erillisessä DetailScreen (AlertDialog) -näkymässä.
- Poistaminen: Tehtävien poisto listalta.
- Suodatus: Mahdollisuus nähdä kaikki tai vain tekemättömät tehtävät.
- Järjestys: Tehtävien järjestäminen joko ID:n tai eräpäivän mukaan.

---

## Asennus

- Kloonaa repo:
- bash: git clone <repo_url>
- Avaa projekti Android Studiossa
- Rakenna ja suorita sovellus emulatorissa tai laitteessa
