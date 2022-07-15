# Inhalt
1.Edgeslist.csv

2.Nodelist.csv

3.Codebuch.md (Codierung der Datensätze)

# Ursprung und Datenerhebung
Wir wollen uns mit den 20 erfolgreichsten Filmen im Zeitraum von 2000 bis 2020 beschäftigen. Dabei sollen die Filme aus zwei Blickwinkel untersucht werden: Was sind die 20 Filme mit den meisten Einnahmen in diesem Zeitraum? Was sind die 20 besten Filme aus der Sicht der Filmkritiker? Gibt es Filme, Regisseur:innen, Produzent:innen, Schauspieler:innen, Drehbuchautor:innen, Filmstudios, die in beiden Netzwerken zu finden sind? Gibt es mehrfache Nennungen innerhalb des Netzwerks? Gibt es “allround” Talente? 
Die Daten zu den Einnahmen entnehmen wir aus der folgenden Seite: https://www.boxofficemojo.com/chart/top_lifetime_gross/?area=XWW.
Die Daten zu den von der internationalen Presse als am besten bewertete Filme entnehmen wir von der folgenden Seite: https://www.filmstarts.de/kritiken/besten/filme/pressewertung/ und https://www.rottentomatoes.com/.
Zusätzlche Informationen über beteiligte Akteure lassen sich einfach im Internet recherchieren und auch gegenprüfen.

## 1) Edge-Attribute
id: numerische Codierung für jeden Knoten des Netzwerks 
from: initiierender Knoten, in diesem Fall: Film mit Verbindung zu allen Mitwirkenden.

to: erhaltender Knoten, in diesem Fall: mitwirkende Personen, wie beispielsweise die Schauspieler:innen, Produzent:innen etc. 

weight: Rankingplazierung aufgrund des Kritiker-Rankings bzw. der Box Office Einnahmen
20 = beste Platzierung (erste Nennung in den Rankings),
1 = schlechteste Plazierung (letzte Nennung in den Rankings)

relation: Auskunft über den genauen Bezug der Personen zum Film geben. 
1 = acting: Schauspieler:innen aller Filme 
2 = production: Produzent:in, Regisseur:in, Produktionsfirma, Komponist:in; Screenplay der Filme 
3 = award: Auszeichnungen der Filme codiert nach den Attributen oscar und golden_globe


Gewichtung der Filme nach Kritiker Ranking, von 1  bis 20
ranking_box_office
Gewichtung der Filme nach Box Office Ranking, von 1 bis 20 

## Node-Attribute

### id:	
Eindeutige numerische Kennzeichnung des Knotens. Identisch zur Edge-List. 
### name:	
Name Film/Name Person/Firma
### type:	
1 = Film
2 = Schauspielerin
3 = Komponist:in 
4 = Regisseur:in 
5 = Produzent:in 
7 = Produktionsfirma
### ranking_money:	
Rankingplatz bei den weltweiten Einnahmen 
### ranking_critics:	
Rankingplatz in den Filmkritiken
### year:	
Erscheinungsjahr Film
### sex:
1 = female
2 = male
3 = divers
### production:	
Produzent:innen. Codiert in numerischer ID
### director: 
Regisseur:in. Codiert in numerischer ID
### screenplay:	
Drehbuchautor:innen. Codiert in numerischer ID
### cast1 - cast3:	
Hauptdarsteller:innen. Codiert in numerischer ID
### composer:	
Komponist:innen. Codiert in numerischer ID.
### production_company1 bis production_company4: 
Produktionsfirmen. Codiert in numerischer ID
### box_office:	
Box office Einnahmen in Milliarden gerundet
### oscar:	
Anzahl gewonnener Oscars in Zahlen
### golden_globe:	
Anzahl gewonnener Golden Globes in Zahlen
