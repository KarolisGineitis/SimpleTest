# Paskaita 1

# Paskaita 2
###Komandinės eilutės įrankiai

Pagal Unix filosofiją, programuojant reikia kurti ir naudoti įrankius - paprastas programas, kurios daro vieną darbą ir jį daro gerai.
Tad toliau bus pateikiamos programos, kurias tenka dažnai naudoti rašant scenarijus ar dirbant terminale, ir trumpi jų paaiškinimai.


####Karšti klavišai

`<ctrl><c>`  - siunčia signalą **SIGINT** procesui, siekiant jį nutraukti. Šis signalas gali būti sulaikytas proceso, todėl jis turi galimybę tvarkingai baigti darbą arba nebaigti darbo.
`<ctrl><z>`  - siunčia signalą **SIGSTOP** procesui, siekiant jį pristabdyti (*suspend*). Šis signalas negali būti sulaikytas, todėl procesas visada yra sulaikomas.

####Informacija apie komandas

**man**- sintaksė: ***$man [KOMANDOS_PAVADINIMAS]*** ; parodo nurodytos komandos naudojimo instrukciją

####Failų peržiūros komandos

**cat** - sintaksė: ***$cat [FAILO_PAVADINIMAS]*** ; nuskaito informaciją iš failo ir ją pateikia kaip išvesties duomenis.

**less** - sintaksė: ***$less [FAILO_PAVADINIMAS]*** ; nuskaito informaciją iš failo ir ją pateikia po vieną puslapį, todėl veikia greičiau, nes neskaito viso failo iškart.

####Failų sistemos informacija

**ls** - sintaksė: ***$ls [PARAMETRAS] [KATALOGAS]*** ; išrašo katalogo turinį terminale. Keli naudingi parametrai : -la (pateikia duagiau informacijos apie failą ir parodo paslėptus failus), -t (išrykiuoja pagal laiką).

**cd** - sintaksė: ***$cd [KATALOGAS]*** ; pakeičia aktyvų(darbo) katalogą.

**pwd** - sintaksė: ***$pwd*** ; terminale išspausdina aktyvaus(darbinio) katalogo kelią.

**chmod** - sintaksė: ***$chmod [NUORODA][OPERATORIUS][BŪSENA] [FAILO_PAVADINIMAS]*** ;  pakeičia failo naudojimo gaireles. *NUORODA* (u-failo savininkas, g-savininko grupė, o-kiti vartotojai ) *OPERATORIUS* (+ prideda būsenas , - pašalina būsenas ) *BŪSENA* ( r-leidimas skaityti, w-leidimas rašyti, x-leidimas vykdyti ).  

**whereis** - sintaksė: ***$whereis [FAILO_PAVADINIMAS]*** ; suranda failus (pirminius) ir išspausdina ju kelią.

**mv** - sintaksė: ***$mv [PIRMAS_FAILAS] [ANTRAS_FAILAS]*** ; perkelia informaciją iš PIRMAS_FAILAS į ANTRAS_FAILAS ir pašalina PIRMAS_FAILAS

Informacijos šaltiniai :

* https://superuser.com/questions/262942/whats-different-between-ctrlz-and-ctrlc-in-unix-command-line

* https://www.rapidtables.com/code/linux/ls.html

* https://www.geeksforgeeks.org
# Paskaita 3

# Paskaita 4
###Unix failų sistema

Unix failų sistema yra loginis didelių informacijos kiekių organizavimo ir laikymo metodas. Jis padeda nesunkiai valdyti kompiuterinę sistemą. Failas yra šios saugojimo sistemos mažiausias blokas. Jį neformaliai galima apibrėžti kaip informacijos (dažniausiai susijusios) rinkinį, kuris gali būti logiškai peržiūrimas kaip baitų srautas.Failų sistema ne tik leidžia organizuoti informaciją, bet ir suteikia įrankius, leidžiančius failus keisti. Taip pat ji pasirūpina logiškos organizacijos susiejimu su išoriniais (fiziškais) prietaisais.
 
Unix failų sistemos ypatumai :
 * *Visa informacija yra laikoma failuose.*
 *  *Visi failai yra organizuojami į katalogus.*
 * *Šie katalogai yra susiejami į medį primenančią struktūrą.*

Šis "medis" yra sukuriamas vadovaujantis tam tirka hierarchija. Aukščiausias katalogas yra vadinamas **root** (*žymimas pasvyruoju brukšniu* ' / '). Po juo yra keli pakatalogiai, kurių dauguma skirta laikyti sistemos failams. Giliau šiuose pakatalogiuose galime rasti programų failus ir/arba vartotojo sukurtus failus.

***Failų tipai***

Iš vartotojo perspektyvos, Unix sistemoje viskas yra laikoma failais. Pavyzdžiui spausdintuvai ar diskai.
Taip gali būti, nes visa informacija iš esmės yra baitų srautas. Visi failai Unix sistemoje gali būti suskirtyti į 3 kategorijas :
 * *paprasti failai*
 * *katalogų failai*
 * *prietaisų failai*
Paprasti failai susideda iš informacijos srautų, saugomų kažkokiame atminties įtaise. Tokių failų pavyzdžiai yra paprasti tekstiniai failai, programų informacijos failai, vykdomieji failai.
Katalogų failai yra lyg talpyklos kitiems failams. Todėl jie nesaugo kažkokios vartotojui suprantamos informacijos, o laiko nuorodas į failus, esančius kataloguose.
Prietaisų failai yra naudojami aprašyti fizinį įtaisą. Jie nelaiko jokios informacijos, o tik atvaizduoja informaciją, gaunamą iš prietaiso.

**Informacijos šaltiniai : **
 homepages.uc.edu/~thomam/Intro_Unix_Text/File_System.html
 https://www.geeksforgeeks.org/unix-file-system/
# Paskaita 5

# Paskaita 6
