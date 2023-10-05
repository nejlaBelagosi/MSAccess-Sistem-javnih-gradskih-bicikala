# MSAccess-Sistem-javnih-gradskih-bicikala

## Opis projekta
Projektovani sistem ima za cilj da korisnicima omogući upotrebu mreže bicikala, administrativnom osoblju omogući uvid u korištenje mreže i menadžerima omogući korištenje opcija za izvještavanje o poslovanju, serviserima olakša posao servisiranja mreže, korisnicima lakšu registraciju i korištenje gradskih bicikala. Svrha IS-a jeste u smanjenju troškova poslovanja, promovisanje zdravijeg načina života, povećanje broja korisnika, efikasnija upotreba vremena za korisnike sistema. Ciljevi koje obuhvata ovaj sistem leže u elektronskoj evidenciji bicikala, online rezervaciji bicikala, elektronskoj evidenciji korištenja mreže, evidenciji svih korisnika kao i praćenje lokacije svih bicikala. Također korisnicima omogućena i efikasnija naplata u cilju povećanja dostupnosti i efikasnosti upravljanja. Pomoću ovog sistema uz iznajmljivanje moguća je i rezervacija bicikala, a postoji i opcija za prijavu kvara istih.  Ovaj sistem koristit će odjeli za administraciju, servisiranje kao i sami klijenti. Prednosti ovog sistema su:
-	laka i jednostavna upotreba
-	omogućen je uvid u zalihe bicikala 
-	ušteda vremena jer je smanjen ručni rad 
-	brz pregled dostupnosti bicikala 
-	upravljanje i evidencija bicikala
-	generisanje velike količine podataka 
-	dostupan i prilagodljiv na svim uređajima (android i ios) itd.

## Specifikacija funkcionalnosti
<table>
  <tr>
    <th>ULOGA (CILJ)</th>
    <th>FUNKCIJE</th>
  </tr>
  <tr>
    <td>	Obezbjeđenje tačnih i blagovremenih informacija o dostupnim biciklima <br>
          Elektronska evidencija bicikala <br>
Online rezervacija bicikala <br>
Elektronska evidencija korštenja mreže <br>
Evidencija svih korisnika sistema <br>
Praćenje lokacije bicikala <br>
</td>
    <td>FUNKCIJE	Uvid u svakodnevne izvještaje različitih sadržaja <br>
Izdavanje potvrda/napomena kao dokaz o izvršenim rezervacijama/prijavama <br>
Prikupljanje svih potrebnih podataka o korisnicima, serviserima, biciklima <br>
Omogućavanje online uplaćivanja
</td>
  </tr>
</table>

## Specifikacija komponenti

<table>
  <tr>
    <th>Hardware</th>
    <th>Software</th>
    <th>Dataware</th>
    <th>Netware</th>
    <th>Orgware</th>
    <th>Lifeware</th>
  </tr>

  <tr>
    <td>Računari i računarske oprema koji služe za unos podataka o biciklima i izradu IS-a <br>
Mobiteli koji su potrebni korisnicima kako bi se registrovali na IS <br>
Ruteri, Aplikacioni server, Database server, Switch, cell tower, SMSC <br>
Printeri koji služe za printanje izvještaja <br>
GPS uređaji koji služe za prećenje bicikala <br>
Telefon za pružanje podrške korisnicima <br>
</td>
    <td>DMS kao digitalna dokumentacija koja predstavlja baze podataka <br>
Microsoft Office paket npr. Word, Excel, Access itd. <br>
Pogrami koji su potrebni za ispisivanje koda npr. MS Visual Code <br>
Jezici koji su potrebni za izradu mobilne aplikacije npr. Swift, C#, C++, Java, MySQL, Python itd. <br>
Mobilna aplikacija <br>
Elektronska pošta npr. Gmail ili text messaging service SMS putem kojih se šalju izvještaji o rezervaciji, uplati itd. <br>
Software za zaštitu od DDOS napada i njemu sličnih <br>
</td>
    <td>Dataware	Svi potrebni i validni podaci o klijentima ( e-mail, ime, prezime, država, grad, broj telefona, lozinka, datum rođenja itd.) <br>
Podaci o biciklima (opis bicikala, tj. Tip bicikla, šifra lokota, da li je biciklo dostupno, da li je u kvaru, na kojoj stanici se nalazi, identifikacioni broj <br>
Podaci o rezervaciji ( da li je poništena, do kada vrijedi, da li je iskorištena itd.) <br>
Podaci o stanici ( lokacija stanice, koliko ima raspoloživih bicikala, stanica) <br>
Podaci o vožnji ( vrijeme početka vožnje, vrijeme završetka vožnje, stanica na kojoj je završena vožnja, koje je biciklo bilo iskorišteno, klijent koji je vozio biciklo) <br>
Podaci o uplati ( iznos uplate, datum uplate i o klijentu koji je izvršio uplatu) <br>
Podaci o serviseru (ime, prezime, telefonski broj, JMBG) <br>
Podaci o servisu ( opis popravke, datum servisa, biciklo koje je servisirano, serviser koji je obavljao popravku itd.) <br>
</td>
    <td>Potreban nam je Wi-Fi kako bi se izvještai poslali preko elektronske pošte, API</td>
    <td>Analiza sistema, potrebni frameworks kao npr. .NETframework, stručan IT kadar</td>
    <td>Klijenti <br>
Administrativno osoblje <br>
Serviseri <br>
Pravni tim <br>
Ekonomisti i menadžeri <br>
Marketinški tim <br>
IT odjel <br>
Tehnička podrška <br>
Poslovni stručnjaci <br>
Generalni direktor <br>
</td>
  </tr>
</table>

## Model arhitekture informacionog sistema
Ovaj model arhitekture izabran je iz razloga što ovaj sistem čini veći broj podsistema, tako npr. imamo jedan od sistema jeste sistem za online rezervaciju bicikla, onda sistem za podršku mreže, moguć je razviti i sistem o servisiranju, nabavci bicikala, o tehničkoj podršci klijentima itd.
Koristi se troslojni model arhitekture. Tri sloja koja su u upotrebi su:
-	prezentacijski,
-	sloj poslovne logike i 
-	sloj baze podataka.
![image](https://github.com/nejlaBelagosi/MSAccess-Sistem-javnih-gradskih-bicikala/assets/122165597/866fa688-50c0-445e-b76d-f43a55113466)

## Model arhitekture mreže
Interni korisnici se nalaze sa iste strane firewalla kao i aplikacijski i database serveri, dok se eksterni korisnici (klijenti i serveri) nalaze sa druge strane. Eksterni korisnici pristupaju pomoću aplikacije na smart telefonu, a interni pomoću web browsera.
![image](https://github.com/nejlaBelagosi/MSAccess-Sistem-javnih-gradskih-bicikala/assets/122165597/f61b473a-5cd2-4405-90a7-82b1dad91517)

## Gantogram
![image](https://github.com/nejlaBelagosi/MSAccess-Sistem-javnih-gradskih-bicikala/assets/122165597/dc9e1c9c-9c27-478e-9183-bfa29848ecc3)



