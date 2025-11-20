# Dodatni zadatak: Tablica rasporeda LEGO radionica

Ovaj zadatak je nastavak na postojeću LEGO početnu stranicu koju ste već izradili  
(LEGO klub Zagreb, s headerom, bannerom, navigacijom i sadržajem u `main` dijelu).

Cilj zadatka je:

- dodati **novu sekciju** u `main` dijelu s naslovom “Raspored radionica”
- unutar te sekcije dodati **tablicu** s terminima radionica
- dodati osnovni **CSS** za oblikovanje tablice

HTML izvan `main` dijela (header, footer) ne trebate mijenjati.

---

## 1. Upute – što treba napraviti

### 1.1 Dodaj novu sekciju u `<main>`

U vašem postojećem dokumentu pronađite `<main>` element i **pred kraj** (prije `</main>`) dodajte novu sekciju:

```html
<div class="section schedule-section">
    <h2 class="section-title">Raspored radionica</h2>

    <table class="raspored">
        <caption>Raspored radionica – zimski semestar</caption>
        <thead>
            <tr>
                <th>Dan</th>
                <th>Vrijeme</th>
                <th>Razina</th>
                <th>Dobna skupina</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Utorak</td>
                <td>18:00 – 20:00</td>
                <td>Početna radionica</td>
                <td>5. i 6. razred</td>
            </tr>
            <tr>
                <td>Četvrtak</td>
                <td>18:00 – 20:00</td>
                <td>Napredna radionica</td>
                <td>7. i 8. razred</td>
            </tr>
            <tr>
                <td>Subota</td>
                <td>10:00 – 12:00</td>
                <td>Specijalna radionica</td>
                <td>otvoreno za sve</td>
            </tr>
        </tbody>
    </table>
</div>
```

### 1.2 Dodaj CSS za tablicu

U `<style>` dio vašeg dokumenta (u `<head>`), gdje već imate postojeći CSS, potrebno je dodati još nekoliko selektora.

Ispod zadnjeg postojećeg CSS bloka dodajte sljedeće stilove:

a) Stil za tablicu rasporeda

Selektor: .raspored

```css
.raspored {
    width: 100%;
    border-collapse: collapse;
    margin-top: 10px;
}
```

Hint:

```css
width: 100%; – tablica ide preko cijele širine sadržaja

border-collapse: collapse; – spaja okvire ćelija u jedan

margin-top: 10px; – mali razmak iznad tablice
```
b) Stil za naslov tablice (caption)

Selektor: .raspored caption
```css
.raspored caption {
    margin-bottom: 5px;
    font-weight: bold;
}

```

Hint:

margin-bottom: 5px; – razmak ispod naslova tablice

font-weight: bold; – naslov tablice je podebljan

c) Stil za ćelije (zaglavlja i podatke)

Selektor: .raspored th, .raspored td

```css
.raspored th,
.raspored td {
    border: 1px solid #cccccc;
    padding: 6px;
    text-align: center;
    font-size: 14px;
}
```

Hint:

border: 1px solid #cccccc; – tanka siva linija oko svake ćelije

padding: 6px; – unutarnji razmak u ćeliji

text-align: center; – tekst u ćeliji je centriran

font-size: 14px; – veličina slova u tablici

d) Stil posebno za zaglavlje tablice

Selektor: .raspored th

```css
.raspored th {
    background-color: #fff7cc;
}
```

