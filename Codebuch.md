# Beraterfirmen in der Bundesliga
# Datensatz #
Codebuch Beraterfirmen der Bundesligaspieler 
Stand Abgabe (27.09.2022)

Erstellt von Hanna Damaschke (hd029) und Julian Rebmann (jr126)

## Inhalt
- buliedges.csv (Edgelist)
- bulinodes.csv (Nodelist)
- Codebuch.md (Codierung der Datensätze)

## Ursprung und Datenerhebung
Der Ursprung unserer Forschung liegt in der Vorlesung „Soziale Netzwerkanalyse“ im Rahmen des Studiums Crossmedia-Redaktion/Public Relations im dritten Semester an der Hochschule der Medien in Stuttgart. 

Der Datenzugang erfolgt über die Webseite transfermarkt.de und die Webseiten der jeweiligen Beraterfirmen. Die Datenerhebung beschränkt sich auf die Top 7 Vereine und deren Spieler der Bundesliga Saison 2021/2022. 

Das Netzwerk ist ein *ungerichtetes Gesamtnetzwerk*. 

# EDGELIST-Attribute

**from**  
Entspricht den Spieler-IDs in der Nodelist.

**to**  
Entspricht der ID der Beratungsfirma oder des Vereins

**relationship**  
Definiert die Art der Geschäftsbeziehung: 1 = Spieler zu Beratungsfirma, 2 = Spieler zu Verein

**rank**
Entspricht der Platzierung des Vereins in der Saison 2021/22 mit 10 addiert (also von 11-28 durchnummeriert)

**agency**
jeweilige Berateragentur des Spielers

**category**
Alterskategorien der Spieler ("teen"=16-19, "young"=20-23, "mid"=24-27, "old"=28-31, "rusty"=32-38)

**worth**
Marktwertkategorien der Spieler ("nothing"\<1Mio, "low"=1-5Mio, "cheap"=5-20Mio, "average"=20-40Mio, "high"=40-60Mio, "expensive"\>60Mio)

# NODELIST-Attribute  
  
**id**  
Eindeutige Identifikation der einzelnen Knotens (Beraterfirmen, Vereine, Spieler), der erfasst wird.  

**name**  
Name der Beraterfirma, des Vereins oder des Spielers als klar Bezeichnung des Knotens. 

**type**  
Art des Knotens: 1 = Beraterfirma, 2 = Verein, 3 = Spieler.

**country**   
Sitz der Beratungsfirma oder Nationalität des Spielers.

**age**   
Alter des Spielers, bei Beraterfirma und Verein bleibt diese Zeile leer (NA).

**value**             
Marktwert des Spielers, bei Beraterfirma und Verein bleibt diese Zeile leer (NA).

**category**
Alterskategorien der Spieler ("teen"=16-19, "young"=20-23, "mid"=24-27, "old"=28-31, "rusty"=32-38)

**worth**
Marktwertkategorien der Spieler ("nothing"\<1Mio, "low"=1-5Mio, "cheap"=5-20Mio, "average"=20-40Mio, "high"=40-60Mio, "expensive"\>60Mio)
