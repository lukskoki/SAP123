# SAP123

CASE STUDY: WORLD HAPPINESS REPORT
Interpretacija podataka značajan je dio obrade podataka. Stoga je bitno znati kontekst podataka i upoznati se s datasetom.

OSNOVNA DESKRIPTIVNA STATISTIKA
Cilj deskriptivne statistike je opisivanje, sažimanje i interpretacija podataka na način koji olakšava razumijevanje njihovih osnovnih obilježja, ali ne daje nikakve zaključke o uzrocima ili posljedicama. 
Neki od osnovnih pojmova u okviru deskriptivne statistike su:

    
    Aritmetička sredina: statistika uzorka i služi kao točkovna procjena μ.
Sredina uzorka je nepristrana procjena očekivanja populacije.
    
    Medijan: robusna (neparametarska mjera), položajna srednja vrijednost koja se nalazi u sredini niza poredanog po veličini.
Predstavlja 50.-ti percentil ili drugi kvartil Q2.

    Mod je vrijednost opservacije koja se najčešće pojavljuje (dominantna vrijednost)

    Rang je najjednostavnija mjera rasipanja i jednak je razlici između najveće i najmanje vrijednosti u skupu podataka.


    Kvantili su točke koje dijele raspon distribucije vjerojatnosti u neprekidne intervale ISTE vjerojatnosti ili koje dijele opservacije na isti način.
    Percentili i kvartili su specijalni slučaj kvantila

    Naredba 'summary' prikazuje sažetak za svaki numerički stupac (minimum, prvi kvartil, medijan, srednju vrijednost, treći kvartil i maksimum). Prikazuje i broj jedinstvenih vrijednosti za faktorske ili karakterne stupce, kao i broj nedostajajućih vrijednosti, ako su prisutne.


VIZUALIZACIJA PODATAKA
Vizualizacija podataka proces je prikazivanja informacija pomoću grafičkih ili slikovnih elemenata kako bi se olakšalo razumijevanje, analiza i interpretacija podataka. 

Primjeri vizualizacija podataka uključuju histograme, pravokutne dijagrame, raspršene dijagrame i mnoge druge. Ovisno o vrsti podataka i cilju analize, odabir određenih vrsta vizualizacija može biti ključan za uspješan prijenos informacija.


Histogrami pokazuju i oblik distribucije i gustoću podataka.
Površina stupca proporcionalna je relativnoj frekvenciji razreda.
Kontinuirane varijable su grupirane u razrede.
Važan je izbor širine razreda, tj. broj razreda.

    Histogram - pokazuje oblik distribucije i gustoću podataka, a zasnovan je na grupiranju varijabli u razrede 



    Dijagram raspršenja (scatter plot) - jedan je od najvažnijih načina prikaza bivarijantnih podataka, te daje informaciju o povezanosti varijabli 

    ovaj kod stvara histogram za "Ladder.score" podatke s 20 intervala i dodaje crvenu vertikalnu liniju koja označava srednju vrijednost tih podataka.


    ovaj kod stvara grafički prikaz medijana "Ladder.score" podataka za različite regije. Točke na grafikonu predstavljaju medijane, a svaka regija ima svoju boju.


ČIŠĆENJE PODATAKA
moguće je da u podatcima nedostaju neke vrijednosti, koje u učitanom `data.frame`-u poprimaju vrijednost `NA`.

Kako ćemo tretirati nedostajuće vrijednosti ovisit će prvenstveno o samom datasetu, odnosno kontekstu podataka.

U našem specifičnom slučaju, ne uklanjamo redove jer svaki redak predstavlja jednu državu. Ne eliminiramo stupce jer je postotak nedostajućih vrijednosti relativno nizak u usporedbi s ukupnim brojem podataka; umjesto toga, zamjenjujemo nedostajuće vrijednosti s medijanom regije kojoj pripada određena država.
