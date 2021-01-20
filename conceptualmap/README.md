# Mapping van geo-klassen en -typen

Imvertor werkt met een configuratiebestand `conceptual-schemas.xml` waarin een mapping is opgenomen tussen gestandaardiseerde ISO/OGC/INSPIRE klassen en typen die wij in informatiemodellen gebruiken, naar bijvoorbeeld in GML voorkomende typen. Imvertor gebruikt dit om bijvoorbeeld GML Application schema's te genereren uit een informatiemodel. 

Bij deze klassen en typen is het ook mogelijk om links op te nemen naar een online gepubliceerde definitie en/of uitleg ervan, die Imvertor dan kan gebruiken om links in de documentatie te genereren. 

Een voorbeeldje. In onze UML modellen gebruiken we vaak `GM_Surface`. 

Imvertor “weet” al (omdat dit in een configuratie bestand staat) hoe dit vertaald moet worden naar een GML type zodat er een correct GML application schema uit komt rollen. 

We genereren met Imvertor niet alleen XML/GML schema’s, maar ook data specificaties, bv dit hoofdstuk uit de IMGeluid catalogus is met Imvertor uit UML gegenereerd: https://docs.geostandaarden.nl/cvgg/img/#cat

Je ziet daarin dat het ISO concept “GM_Surface” niet gedocumenteerd is. Een lezer die het niet kent, kan niet direct opzoeken wat het betekent. Zie bv het geometrie attribuut in de klasse VlakbronIndustrie 
https://docs.geostandaarden.nl/cvgg/img/#detail_attribute_IMGeluidAlgemeen_VlakbronIndustrie_geometrie

Terwijl andere typen klikbaar zijn omdat ze elders in de data specificatie worden gedefinieerd. 

Nu willen we Imvertor in gevallen zoals `GM_Surface links` laten genereren naar definities in de ISO Geolexica, het INSPIRE register en ons eigen definities.geostandaarden.nl voor NEN 3610. Daarvoor hebben we een eerste (onvolledige) [mapping](https://github.com/Geonovum/imvertor/blob/main/conceptualmap/mapping-ISOlexicon.xlsx) gemaakt. 

De ambitie is om niet alleen deze mapping te verbeteren, maar om ook de lijst van in informatiemodellen te gebruiken geo-klassen en -typen te standaardiseren. 
