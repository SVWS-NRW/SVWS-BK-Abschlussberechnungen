
# ABITUR-Berechnungen BK Anlage D 

Die Abiturprüfung (Block II) erfolgt in mehreren Schritten und wird vom Allgemeinen Prüfungsaussschuss (APA) 
organisiert und überwacht. 

Folgende Schritte werden beim Abitur durchlaufen:
1. Zulassung zum Abitur (1. Sitzung des APA)
2. Auswertung der Abiturergebnisse und Festlegung von mündlichen Prüfungen (2. Sitzung des APA)
3. Feststellung der Abiturergebnisse nach der mündlichen Prüfung (3. Sitzung des APA)

## Wahl der Abiturfächer für das 3. und 4. Fach
Am BK sind die möglichen Fächer in der Abiturprüfung an den Bildungsgang gebunden. 

### Kriterien für die zulässige Wahl des dritten und vierten Abiturfachs
1. Die beiden Fächer müssen eine zulässige Kombination aus der in der APO-BK für jeden Bildungsgang festgelegten möglichen Kombinationen sein.
2. In beiden Fächern müssen ab Beginn der 12.1 Klausuren geschrieben worden sein.

## Zulassung zur Abiturprüfung

### Zu berücksichtigende Halbjahre und Daten

Es sind die Leistungsdaten der vier gewerteten Halbjahre der Qualifikationsstufen Q1 und Q2 zu betrachten.
Wiederholte Halbjahre bleiben unberücksichtigt. Es ist auch möglich am Ende der 13.1 in die 12.2 zurück zu gehen.

Die Sprachenfolge mit Fächern und Belegungszeiträumen

### Einbringen von Kursen
Folgende Kurse werden in das Abitur eingebracht mit den beiden Bedingungen das bestmögliche Kurse gewählt werden und Kurse mit 0 Punkten nicht eingebracht werden können:
  1. die 8 Leistungskurse
  2. die 8 Kurse der weiteren 2 Abiturfächer
  3. KurseAuffüllen (4, Deutsch)
  4. KurseAuffüllen (4, Mathematik)
  5. KurseAuffüllen (4, Naturwissenschaft ab 11.1)
  6. KurseAuffüllen (2, Gesellschaftslehre mit Geschichte)
  7. KurseAuffüllen (4, gesellschaftswissenschaftliches Aufgabenfeld)
  8. KurseAuffüllen (4, fortgeführte oder ab 11.1 Fremdsprache)
  9. KurseAuffüllen (2, neu einsetzende Fremdsprache, falls keine 2. FS in Sek-I 4 Schuljahre am Stück)<br>Für das Einbringen der Fremdsprachen müssen die gültigen Kombinationen ausgerechnet werden und die beste Kombination gewält werden. Siehe dazu:  https://git.svws-nrw.de/svws/SVWS-Server/-/issues/2158<br>
  10. KurseAuffüllen (32)
  11. KurseAuffüllen (40 inkl. der Facharbeit, wobei diese für 2 Kurse zählt, solange Kurspunkte größer als bisheriger Durchschnitt)

### Kriterien für die Zulassung
1. Teilnahme am Unterricht in den Fächern der Stundentafel des jeweiligen Bildungsgang.
2. Die Abiturfächer sind in der Kombination für den Bildungsgang zulässig und es wurden seit Beginn der 12.1 Klausuren geschrieben.
3. eingebrachtSindKursart(4, LK1)
3. eingebrachtSindKursart(4, LK2)
3. eingebrachtSindKursart(4, AB3)
3. eingebrachtSindKursart(4, AB4)
4. eingebrachtSindFach(4, Deutsch)
4. eingebrachtSindFach(4, Mathematik)
4. eingebrachtSindFach(2, Gesellschaftslehre mit Geschichte)
5. eingebrachtSindAufgabenfeld(4, Gesellschaftswissenschaft)
6. eingebrachtSindFachgruppe(4, Naturwissenschaft, ab 11.1)
7. eingebrachtSindFS(4, fortgeführte oder ab 11.1 Fremdsprache)
7. eingebrachtSindFS(2, ab 11.1 Fremdsprache, nur wenn keine 2. FS in Sek1)
8. eingebrachtSind(32, ohne Facharbeit)
9. eingebrachtSindMaximal(40, Facharbeit zählt doppelt)
10. punkteErreicht(200, nach Formel im § 25 Abs. 3)
11. defizitePrüfen( 32, 32, 6, 3) anzVon, anzBis, maxDefiziteGes, maxDefizitLK
11. defizitePrüfen( 33, 37, 7, 3)
11. defizitePrüfen( 38, 40, 8, 3)
12. zweiteFSNichtNull(4, ab 12.1 Fremdsprache, nur wenn keine 2. FS in Sek1)

## Ermitteln der Bestehensprüfungen
Nach der Abiturprüfung im ersten bis vierten Abiturfach muss festgestellt werden ob die Abiturprüfung (Block II) bestanden ist. Wenn diese nicht bestanden ist, müssen Bestehensprüfungen angesetzt werden. (APO-BK Anlage D § 21 Abs. 3)

### Ermitteln ob Abiturprüfung bestanden ist (§ 25 Abs. 4)
1. Punktesumme5fach(LK1, LK2, AB3, AB4) oder <br>
   Punktesumme4fach(LK1, LK2, AB3, AB4, BLL)
2. mindestPunktzahlErreicht(Punktsumme, 100)
3. mindestPunktzahlErreicht(LK[], 5, 1) kurse, mindestPunkteEinfach, anzahlKurse
4. mindestPunktzahlErreicht(ABI[], 5, 2)

### Bestehensprüfungen festlegen (§ 21, § 25 Abs. 4)
Bestehensprüfungen werden nur im ersten bis dritten Abiturfach angesetzt! <br>
Folgende Fälle sind zu unterscheiden:
1. Mindestpunktzahl Block II ist erreicht oder mittelbar erreicht<br>
   Dann werden nur die Bestehensprüfungen in den ersten drei Abiturfächern angesetzt, in denen keine fünf Punkte in einfacher Wertung erreicht wurden. 
    1. Die Punkte sind direkt erreicht
    2. Die Punkte werden in jedem Fall erreicht, wenn die Bedingung erreicht ist, dass mindestens ein LK fünf Punkte hat und höchstens zwei Prüfungsteile unter fünf Punkte sind.
2. Mindestpunktzahl Block II ist nicht erreicht auch nicht mittelbar<br>
   In allen schriftlichen Abiturfächern wird eine mündliche Bestehensprüfung angesetzt.

## Feststellen der Abitur-Prüfungsergebnisse (§ 24, §25)
In der letzten APA-Konferenz (3.) wird das Gesamtergebnis der Abiturprüfung festgestellt.

### Bestehen prüfen
Bestehen wird entsprechend den oben genannten Bedingungen geprüft.
Wenn das Abitur nicht bestanden wird, wird keine Durchschnittsnote berechnet und das Abiturergebnis auf "Nichtbestanden" gesetzt.

### Berechnung der Abitur-Gesamtpunktzahl
Die Gesamtpunktzahl ergibt sich aus den Punkten im Block I (Qualifikationsphase) und im Block II (Abiturprüfung).

#### Punkte im Block I
Die Punkte ergeben sich aus der Summe der eingebrachten Kurse.
1. Punktsumme __P__ bilden
   - doppelte Punktzahl der vier Leistungskurse
   - einfache Punktzahl der eingebrachten Grundkurse
   - doppelte Punktzahl einer eingebrachten Facharbeit
2. Kursanzahl __K__ ermitteln
   - 16 für 8 doppelt gewichtete LKs
   -  2 falls eine Facharbeit eingebracht wird
   - GK Anzahl der eingebrachten Grundkurse
3. Punkte normieren auf 40 eingebrachte Kurse
   - __EI__ = Ergebnis Block I
   - __EI__ = __P__ / __K__ * 40

### Punkte im Block II
 1. Faktor __F__ festlegen<br>
    4 : besondere Lernleistung eingebracht<br>
    5 : keine besondere Lernleistung eingebracht<br>
 
 2. Ergebnis __ET__ jedes Prüfungsteils <br>
    - falls mündliche Prüfung (nur 1. bis 3. Fach)<br>
      __ET__ = (2s + m) / 3 * __F__ (s=schriftl, m=mündl.)<br>
      Ergebnis kaufmännisch runden.
    - ohne mündliche Prüfung<br>
      __ET__ = p * __F__ (p = erreichte Punkte im Prüfungsteil)
 
 3. Summe __EII__ aus allen __ET__ der Prüfungsteile bilden

### Ermittlung der Abitur-Durchschnittsnote
Die Durchschnittsnote des Abiturs wird wie folgt ermittelt:
1. Note berechnen nach der Formel:
   N = 5,666 - ((__EI__ + __EII__) / 180)
2. Nach der ersten Nachkommastelle wird abgeschnitten.
3. Ein Notenwert kleiner 1,0 ist nicht zulässig und wird auf 1,0 korrigiert.


## Referenzen zur APO-BK
- APO-BK Anlage D § 6
  >__Wahl der Abiturprüfungsfächer__<br>
Eine Schülerin oder ein Schüler legt die Abiturprüfung in vier Fächern
ab. Das erste und zweite Fach der Abiturprüfung sind die in
den Anmerkungen zur Stundentafel des Bildungsganges als erstes
und zweites Abiturprüfungsfach festgelegten oder zur Wahl gestellten
Fächer. Das dritte und vierte Abiturprüfungsfach legt die Schülerin
oder der Schüler zu Beginn der Jahrgangsstufe 13.1 fest. Dabei
muss es sich um die in den Anmerkungen zur Stundentafel als drittes
beziehungsweise viertes Abiturfach ausgewiesenen Fächer handeln,
in denen spätestens vom Beginn der Jahrgangsstufe 12.1 an
Klausuren geschrieben wurden.
- APO-BK Anlage D § 15 Abs. 2
	>(2) Zugelassen wird, wer am Unterricht der Jahrgangsstufen 12 und
13 gemäß der für den Bildungsgang gültigen Stundentafel teilgenommen
hat und im Grund- und Leistungskursbereich der Qualifikationsphase
(Block I) folgende Bedingungen erfüllt:
    >1. Es müssen mindestens 32 und höchstens 40 Kurse, darunter die
acht Leistungskurse, eingebracht werden. Werden mehr als 32 Kurse
eingebracht, kann ein Kurs durch eine Facharbeit nach Absatz 4
Nummer 3 ersetzt werden.
    >2. Es müssen mindestens 200 Punkte gemäß § 25 Absatz 3 erreicht
werden.
    >3. Von den gemäß Nummer 1 eingebrachten Kursen dürfen<br>
      a) bei Einbringung von genau 32 Kursen nicht mehr als sechs,<br>
		  b) bei Einbringung von 33 bis 37 Kursen nicht mehr als sieben und<br>
		  c) bei Einbringung von 38 bis 40 Kursen nicht mehr als acht Kurse<br>
mit weniger als fünf Punkten in einfacher Gewichtung bewertet worden
sein.<br>
Darunter dürfen nicht mehr als drei Leistungskurse sein. Kurse, die
mit null Punkten bewertet worden sind, können nicht eingebracht
werden.
	>4. Schülerinnen und Schüler, die in der Sekundarstufe I keinen
durchgängigen Unterricht in einer zweiten Fremdsprache im Umfang
von mindestens vier Jahren erhalten haben, dürfen zum Erwerb
der allgemeinen Hochschulreife in keinem der vier in der Qualifikationsphase
belegten Kurse der in der Jahrgangsstufe 11 neu
einsetzenden Fremdsprache mit null Punkten bewertet worden sein,
	>5. Inhaltsgleiche Kurse dürfen nur einmal eingebracht werden.

- APO-BK AnlageD § 15 Abs. 3
  >(3) Unter den einzubringenden Kursen im Block I müssen mindestens
sein (Pflichtkurse):
  >1. Jeweils die vier Kurse der vier Abiturprüfungsfächer, die gemäß
der für den Bildungsgang gültigen Stundentafel ausgewiesen sind.
Die Kurse der beiden Leistungskursfächer (1. und 2. schriftliches
Prüfungsfach) werden doppelt gewichtet.
  >2. Soweit nicht bereits als Abiturprüfungsfächer eingebracht:<br>
      a) vier Kurse Deutsch,<br>
      b) vier Kurse der aus der Sekundarstufe I fortgeführten oder der in
der Jahrgangsstufe 11 neu einsetzende Fremdsprache,<br>
      c) vier Kurse Mathematik,<br>
      d) vier Kurse der aus der Jahrgangsstufe 11 fortgeführten Naturwissenschaft,<br>
      e) vier Kurse aus dem gesellschaftswissenschaftlichen Aufgabenfeld,
darunter zwei Kurse des Faches Gesellschaftslehre mit Geschichte
und<br>
      f) zum Erwerb der allgemeinen Hochschulreife ergänzend zwei Kurse
der in der Jahrgangsstufe 11 neu einsetzenden Fremdsprache,
wenn Schülerinnen und Schüler in der Sekundarstufe I keinen
durchgängigen Unterricht in einer zweiten Fremdsprache im Umfang
von mindestens vier Jahren erhalten haben.
  >3. Soweit die Einbringung der (Pflicht-) Kurse nach Nummer 1 und 2
weniger als 32 Kurse in einfacher Gewichtung ergibt, müssen mindestens
so viele weitere Kurse der Qualifikationsphase nach Absatz
4 in den Block I eingebracht werden, dass insgesamt mindestens 32
Kurse in einfacher Gewichtung im Block I berücksichtigt werden
können.

- APO-BK AnlageD § 15 Abs. 3
  >(4) In den Block I können darüber hinaus eingebracht werden
  >1. weitere Kurse der Fächer des berufsbezogenen oder des berufsübergreifenden
Lernbereichs gemäß der für den Bildungsgang gültigen
Stundentafel (Wahlkurse).
  >2. Kurse des Differenzierungsbereichs, die die Anforderungen an
Grundkurse erfüllen (Wahlkurse) und
  >3. eine Facharbeit gemäß § 8 Absatz 2; sie wird doppelt gewichtet.
Insgesamt können bis zu acht Wahlkurse oder bis zu sieben Wahlkurse
und die Facharbeit eingebracht werden.

- APO-BK Anlage D § 21 Abs. 3
  >Mündliche Prüfungen im ersten bis dritten Abiturfach sind anzusetzen,
wenn das Bestehen der Abiturprüfung gefährdet ist, weil die
Mindestbedingungen gemäß § 25 Absatz 4 nicht erfüllt sind.

- APO-BK Anlage D § 25 Abs. 3
  >(3) In Block I sind die Leistungen der Kurse in der Qualifikationsphase
gemäß § 15 einzubringen. Die Gesamtpunktzahl in Block I
wird nach folgender Formel berechnet; das Endergebnis (E I) wird
auf eine ganzzahlige Punktzahl gerundet, wobei ab der Dezimalen 5
aufgerundet wird:<br>
EI = (Punkte der eingebrachten Kurse)/(Anzahl der eingebrachten Kurse) * 40 <br>
Dabei zählen Leistungskurse und die Facharbeit im Zähler wie im Nenner doppelt.

- APO-BK Anlage D § 25 Abs. 4
  >(4)Im Block II werden die Prüfungsleistungen gleich gewichtet:
  >1. Werden im Block II die Prüfungsleistungen in den vier Abiturfächern
(vier Prüfungselemente) eingebracht, so werden die erbrachten
Prüfungsleistungen jeweils fünffach gewichtet. Die Abiturprüfung
hat bestanden, wer mindestens 100 Punkte erreicht hat. Dabei
müssen in mindestens zwei Prüfungsfächern (Prüfungselementen),
darunter einem Leistungskursfach, mindestens 25 Punkte erreicht
worden sein.
  >2. Werden im Block II die Prüfungsleistungen in den vier Abiturfächern
und einer besonderen Lernleistung (fünf Prüfungselemente)
eingebracht, so werden die erbrachten Prüfungsleistungen in den
vier Abiturfächern und der besonderen Lernleistung jeweils vierfach
gewichtet. Die Abiturprüfung hat bestanden, wer mindestens 100
Punkte erreicht hat. Dabei müssen in mindestens drei Prüfungselementen,
darunter einem Leistungskursfach, mindestens 20 Punkte
erreicht worden sein.


## Pseudocode 
Der Pseudocode ist nur etwas überarbeitet und aus der FHR und noch nicht an alles angepasst.
```
//Datenstruktur kurs 
kurs{
  char fach;
  char fachgruppe;
  char kursart; //GK|LK
  bool markiert; //ob schon in Berechnung eingegangen
}

//Funktionen

einbringBedingungen{
   //Bereich, Fach, Fachgruppe, anz, anzG5 //anzG5 = benötigte Kurse mit mind. 5 Pkt.
   { FACH, 'Deutsch', 'Deutsch', 2, 0 },
   { FACH, 'Mathematik', 'Mathematik', 2, 0 },
   { FACHGRUPPE, '*', 'Fremdsprache', 2, 0 },
   { FACHGRUPPE, '*', 'Gesellschaft', 2, 0 },
   { FACHGRUPPE, '*', 'Naturwissenschaft', 2, 0 },
   { LK, '*', 'Leistungskurs', 4, 2 },
   { GK, '*', 'Grundkurs', 11, 7 }
}

boolean abiturBestanden(){
   kurse = eingebrachteKurseBlock1();
   foreach( fb in fachbedingungen ){
     switch( fb.bereich ){
       : FACH
         markiereFach( kurse, fb.Fach, fb.anz );
         break;
       : FACHGRUPPE
         markiereFachgruppe( kurse, fb.Fachgruppe, fb.anz );
         break;
       : LK
         fhrBestanden &= pruefeLK( kurse, fb.anz, fb.anzG5 );
       : GK
         fhrBestanden &= pruefeGK( kurse, fb.anz, fb.anzG5 );
       }
     }
     if ( not fhrBestanden ) {
       return note;
     }
}

double berechneAbiturDurchschnitt(){
   int deutsch=0, mathematik=0, fremdsprache=0, gesellschaft=0, nw=0;
   int lk = 0; int gk = 0;
   int lk5 = 0; int gk5 = 0;
   int punkte;
   bool abiBestanden = true;
   }
   neueNote = berechneDurchschnitt(kurse);
   if ( note == 0.0 OR note > neueNote ) {
     return neueNote;
   } else {
     return note;
   }
}

markiereFach( kurse, fach, anz ){
  int markiert = 0;

  foreach( kurs in kurse ){
    if( !kurs.markiert ) {
      if( kurs.fach == fach ){
        if( markiert < anz ){
          kurs.markiert = true;
          markiert++;
        } else {
          break;
        }
      }
    }
  }
}


markiereFachgruppe( kurse, gruppe, anz ){
  fachgruppeFach{ fach, punkte = 0, anzahl = 0};
  array<fachgruppeFach> fachgrFaecher;

  foreach( kurs in kurse ){
    if( !kurs.markiert ) {
      if( kurs.fachgruppe == gruppe && kurs.punkte > 0 ) {
        fachgrFaecher[kurs.fach].fach = kurs.fach;
        fachgrFaecher[kurs.fach].punkte = kurs.punkte;
        fachgrFaecher[kurs.fach].anzahl++;
      }
    }
  }
 
  bestPkt = 0;
  bestFach = ""; 
  foreach( fgrFach in fachgrFaecher) {
    if( bestPkt < fgrFach.punkte && fgrFach.anzahl == anz ) {
      bestPkt = fgrFach.punkte;
      bestFach = fgrFach.Fach;
    }
  }

  if ( bestFach <> "" ) {
    foreach( kurs in kurse ){
      if ( kurs.fach == bestFach ){
        kurs.markiert = true;
      }
    }
  }
}


pruefeLK( kurse, soll, anzG5 ){
  ist = 0;
  ist5 = 0;
  foreach(kurs in kurse){
    if( kurs.kursart = "LK" ){
      kurs.markiert = true;
      ist++;
      if( kurs.punkte >= 5 ){
        ist5++;
      }
    }
  }

  if ( (ist5 >= anzG5) && (ist == soll) ) {
    return true;
  } else {
    return false;
  }
}


bool pruefeGK( kurse, soll, anzG5 ){
  ist = 0;
  ist5 = 0;
  foreach(kurs in kurse){
    if( kurs.kursart = "GK" ){
      kurs.markiert = true;
      ist++;
      if( kurs.punkte >= 5 ){
        ist5++;
      }
    }
  }

  aktPkt = 15;
  while( (ist < soll) && (aktPkt > 0)){
    foreach(kurs in kurse) {
      if( !kurs.markiert && kurs.punkte = aktPkt ) {
        kurs.markiert = true;
        ist++;
        if( kurs.punkte >= 5 ){
          ist5++;
        }
      }
    }
    aktPkt--;
  }

  if ( (ist5 >= anzG5) && (ist == soll) ) {
    return true;
  } else {
    return false;
  }
}


double berechneDurchschnitt( kurse ) {
  int punkte = 0;  //N = (5.666-P/57)
  int anz0 = 0;
  foreach( kurs in kurse ) {
    if ( kurs.markiert ) {
      if( kurs.punkte == 0 ) anz0++;
      punkte += kurs.punkte;
    }
  }
  if ( anz0 > 0 ) {
    return 0.0;
  } else {
    return 5.6666 - (punkte / 57.0);
  }
}
```



