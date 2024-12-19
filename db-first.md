## Consegna:

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

| name                | type          | attributes                          | key     | note                                                                  |
| ------------------- | ------------- | ----------------------------------- | ------- | --------------------------------------------------------------------- |
| id                  | BIGINT(20)    | NOT NULL - AUTOINCREMENT - UNSIGNED | primary |
| VIN                 | CHAR(17)      | NOT NULL - UNIQUE                   | ---     |
| make                | VARCHAR(30)   | NOT NULL                            | ---     |
| model               | VARCHAR(30)   | NOT NULL                            | ---     |
| year_of_manufacture | YEAR          | NOT NULL                            | ---     |
| engine_type_ID      | TINYINT       | NOT NULL                            | ---     |
| fuel                | VARCHAR(20)   | NOT NULL                            | ---     |
| color               | VARCHAR(20)   | NOT NULL                            | ---     |
| mileage             | INT           | NOT NULL                            | ---     |
| condition           | CHAR(1)       | DAFAULT 'U' - NULL                  | ---     | 'u' usato, da 'a' a 'e' per indicare le condizioni da ottime a scarse |
| price               | DECIMAL(10,2) | NOT NULL                            | ---     |
| acquired_at         | DATE          | NOT NULL                            | ---     |
| warranty            | TINYINT(1)    | NOT NULL                            | ---     |
