# Testresultaten - Decisiontree  

In dit document staan de verschillende resultaten van het testen van het prototype uitgewerkt.

Developer:		Robin

Reviewer 1:		Sander

Reviewer 2:		Eric



## Accuraatheid 

Onder het onderdeel accuraatheid zijn een aantal verschillende zaken van het prototype getest beteft de accuraatheid van de gemaakte voorspelling.

#### Dataset grootte 

Het eerste onderdeel dat getest is, is de toename van de accuraatheid van het algoritme naarmate de hoeveelheid beschikbare trainingsdata groter wordt. Dit is getest door het prototype te trainen kleinere hoeveelheden data van de volledige dataset. 

De onderstaande tabel bevat de waardes van de gemiddelde accuraatheids percentage van de applicatie die zijn gevonden door de applicatie te testen met de testdataset. 

| Percentage data        | Developer | Reviewer 1 | Reviewer 2 |
| ---------------------- | --------- | ---------- | ---------- |
| **25% van de dataset** | 60 %      | 50%        |            |
| **50% van de dataset** | 83,33 %   | 80%        |            |
| **75% van de dataset** | 86,67 %   | 86.67%     |            |
| **100%  van de dataset** | 86,67 % | 86,67%     |            |

#### Aantal ingevoerde symptomen

Naast de afhankelijkheid van de accuraatheid ten opzichte van de grootte van de dataset is ook de accuraatheid van het prototype getest ten opzichte van het aantal ingevoerde symptomen waarmee de voorspelling moet worden gedaan. 

In de onderstaande tabellen staan de resultaten van de tests die zijn uitgevoerd om de accuraatheid te bepalen.

| 1 symptoom ingevoerd | **Gebruikt geslacht** | Gebruikte leeftijd | Gebruikt symptoom | Verwachte voorspelling | **Correcte voorspelling (j/n)** |
| -------------------- | --------------------- | ------------------ | ----------------- | ---------------------- | ------------------------------- |
| developer            | vrouw                 | 32                 | kortademig        | astma                  | j                               |
| developer            | man                   | 20                 | hoesten           | griep                  | n (astma)                       |
| developer            | vrouw                 | 10                 | koorts            | verkoudheid            | n (bronchitis)                  |
| developer            | vrouw                 | 42                 | neusvleugelen     | benauwdheid            | n (astma)                       |
| reviewer 1           | man                   | 16                 | niezen            | verkoudheid            | J                               |
| reviewer 1           | man                   | 63                 | hoesten           | verkoudheid            | N (griep)                       |
| reviewer 1           | vrouw                 | 43                 | hoofdpijn         | griep                  | N (verkoudheid)                 |
| reviewer 1           | man                   | 43                 | kortademig        | astma                  | J                               |
| reviewer 2           |                       |                    |                   |                        |                                 |
| reviewer 2           |                       |                    |                   |                        |                                 |
| reviewer 2           |                       |                    |                   |                        |                                 |
| reviewer 2           |                       |                    |                   |                        |                                 |

| 2 symptomen ingevoerd | **Gebruikt geslacht** | Gebruikte leeftijd | Gebruikte symptomen                 | Verwachte voorspelling | **Correcte voorspelling (j/n)** |
| --------------------- | --------------------- | ------------------ | ----------------------------------- | ---------------------- | ------------------------------- |
| developer             | man                   | 88                 | kortademig, piepende ademhaling     | astma                  | j                               |
| developer             | vrouw                 | 42                 | gebrek aan eetlust, hoesten         | benauwdheid            | n (astma)                       |
| developer             | vrouw                 | 55                 | spierpijn, piepende ademhaling      | bronchitis             | n (astma)                       |
| developer             | man                   | 33                 | verstopte neus, hoesten             | verkoudheid            | n (astma)                       |
| reviewer 1            | vrouw                 | 16                 | kortademig, piepende ademhaling     | astma                  | J                               |
| reviewer 1            | man                   | 25                 | Hoesten,  Hoge slijmproductie       | bronchitis             | J                               |
| reviewer 1            | vrouw                 | 54                 | Verstopte neus,  Gebrek aan eetlust | verkoudheid            | N (Griep)                       |
| reviewer 1            | man                   | 78                 | Keelpijn, hoofdpijn                 | griep                  | J                               |
| reviewer 2            |                       |                    |                                     |                        |                                 |
| reviewer 2            |                       |                    |                                     |                        |                                 |
| reviewer 2            |                       |                    |                                     |                        |                                 |
| reviewer 2            |                       |                    |                                     |                        |                                 |

| 3 symptomen ingevoerd | **Gebruikt geslacht** | Gebruikte leeftijd | Gebruikte symptomen                       | Verwachte voorspelling | **Correcte voorspelling (j/n)** |
| --------------------- | --------------------- | ------------------ | ----------------------------------------- | ---------------------- | ------------------------------- |
| developer             | vrouw                 | 81                 | hoesten, niezen, spierpijn                | verkoudheid            | j                               |
| developer             | man                   | 25                 | vermoeidheid, hoofdpijn, gebrek aan eetlust | verkoudheid          | j                               |
| developer             | man                   | 51                 | kortademig, benauwdheid, hoesten          | astma                  | j                               |
| developer             | man                   | 66                 | koorts, spierpijn, keelpijn               | griep                  | j                               |
| reviewer 1            | vrouw                 | 35                 | Benauwdheid, Hoesten, Koorts              | Astma                  | N (Bronchitis)                  |
| reviewer 1            | vrouw                 | 74                 | Spierpijn, Hoesten, Koorts                | Bronchitis             | J                               |
| reviewer 1            | man                   | 24                 | Gebrek aan eetlust,  Hoofdpijn,  Keelpijn | Verkoudheid            | J                               |
| reviewer 1            | man                   | 45                 | Koorts, Hoofdpijn,  Verstopte Neus        | Griep                  | J                               |
| reviewer 2            |                       |                    |                                           |                        |                                 |
| reviewer 2            |                       |                    |                                           |                        |                                 |
| reviewer 2            |                       |                    |                                           |                        |                                 |
| reviewer 2            |                       |                    |                                           |                        |                                 |

| 4 symptomen ingevoerd | **Gebruikt geslacht** | Gebruikte leeftijd | Gebruikte symptomen                                      | Verwachte voorspelling | **Correcte voorspelling (j/n)** |
| --------------------- | --------------------- | ------------------ | -------------------------------------------------------- | ---------------------- | ------------------------------- |
| developer             | man                   | 24                 | neusvleugelen, pijn bij borst, hoofdpijn, gebrek aan eetlust | longontsteking     | j                               |
| developer             | vrouw                 | 52                 | koorts, keelpijn, verstopte neus, vermoeidheid           | verkoudheid            | n (longontsteking)              |
| developer             | vrouw                 | 75                 | keelpijn, spierpijn, hoofdpijn, niezen                   | griep                  | n (verkoudheid                  |
| developer             | man                   | 11                 | hoesten, spierpijn, verstopte neus, koorts               | benauwdheid            | n (griep)                       |
| reviewer 1            | man                   | 22                 | Benauwdheid,  Kortademig,  Hoesten,  Piepende ademhaling | Astma                  | J                               |
| reviewer 1            | vrouw                 | 35                 | Benauwdheid,  Kortademig,  Hoesten,  Piepende ademhaling | Astma                  | J                               |
| reviewer 1            | man                   | 44                 | Hoesten, Keelpijn,  Hoge slijmproductie,  Pijn bij borst | Longontsteking         | N (Bronchitis)                  |
| reviewer 1            | vrouw                 | 4                  | Gebrek aan eetlust, Hoesten,  Koorts, Niezen             | Verkoudheid            | J                               |
| reviewer 2            |                       |                    |                                                          |                        |                                 |
| reviewer 2            |                       |                    |                                                          |                        |                                 |
| reviewer 2            |                       |                    |                                                          |                        |                                 |
| reviewer 2            |                       |                    |                                                          |                        |                                 |

| 5 symptomen ingevoerd | **Gebruikt geslacht** | Gebruikte leeftijd | Gebruikte symptomen                                          | Verwachte voorspelling | **Correcte voorspelling (j/n)** |
| --------------------- | --------------------- | ------------------ | ------------------------------------------------------------ | ---------------------- | ------------------------------- |
| developer             | man                   | 31                 | hoofdpijn, gebrek aan eetlust, koorts, keelpijn, verstopte neus | vermoeidheid        | n (griep)                       |
| developer             | vrouw                 | 53                 | hoofdpijn, keelpijn, koorts, kortademig, verstopte neus      | benauwdheid            | n (longontsteking)              |
| developer             | man                   | 77                 | hoesten, hoge slijmproductie, piepende ademhaling, koorts, spierpijn | bronchitis     | j                               |
| developer             | vrouw                 | 11                 | kortademig, benauwdheid, hoesten, piepende ademhaling, hoofdpijn | astma              | j                               |
| reviewer 1            | man                   | 1                  | Hoesten,  Benauwdheid,  Gebrek aan eetlust,  Kortademig,  Neusvleugelen | Astma                  | J                               |
| reviewer 1            | man                   | 27                 | Hoesten, Keelpijn,  Hoge slijmproductie,  Pijn bij borst,  Kortademig | Longontsteking         | N (Bronchitis)                  |
| reviewer 1            | man                   | 66                 | Hoge slijmproductie, Keelpijn, Kortademig, Spierpijn, Pijn bij borst | Bronchitis             | J                               |
| reviewer 1            | vrouw                 | 41                 | Keelpijn, Hoofdpijn, Spierpijn,  Vermoeidheid,  Verstopte Neus | Griep                  | N (Verkoudheid)                 |
| reviewer 2            |                       |                    |                                                              |                        |                                 |
| reviewer 2            |                       |                    |                                                              |                        |                                 |
| reviewer 2            |                       |                    |                                                              |                        |                                 |
| reviewer 2            |                       |                    |                                                              |                        |                                 |