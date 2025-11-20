# Zadatak: Dodaj CSS na postojeći HTML (početni nivo)

Dobivate gotov HTML kod.  
Vaš zadatak je dodati osnovni CSS unutar `<style>` taga.

Ne morate izmišljati vlastita svojstva – sve potrebne deklaracije nalaze se niže u zadatku.  
Vaš posao je:

- odabrati **koji selektor** treba koje deklaracije  
- kopirati deklaracije na pravo mjesto u CSS-u

HTML se **ne smije mijenjati**.

---

## 1. HTML koji dobijete

U datoteku `index.html` upišite sljedeći kod:

```html
<!DOCTYPE html>
<html lang="hr">
<head>
    <meta charset="UTF-8">
    <title>Moja prva stranica – Header</title>
    <style>
        /* OVDJE ĆETE DODATI SVOJ CSS KOD */
    </style>
</head>
<body>

    <header>
        <div class="banner">
            <img src="lego_banner.jpg" alt="Lego">
        </div>

        <nav class="main-nav">
            <ul>
                <li><a href="#">Početna</a></li>
                <li><a href="#">O nama</a></li>
                <li><a href="#">Usluge</a></li>
                <li><a href="#">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <p>Ovdje će ići ostatak sadržaja stranice.</p>
    </main>

    <footer>
        &copy; Vaše ime i prezime
    </footer>
</body>
</html>


2. CSS kostur koji trebate popuniti

U dio <style> (u <head>) zalijepite ovaj kostur i popunite ga deklaracijama:

/* 1. Reset osnovnih margina i paddinga za sve elemente */
* {
    /* ovdje idu deklaracije za margin i padding */
}

/* 2. Osnovni stil za cijelu stranicu */
body {
    /* ovdje idu deklaracije za font i pozadinsku boju stranice */
}

/* 3. Header dio stranice */
header {
    /* ovdje idu deklaracije za pozadinsku boju, border, margin i padding */
}

/* 4. Banner slika unutar headera */
.banner img {
    /* ovdje idu deklaracije za širinu slike i da nema razmaka ispod slike */
}

/* 5. Navigacija ispod bannera */
nav {
    /* ovdje idu deklaracije za pozadinsku boju navigacije, padding i gornji margin */
}

/* 6. Lista u navigaciji */
ul {
    /* ovdje idu deklaracije za list-style, margin i padding */
}

/* 7. Stavke liste u navigaciji */
li {
    /* ovdje idu deklaracije za prikaz u jednom redu i razmak desno */
}

/* 8. Linkovi u navigaciji */
a {
    /* ovdje idu deklaracije za text-decoration, boju teksta, border, padding i veličinu fonta */
}

/* 9. Glavni sadržaj (main) */
main {
    /* ovdje idu deklaracije za pozadinsku boju, border, margin i padding */
}

/* 10. Tekst u glavnom sadržaju */
main p {
    /* ovdje ide deklaracija za razmak između redova (line-height) */
}

/* 11. Footer */
footer {
    /* ovdje idu deklaracije za poravnanje teksta, veličinu fonta, boju teksta i donji margin */
}


3. Deklaracije koje morate iskoristiti

Sve potrebne deklaracije su napisane ispod.
Kopirajte ih i zalijepite u odgovarajuće selektore iz CSS kostura.

Napomena: ne ponavljajte deklaracije bez potrebe.

margin: 0;
padding: 0;

font-family: Arial, sans-serif;
background-color: #f0f0f0;

background-color: white;
border: 1px solid #cccccc;
margin: 20px;
padding: 10px;

width: 100%;
display: block;
border-bottom: 3px solid #ffcc00;

background-color: #333333;
padding: 8px;
margin-top: 10px;

list-style-type: none;
margin: 0;
padding: 0;
text-align: center;

display: inline-block;
margin-right: 15px;

text-decoration: none;
color: white;
border: 1px solid white;
padding: 5px 12px;
font-size: 14px;

background-color: white;
border: 1px solid #cccccc;
margin: 0 20px 20px 20px;
padding: 10px;

line-height: 1.5;

text-align: center;
font-size: 12px;
color: #555555;
margin-bottom: 10px;


4. Uputa za rad

Otvorite datoteku index.html.

U <style> tag zalijepite CSS kostur iz poglavlja 2.

Zatim iskoristite deklaracije iz poglavlja 3 i rasporedite ih u odgovarajuće selektore.

Pokušajte logički rasporediti deklaracije:

što ide u body

što ide u header

što ide u .banner img

što ide u nav, ul, li, a

što ide u main i main p

što ide u footer

Spremite datoteku i otvorite je u pregledniku.

Cilj je da dobijete jednostavnu, ali urednu stranicu s bannerom, navigacijom, glavnim sadržajem i footerom.