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

**relation**  
Definiert die Art der Geschäftsbeziehung: 1 = Spieler zu Beratungsfirma, 2 = Spieler zu Verein

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
