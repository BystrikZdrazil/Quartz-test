```dataviewjs

var a = moment("2024-10-15");
var b = moment("2024-11-26");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `**ZEK SPOLOČNÉ ZADANIE**     <progress style="height:10px;width:20%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** 
	| `
	html += +p+` days remaining` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%** 
	| `+ p + ` days remaining`
} else if (r==q) {
	html += `   
	Ends today`
} else if (r>q) {
	html += `   
	Ended `+-p+` days ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```


# HOSPODÁRSKE A OBCHODNÉ PRÁVO

## (HOPR)

8. prednáška

Vyučujúci:JUDr.Mária Veterníková, PhD.

Katedra obchodného práva OF EUBA

# OBCHODNÉ ZÁVÄZKOVÉ VZTAHY

# POJEM OBCHODNÉ ZÁVÄZKOVÉ VZTAHY

Obchodnými záväzkovými vzťahmi všeobecne rozumieme záväzkové vzťahy upravené OBZ.

Každý záväzkový právny vzťah, teda aj obchodnýzáväzkový vzťah sa vyznačuje týmito spoločnými znakmi:

·ide o právny vzťah, z ktorého veritel'ovi vzniká právo na plnenie od dlžníka (pohľadávka) a dlžníkovi vznikápovinnosť plnit záväzok

·ide o relatívny právny vzťah, ktorý vzniká medzi konkrétnymi subjektmi, teda medzi veriteľom a dlžníkom

·musí mať aspoň dva subjekty, ako aj dve strany

## DRUHY

## OBCHODNÝCH ZÁVÄZKOVÝCH VZTAHOV

Obchodné záväzkové vzťahy možno deliť na tieto druhy:

.relatívne obchodné záväzkové vzťahy

·absolútne obchodné záväzkové vzťahy

.fakultatívne obchodné záväzkové vzťahy

RELATÍVNE

# OBCHODNÉ ZÁVÄZKOVÉ VZTAHY

Za relatívne obchodné záväzkové vzťahy sa považujú tieto záväzkové vzťahy:

·záväzkové vzťahy medzi podnikatel'mi navzájom, ak pri ich vzniku je zrejmé s prihliadnutím na všetky okolnosti, že sa týkajúich podnikatelskej činnosti

·záväzkové vzťahy medzi podnikatel'om pri jeho podnikateľskej činnosti a subjektom verejného práva (napr. štátny orgán, obec), ak sa týkajú zabezpečovania verejných potrieb alebo vlastnej prevádzky.

## ABSOLÚTNE

# OBCHODNÉ ZÁVÄZKOVÉ VZTAHY

môžeme rozdeliť do troch skupín:

·záväzkové vzť'ahy týkajúce sa obchodných spoločností

·záväzkové vzť'ahy týkajúce sa družstiev

·záväzkové vzťahy vznikajúce z nasledujúcich právnych úkonov:

1. záväzkové vzťahy z burzových obchodov a ich sprostredkovania, z odplatných zmlúv týkajúcich sa cenných papierov,

2. záväzkové vzťahy vznikajúce z taxatívne vymenovaných typov zmlúv (napr. zmluvy o úvere)

3. záväzkové vzťahy z bankovej záruky, z cestovného šeku a sľ'ubu odškodnenia.

## FAKULTATÍVNE

# OBCHODNÉ ZÁVÄZKOVÉ VZTAHY

Fakultatívnymi obchodnými záväzkovými vzťahmi sú tie obchodnoprávne vzťahy, ktorých obchodnýcharakter je založený dohodou strán.

Takáto dohoda sa musí urobiť v písomnej forme.

## SPOLOČNÉ

# OBCHODNÉ ZÁVÄZKOVÉ VZTAHY

Ak na strane veriteľ'a, ako aj na strane dlžníka vystupuje jeden subjekt (účastník) hovoríme o jednoduchom záväzkovom vzťahu.

Ak je na jednej alebo na oboch stranách záväzkového vzťahu viac subjektov

(účastníkov), hovoríme o spoločných záväzkových právnych vzťahoch alebo o spoločných záväzkoch a spoločných právach.

# DRUHY SPOLOČNÝCH

# OBCHODNYCH ZÁVÄZKOV

Spoločným záväzkom je taký záväzok, pri ktorom na jednej strane alebo na obidvoch stranách záväzkového právneho vzťahu vystupuje viac účastníkov, t.j. viac dlžníkov alebo viac veritelov.

Spoločné obchodné záväzky rozlišujeme na:

## .solidárne záväzky

.nedeliteľné záväzky (predmet plnenia musí byťsplnený naraz, nie je možné plniť po častiach,napr. zhotovenie sochy)

·delené záväzky predpokladom ich vzniku je deliteľné plnenie

## zÁKLADNÉ ZÁSADY

## OBCHODNÝCH ZÁVÄZKOVÝCH VZTAHOV

·zásada zmluvnej slobody

·zásada rovnosti zmluvných strán

·zásada bezformálnosti právnych úkonov

·zásada “dohody sa majú dodržiavat”

·zásada dobrej viery

·zásada profesionality

·zásada poctivého obchodného styku-ide o poctivé a slušné správanie podnikatelov vo vzájomnych vzťahoch, ale aj vo vzťahoch s iným subjektami

## VZNIK

## OBCHODNÝCH ZÁVÄZKOVÝCH VZTAHOV

# Obchodné záväzkové vzťahy vznikajú z

·právnych úkonov (najmä zo zmlúv)

·protiprávnych úkonov (napr. spôsobenie škody)

·iných skutočností predpokladaných zákonom (napr. vznik ručenia pri obchodných spoločnostiach)

# UZAVIERANIE OBCHODNÝCH ZMLÚV

Proces vzniku zmluvy sa skladá z dvoch jednostranných právnych úkonov,a to:

·návrh na uzavretie zmluvy

·prijatie návrhu na uzavretie zmluvy

OBZ v ustanovených prípadoch umožňuje postupnéuzavieranie zmluvy, teda také, že sa zmluvné strany dohodnú, že:

- dodatočne si určia obsah záväzku - napríklad termín plnenia

- dodatočne si dohodnú nepodstatnú časť zmluvy (v prípade vyhotovenia napr. znaleckého posudku) s dojednaním, že ak k tomu nedôjde, zmluva nevznikne

- chýbajúci obsah zmluvy doplní súd alebo tretia osoba určená v zmluve

# VEREJNÝ NÁVRH NA UZAVRETIE ZMLUVY

Verejný návrh na uzavretie zmluvy predstavuje osobitnýspôsob uzavierania obchodných zmlúv, pri ktorom ide o prejav vôle, ktorým sa navrhovateľ obracia na neurčitéosoby s cielom uzavretia zmluvy.

Verejný návrh

·musí obsahovať podstatné časti zmluvy a pri nepomenovaných zmluvách musí obsahovaťdostatočné určenie záväzku

·musí byť' zverejnený

Proces uzavretia zmluvy na základe verejného návrhu pozostáva z troch právnych úkonov, a to návrhu, prijatia návrhu a potvrdenia.

## OBCHODNÁ VEREJNÁ SÚTAŽ

je ďaľším osobitným spôsobom uzavierania obchodných zmlúv,pri ktorom je neurčitým osobám adresovanávýzva na podávanie návrhov na uzavretie zmluvy.

Cieľ'om tejto súťaže je zabezpečiť výber najvhodnejšieho návrhu na uzavretie určitej obchodnej zmluvy.

Vyhlasovatel' vyberie najvhodnejší návrh z predložených návrhov a oznámi jeho prijatie spôsobom a v lehote, ktoré určujú podmienky súťaže.Zmluva je uzavretá okamihom dôjdenia vyjadrenia o prijatí návrhu navrhovateľovi.

## ZMLUVA O UZAVRETÍ BUDÚCEJ ZMLUVY

je dohoda,ktorou sa jedna alebo obe zmluvnéstrany zaväzujú uzavrieť v určitej dobe budúcu zmluvu s predmetom plnenia, ktorý je určenýaspoň podstatným spôsobom.

## Podstatnými obsahovými náležitosťami zmluvy sú:

·záväzok uzavrieť budúcu zmluvu

·doba,do ktorej bude budúca zmluva uzavretá

·predmet plnenia budúcej zmluvy

Zmluva o budúcej zmluve musí mať písomnúformu.

## ZABEZPEČENIE

## OBCHODNÝCH ZÁVÄZKOVÝCH VZTAHOV

Inštitút zabezpečenia záväzkov patrí do skupiny osobitných súkromnoprávnych prostriedkov ochrany subjektívnych práv a povinností vznikajúcich v rámci záväzkových vzťahov.

Ciel'om právnych prostriedkov zabezpečenia záväzkov je posilniť postavenie veriteľa, a tým zabezpečiť splnenie jeho pohľadávky.

V tretej časti OBZ sú upravné tieto zabezpečovacie prostriedky: 1. zmluvná pokuta

2. ručenie

3. banková záruka

4. uznanie záväzku

## FUNKCIE

# ZABEZPECOVACICH PROSTRIEDKOV

# Zabezpečovacie prostriedky plnia tieto funkcie

·preventívnu funkciu; spočíva v predchádzaníohrozeniu a porušeniu právom chranených vzťahov

·zabezpečovaciu funkciu; poskytuje veriteľovi posilnenie jeho práv na budúce plnenie; dlžníka zároveň motivuje k dobrovoľnému splneniu záväzku,

· uhradzovaciu funkciu; spočíva v tom, že ak zabezpečená povinnosť nebude včas a riadne splnená, pohľadávku veriteľa možno uspokojiťprostredníctvom zabezpečenia

·represívnu funkciu; je sankciou za porušenie záväzku; platňuje sa výnimočne, napr. pri zmluvnej pokute

## ZMLUVNÁ POKUTA

Zmluvnou pokutou rozumieme dohodou určenéplnenie, ktoré je povinná poskytnúť zmluvnástrana, ktorá poruší zmluvnú povinnost'.

Obligatórnymi obsahovými náležitosťami dohody o zmluvnej pokute sú:

·označenie zmluvných strán

·určenie povinnosti, ktorej splnenie má zmluvnápokuta zabezpečiť

·určenie výšky zmluvnej pokuty alebo spôsobu jej určenia

Dohoda o zmluvnej pokute musí byť písomná.

## RUČENIE

Ručenie je právny vzťah medzi veriteľom a ručiteľom, t.j. osobou, ktorá veriteľovi vyhlási, že ho uspokojí, ak dlžník nesplní jeho záväzok.

Ručením možno zabezpečiť len platný záväzok alebo jeho časť, možno ním zabezpečiť aj záväzok, ktorý vznikne v budúcnosti,alebo ktorého vznik závisí od splnenia podmienky.

Ručenie môže vzniknúť nielen dobrovoľne na základe písomného vyhlásenia ručiteľ'a, ale aj na základe zákona (napr. podľ'a § 59 ods. 7 OBZ po zániku spoločnosti ručia spoločníci za záväzky spoločnosti do výšky svojho podielu na likvidačnom zostatku, najmenej však v rozsahu, v ktorom za ne ručili za trvania spoločnosti)

# BANKOVÁ ZÁRUKA

Bankovou zárukou rozumieme záväzok banky voči veriteľovi, že ho uspokojí podľa záručnej listiny, ak dlžník svoj záväzok nesplní.

Banková záruka vzniká jednostranným právnym úkonom ručiteľa, ktorým je vystavenie záručnej listiny bankou.

Záručná listina musí mať písomnú formu a musíobsahovať tieto náležitosti:

·záväzok banky,že uspokojí veriteľa,

·označenie dlžníka a jeho záväzok, za ktorý banka preberá bankovú záruku

·uvedenie sumy, za ktorú banka ručí

## UZNANIE ZÁVÄZKU

Uznanie záväzku je jednostranným právnym úkonom dlžníka adresovaným veriteľom,ktorýzakladá vyvratiteľnú právnu domnienku, že záväzok v uznanom rozsahu v čase uznania záväzku trval.

## Uznať možno

## ·existujúci záväzok

·premlčaný záväzok; od okamihu uznania záväzku začne plynúť nová štvrročná premlčacia doba,pričom premlčacia doba sa skončí najneskôr po uplynutídesiatich rokov odo dňa, keď začala plynúť prvý raz.

Uznanie záväzku musí mať písomnú formu.

# DAKUJEM VAM ZA POZORNOST

## JUDr. Mária Veterníková,PhD.



