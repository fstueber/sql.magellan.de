# Tabelle **Abteilungen**



## Spalten

Diese Tabelle hat 5 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Leiter`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_ABTEILUNGEN`**

:   `Mandant, Kuerzel`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_ABTEILUNGEN_MANDANT`**

:   `Mandant`

    

**`IDX_Abteilungen_Leiter`**

:   `Leiter`

    

**`PK_ABTEILUNGEN`**

:   `Mandant, Kuerzel`

    
