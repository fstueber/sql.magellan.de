# Tabelle **MedienStichworte**



## Spalten

Diese Tabelle hat 4 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Medium`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Stichwort`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_MEDIENSTICHWORTE`**

:   `Mandant, ID`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_MEDIENSTICHWORTE_MEDIUM`**

:   `Mandant, Medium`

    

**`IDX_MSW_MEDIUM`**

:   `Mandant, Medium`

    

**`PK_MEDIENSTICHWORTE`**

:   `Mandant, ID`

    
