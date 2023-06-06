# Tabelle **MedienSchlagworte**



## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Medium`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Schlagwort`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_MEDIENSCHLAGWORTE`**

:   `Mandant, Medium, Schlagwort`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_MEDIENSCHLAGWORTE_SCHLAGWORT`**

:   `Mandant, Schlagwort` » [`Schlagworte (ID, Mandant)`](../../tables/schlagworte) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_MEDIENSCHLAGWORTE_MEDIUM`**

:   `Mandant, Medium`

    

**`FK_MEDIENSCHLAGWORTE_SCHLAGWORT`**

:   `Mandant, Schlagwort`

    

**`PK_MEDIENSCHLAGWORTE`**

:   `Mandant, Medium, Schlagwort`

    
