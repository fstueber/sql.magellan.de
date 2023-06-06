# Tabelle **KlassenbuchKlassenwechsel**



## Spalten

Diese Tabelle hat 8 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Von`**

:   [`TIMESTAMP`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Bis`**

:   [`TIMESTAMP`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`KlasseRegulaer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`KlasseTemporaer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Grund`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_KBKWECHSEL`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_KBKWECHSEL_KLASSETEMP`**

:   `KlasseTemporaer, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

**`FK_KBKWECHSEL_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 4 Indizes.

**`FK_KBKWECHSEL_KLASSEREG`**

:   `Mandant, KlasseRegulaer`

    

**`FK_KBKWECHSEL_KLASSETEMP`**

:   `Mandant, KlasseTemporaer`

    

**`FK_KBKWECHSEL_SCHUELER`**

:   `Mandant, Schueler`

    

**`PK_KBKWECHSEL`**

:   `Mandant, ID`

    
