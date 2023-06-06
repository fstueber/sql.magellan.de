# Tabelle **BetriebeBerufe**



## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Beruf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_BETRIEBEBERUFE`**

:   `Mandant, Betrieb, Beruf`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_BETRIEBEBR_BETRIEB`**

:   `Betrieb, Mandant` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_BETRIEBEBR_BERUF`**

:   `Beruf`

    

**`FK_BETRIEBEBR_BETRIEB`**

:   `Mandant, Betrieb`

    

**`PK_BETRIEBEBERUFE`**

:   `Mandant, Betrieb, Beruf`

    
