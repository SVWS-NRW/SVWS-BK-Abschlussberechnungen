
# FHR12-Algorithmus BK Anlage D 

In der Anlage D wird die Fachhochschulreife (schulischer Teil) in der Qualifikationsphase erworben. Hierzu werden zwei *aufeinanderfolgende* Halbjahre ausgewertet um die Erlangung der FHRsT zu festzustellen.

## Bedingungen zum Erwerb des FHR12-Abschlusses

### zu berücksichtigende Halbjahre

Je nach Zeitpunkt des Abgangs sind folgende Halbjahrespaare zu prüfen:
- Am Ende der 12.2 muss 12.1/12.2 ausgewertet werden.
- Am Ende der 13.1 wird 12.1/12.2 und 12.2/13.1 betrachtet.
- Am Ende der 13.2 wird 12.1/12.2, 12.2/13.1 und 13.1/13.2 betrachtet.

### Kriterium für das Bestehen
1. Wenn in einem der genannten Halbjahrespaare die Leistungsanforderungen für die FHR erfüllt sind, wird die FHRsT erworben.
2. In den 4 Leistungskursen darf kein Kurs 6 sein 
3. In den 4 Leistungskursen müssen insgesamt 20 Punkte erreicht worden sein. (40 bei Doppelgewichtung)
4. Mindestens zwei Leistungskurse müssen jeweils 5 Punkte haben.
5. in den 2 Halbjahren müssen 11 Grundkurse belegt sein, von denen keiner 0 Punkte hat und die insgesamt mindestens 55 Punkte erbringen.
6. Mindestens sieben der elf Grundkurse müssen mindestens 5 Punkte aufweisen.
7. Unter den insgesamt genannten Kursen müssen sein:
   - 2 x Deutsch 
   - 2 x Fremdsprache
   - 2 x Gesellschaftswissenschaft , Aufgabenfeld 2
   - 2 x Mathematik
   - 2 x Naturwissenschaft (2 x Biologie oder 2 x Chemie oder 2 x Physik)
8. Ein Fach darf mit maximal 2 Kursen vertreten sein.

## Berechnung der FHR-Durchschnittsnote

1. Summe bilden aus:
   - doppelte Punktzahl der vier Leistungskurse
   - einfache Punktzahl der elf Grundkurse
2. Note berechnen nach der Formel:
   N = 5,666 - (Summe / 57)
3. Nach der ersten Nachkommastelle wird abgeschnitten.
4. Ein Notenwert kleiner 1.0 ist nicht zulässig und wird auf 1.0 korrigiert.


## Referenzen zur APO-BK

- APO-BK AnlageD § 13a Abs. 2
  >(2) Schülerinnen und Schülern, die den Bildungsgang nach der Jahrgangsstufe
12 verlassen, kann der schulische Teil der Fachhochschulreife
bescheinigt werden, wenn folgende Bedingungen in der
Jahrgangsstufe 12 erfüllt sind:
  >1. In den beiden Leistungskursfächern müssen je zwei Kurse belegt
und insgesamt mindestens 40 Punkte der zweifachen Wertung erreicht
sein.
  >2. Es müssen elf Grundkurse belegt und in diesen insgesamt mindestens
55 Punkte der einfachen Wertung erreicht sein.
  >3. Unter den nach Nummern 1 und 2 anzurechnenden Kursen müssen
je zwei Kurse in Deutsch, einer Fremdsprache (§ 4 Absatz 1 und 5),
einer Gesellschaftswissenschaft, Mathematik, einer Naturwissenschaft
(Biologie oder Physik oder Chemie) sein. Außer den genannten
Fächern können aus weiteren Fächern höchstens je zwei Halbjahreskurse
angerechnet werden.
  >4. In zwei der vier anzurechnenden Leistungskurse und in sieben der
elf anzurechnenden Grundkurse müssen jeweils fünf Punkte der einfachen
Wertung erreicht sein. Mit null Punkten bewertete Kurse gelten
als nicht belegt. \
Der Erwerb der Fachhochschulreife erfolgt nach den Bestimmungen
der Gleichwertigkeitsverordnung.

- APO-BK AnlageD § 13a Abs. 3
  >(3) Für abgehende Schülerinnen und Schüler, die am Ende der Jahrgangsstufe
13.1 oder 13.2 den schulischen Teil der Fachhochschulreife
erwerben wollen, gelten die Bedingungen gemäß Absatz 2 mit
der Maßgabe, dass die Gesamtqualifikation insgesamt in zwei aufeinander
folgenden Halbjahren erbracht worden sein muss.

- APO-BK AnlageD § 13a Abs. 4
  >Die Gesamtpunktzahl \[P\] (mindestens 95, höchstens 285 Punkte),
die sich aus der Bewertung der vier Leistungs- und elf Grundkurse ergibt,
wird nach der Formel
in eine Durchschnittsnote \[N\] umgerechnet. Diese wird auf eine Stelle
hinter dem Komma bestimmt; es wird nicht gerundet. Eine Gesamtpunktzahl
über 266 ergibt die Durchschnittsnote 1,0. Die Durchschnittsnote
wird in Ziffern und Buchstaben auf dem Abgangszeugnis
ausgewiesen. Die Formel lautet: N = (5.666-P/57)

## Pseudocode
```
//Datenstruktur kurs 
kurs{
  char fach;
  char fachgruppe;
  char kursart; //GK|LK
  bool markiert; //ob schon in Berechnung eingegangen
}

//Funktionen
berecheneFhr12 { 
  // Note 0.0 bedeutet, nicht bestanden.
  note = 0.0 
  IF ( (jahrgangsstufe * 10 + halbjahr) >= 22 ) 
    note = berechneFhrDurchschnitt(12, 1, 12, 2, note);
  IF ( (jahrgangsstufe * 10 + halbjahr) >= 31 )
    note = berechneFhrDurchschnitt(12, 2, 13, 1, note);
  IF ( (jahrgangsstufe * 10 + halbjahr) >= 32 )
    note = berechneFhrDurchschnitt(13, 1, 13, 2, note);
}

fachbedingungen{
   //Bereich, Fach, Fachgruppe, anz, anzG5 //anzG5 = benötigte Kurse mit mind. 5 Pkt.
   { FACH, 'Deutsch', 'Deutsch', 2, 0 },
   { FACH, 'Mathematik', 'Mathematik', 2, 0 },
   { FACHGRUPPE, '*', 'Fremdsprache', 2, 0 },
   { FACHGRUPPE, '*', 'Gesellschaft', 2, 0 },
   { FACHGRUPPE, '*', 'Naturwissenschaft', 2, 0 },
   { LK, '*', 'Leistungskurs', 4, 2 },
   { GK, '*', 'Grundkurs', 11, 7 }
}

double berechneFhrDurchschnitt( jahrgang1, abschnitt1, jahrgang2, abschnitt2, note){
   int deutsch=0, mathematik=0, fremdsprache=0, gesellschaft=0, nw=0;
   int lk = 0; int gk = 0;
   int lk5 = 0; int gk5 = 0;
   int punkte;
   bool fhrBestanden = true;
   kurse = holekurseOhneDiff( jahrgang1, abschnitt1, jahrgang2, abschnitt2 );
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



