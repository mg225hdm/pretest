
# Inhalt
1.Edgeslist.csv

2.Nodelist.csv

3.Codebuch.md (Codierung der Datensätze)

# Ursprung und Datenerhebung
Die Daten zu den Einnahmen entnehmen wir aus der folgenden Seite: https://www.boxofficemojo.com/chart/top_lifetime_gross/?area=XWW.
Die Daten zu den von der internationalen Presse als am besten bewertete Filme entnehmen wir von der folgenden Seite: https://www.filmstarts.de/kritiken/besten/filme/pressewertung/.
Zusätzlche Informationen über beteiligte Akteure lassen sich einfach im Internet recherchieren und auch gegenprüfen.

# 1) Edge-Attribute
from,to

Es gibt keine Edge-Attribute 
# 2) Node-Attribute
id,name, type, ranking_money,	ranking_critics,	year, production, screenplay,	cast1,	cast2,	cast3,	composer,	production_company1,	production_company2,	production_company3	production_company4,	box_office,	oscar	golden_globe
- id:	Eindeutige Kennzeichnung des Knotens 
- name:	Name Film/Name Person/Firma
- type:	Film/Schauspieler:in, Komponist:in, Regisseur:in, Produzent:in, Produktionsfirma
- ranking_money:	Rankingplatz bei den weltweiten Einnahmen 
- ranking_critics:	Rankingplatz in der internationalen Presse
- year:	Erscheinungsjahr Film/Gründungsjahr Firma/Geburtsjahr Person
- production:	Produzent:innen
- screenplay:	Drehbuchautor:innen
- cast1 - cast3:	Hauptdarsteller:innen
- composer:	Komponist:innen
- production_company1 bis production_company4: Produktionsfirmen
- box_office:	Box office Einnahmen in Milliarden gerundet
- oscar:	Anzahl gewonnener Oscars in Zahlen
- golden_globe:	Anzahl gewonnener Golden Globes in Zahlen
