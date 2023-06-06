# Tabelle **Bildungsgaenge**



## Spalten

Diese Tabelle hat 18 Spalten.

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Bezeichnung2`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Berufsfeld`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Organisation`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Unterrichtsform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Fachrichtung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schwerpunkt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schwerpunkt2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Klassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Dauer`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Qualifikationsniveau`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`StatistikID`**

:   [`VARCHAR(16)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Kategorie`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`GueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`GueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_BILDUNGSGAENGE`**

:   `Kuerzel`

    

## Fremdschlüssel

Diese Tabelle hat 8 Fremdschlüssel.

**`FK_BILDUNGSGAENGE_FACHRICHTUNG`**

:   `Fachrichtung` » [`Fachrichtungen (Kuerzel)`](../../tables/fachrichtungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_BILDUNGSGAENGE_KLASSENSTUFE`**

:   `Klassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_BILDUNGSGAENGE_ORGANISATION`**

:   `Organisation` » [`Organisationen (Kuerzel)`](../../tables/organisationen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_BILDUNGSGAENGE_QUALI`**

:   `Qualifikationsniveau` » [`Qualifikationsniveaus (Kuerzel)`](../../tables/qualifikationsniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_BILDUNGSGAENGE_SCHULFORM`**

:   `Schulform` » [`Schulformen (Kuerzel)`](../../tables/schulformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_BILDUNGSGAENGE_SCHWERPUNKT`**

:   `Schwerpunkt` » [`Schwerpunkte (Kuerzel)`](../../tables/schwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_BILDUNGSGAENGE_SCHWERPUNKT2`**

:   `Schwerpunkt2` » [`Schwerpunkte (Kuerzel)`](../../tables/schwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_BILDUNGSGAENGE_UNTERRICHT`**

:   `Unterrichtsform` » [`Unterrichtsformen (Kuerzel)`](../../tables/unterrichtsformen) · `ON UPDATE SET NULL` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 11 Indizes.

**`FK_BILDUNGSGAENGE_BERUFSFELD`**

:   `Berufsfeld`

    

**`FK_BILDUNGSGAENGE_FACHRICHTUNG`**

:   `Fachrichtung`

    

**`FK_BILDUNGSGAENGE_KLASSENSTUFE`**

:   `Klassenstufe`

    

**`FK_BILDUNGSGAENGE_ORGANISATION`**

:   `Organisation`

    

**`FK_BILDUNGSGAENGE_QUALI`**

:   `Qualifikationsniveau`

    

**`FK_BILDUNGSGAENGE_SCHULFORM`**

:   `Schulform`

    

**`FK_BILDUNGSGAENGE_SCHWERPUNKT`**

:   `Schwerpunkt`

    

**`FK_BILDUNGSGAENGE_SCHWERPUNKT2`**

:   `Schwerpunkt2`

    

**`FK_BILDUNGSGAENGE_UNTERRICHT`**

:   `Unterrichtsform`

    

**`IDX_Bildungsgaenge_Kategorie`**

:   `Kategorie`

    

**`PK_BILDUNGSGAENGE`**

:   `Kuerzel`

    
