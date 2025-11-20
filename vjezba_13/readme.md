# Dodatni zadatak: LEGO početna stranica – sadržaj i oblikovanje `main` dijela

Pretpostavljamo da ste prethodni zadatak već napravili  
(header s bannerom, navigaciju, osnovni `main` blok i footer).

Sada nadograđujemo stranicu tako da početna stranica izgleda kao jednostavna  
početna stranica LEGO kluba.

U ovom zadatku:

- dodajete novi HTML sadržaj unutar `<main>` elementa  
- dodajete nove CSS stilove za taj sadržaj  
- za svaku stavku dobivate gotove deklaracije (hintove), samo ih trebate staviti u odgovarajuće selektore

---

## 1. HTML sadržaj za LEGO početnu stranicu

U datoteci `index.html` **zamijenite postojeći `<main>` element** ovim kodom:

```html
<main>
    <h1>LEGO klub Zagreb</h1>

    <h2>Dobrodošli u naš LEGO svijet</h2>

    <p class="uvod">
        LEGO klub Zagreb okuplja studente koji vole slagati modele, smišljati priče
        i učiti kroz igru. Cilj kluba je razvijati maštu i logičko razmišljanje.
    </p>

    <p id="osnovan">
        Klub je osnovan 2024. godine i od tada redovito organiziramo radionice,
        natjecanja i izložbe LEGO modela.
    </p>

    <p>
        Na radionicama radimo u malim timovima. Svaki tim dobiva zadatak, a
        zatim zajedno planiraju, slažu modele i predstavljaju svoje rješenje.
        Na taj način učimo suradnju i komunikaciju.
    </p>

    <p>
        Posebno potičemo
        <span class="vazno">kreativnost</span> i
        <span class="vazno">rješavanje problema</span>
        kroz zabavne LEGO izazove.
    </p>

    <a class="lego-link" href="https://www.lego.com" target="_blank">
        Posjeti službenu LEGO stranicu
    </a>

    <img class="lego-slika" src="lego_set.jpg" alt="LEGO set">

    <h2>Popularne LEGO teme u našem klubu</h2>

    <ul class="lista-tema">
        <li>LEGO City</li>
        <li>LEGO Technic</li>
        <li>LEGO Star Wars</li>
        <li>LEGO Friends</li>
    </ul>

    <p class="napomena">
        Napomena: informacije o rasporedu radionica i prijavi nalaze se na oglasnoj ploči škole.
    </p>
</main>
```

## 2. Zadatak – dodajte CSS za novi sadržaj

U `<style>` dio (gdje već imate kod od prethodnog zadatka)
dodajte nove selektore i u njih upišite odgovarajuće deklaracije.

Ispod su hintovi – gotove deklaracije koje trebate iskoristiti.

### 2.1 Glavni naslov na stranici

Za naslov unutar main dijela (selektor možete npr. nazvati main h1):

```css
text-align: center;

color: blue;

margin-top: 10px;

margin-bottom: 10px;

font-size: 28px;
```

### 2.2 Podnaslovi u main dijelu

Za podnaslove (npr. selektor main h2):

```css
margin-top: 15px;

margin-bottom: 8px;

color: #333333;

font-size: 20px;
```


### 2.3 Svi odlomci u main dijelu

Za tekst odlomaka (npr. selektor main p):
```css
line-height: 1.5;

margin-bottom: 10px;

font-size: 16px;
```
### 2.4 Uvodni odlomak

Za uvodni odlomak (selektor .uvod):
```css
font-style: italic;

font-weight: bold;

margin-bottom: 15px;
```
### 2.5 Odlomak s godinom osnivanja

Za odlomak s informacijom o osnivanju (selektor #osnovan):
```css
background-color: #ffffff;

border: 1px solid #cccccc;

padding: 8px;

margin-bottom: 12px;
```
### 2.6 Naglašene riječi u tekstu

Za naglašene riječi unutar odlomaka (selektor .vazno):
```css
color: green;

font-weight: bold;
```
### 2.7 Poveznica na službenu LEGO stranicu

Za poveznicu na LEGO stranicu (selektor .lego-link):
```css
display: inline-block;

margin-top: 10px;

margin-bottom: 10px;

text-decoration: none;

border: 1px solid blue;

padding: 5px 10px;

color: blue;

background-color: #ffffff;
```
### 2.8 Slika LEGO seta u main dijelu

Za sliku u main dijelu (selektor .lego-slika):
```css
width: 300px;

border: 1px solid #cccccc;

margin-top: 10px;

margin-bottom: 10px;
```
### 2.9 Popis popularnih LEGO tema

Za listu s temama (selektor .lista-tema):
```css
margin-left: 20px;

margin-bottom: 10px;

list-style-type: square;
```
### 2.10 Napomena na dnu main dijela

Za napomenu (selektor .napomena):

```css

color: red;

font-size: 14px;

margin-top: 10px;
```
## 3. Što trebate napraviti

U index.html zamijenite `<main>` element kodom iz poglavlja 1.

U `<style>` dio dodajte nove selektore (npr. main h1, main h2, .uvod, #osnovan, .vazno, .lego-link, .lego-slika, .lista-tema, .napomena).

U svaki selektor upišite odgovarajuće deklaracije iz poglavlja 2.

Spremite datoteku i otvorite je u pregledniku.

Cilj je da početna stranica LEGO kluba ima:

jasan naslov i podnaslove

nekoliko odlomaka čitljivo oblikovanog teksta

istaknutu informaciju o osnivanju kluba

link na službenu LEGO stranicu

sliku LEGO seta

popis najpopularnijih LEGO tema


napomenu na dnu sadržaja

