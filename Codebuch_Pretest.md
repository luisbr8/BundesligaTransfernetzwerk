# Datensatz Netzwerkanalyse #
### Christian Mittweg, Eddie Schatz, Luis Bracht, Luisa Käppele, Sina Kuonath  ###

## Inhalt
- Edges.csv (Edgelist)
- Nodes.csv (Nodelist)
- Codebuch_Pretest.md (Codierung der Datensätze)

# EDGE-Attribute

FROM  
Verein/Liga, von dem der Geldfluss ausgeht  

TO  
Verein/Liga, zu dem der Geldfluss geht  

FROM_ALT  
Wenn Liga, dann Vereinsname des geldgebenden Vereins  

TO_ALT  
Wenn Liga, dann Vereinsname des geldnehmenden Vereins 

PLAYERNAME  
Name des transferierten Spielers  

WEIGHT  
Kategorisierung der Transfersummen  

1 = ablösefrei oder unbekannte Transfersumme  
2 = bis 100.000€  
3 = bis 500.000€  
4 = bis 1.000.000€  
5 = bis 5.000.000€  
6 = bis 10.000.000€
7 = über 10.000.000€  

TRANSFERTYPE  
Beschreibt die Art des Transfers  

1 = Transfer  
2 = Leihgeschäft  

YEAR  
Das Jahr, indem das Transfergeschäft vollzogen wurde  

TRANSFERFENSTER   
Das Transferfenster, indem das Transfergeschäft vollzogen wurde 

1 = Sommertransferfenster   
2 = Wintertransferfenster 

TRANSFERID  
Hier steht der einzigartige Link zum Wechsel auf transfermarkt.de (bsp. https://www.transfermarkt.de/jumplist/transfers/spieler/768384/transfer_id/3017239). Dieser Link dient zum einen als Beleg und zum anderen als Überprüfungsmöglichkeit, um mögliche Duplikate schnell ausfindig zu machen.  

# NODE-Attribute  
  
ID   
Einzigartige Abkürzung der Vereine und Ligen.   

NAME
Einzigartige Abkürzung der Vereine und Ligen für Beschriftung im Netwerk.

NAME2
Ausgeschriebener Name des Vereins oder der Liga. 
  
TYPE  
Der Typ des Knotens   

1 = Verein, der zum Zeitpunkt des Transfers in der Bundesliga gespielt hat  
2 = Untere deutsche Ligen sowie ausländische Ligen  

LEVEL   
Das Niveau der Liga. Orientiert sich an der Fünf-Jahres-Wertung der UEFA sowie einer eigenen Einordnung für außereuropäische Ligen  

1 = "Big Five"-Ligen in Europa   
2 = Platz 6 bis 22 der UEFA, dazu Brasilien, USA und China als attraktive außereuropäische Ligen  
3 = Rest  

##
