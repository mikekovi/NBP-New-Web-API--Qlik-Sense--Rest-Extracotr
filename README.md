# NBP-New-Web-API--Qlik-Sense--Rest-Extractor

I wanted to share with You an extractor I created for NBP ( National Bank of Poland / Narodowy Bank Polski )

Basically it extracts all tables (A,B,C) of currency exchange rates from 2002-01-01  up to Date ( Today () ).

to sucesfully run this extractor you need to

Create  REST connection  for example (http://api.nbp.pl/api/exchangerates/tables/A/2018-01-01/2018-03-31/) , dates are irrelevant as this URL is  changed every iteration with variable.
NBP connection.png
nbp connection
Create local folder connection 'Extract' - qvd files will be stored there.
Extract connection.png
extract connection
 

Extractor stores :

ratesA.qvd - Middle exchange rates of foreign currencies – table A
ratesB.qvd - Middle exchange rates of foreign currencies – table B
ratesC.qvd - Buy and sell prices of foreign currencies – table C
ratesABC.qvd - concatenated tables A,B,C in one qvd
restA-var.qvd - variables used with each iteration for table A
restB-var .qvd- variables used with each iteration for table B
restB-var.qvd - variables used with each iteration for table C 
