# Tabelle **SchuelerAusbildung**



## Spalten

Diese Tabelle hat 25 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`GUID`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`AusbilderKontakt`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`PraxisBetrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`PraxisKontakt`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Beruf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Bildungsgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Organisation`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`AusbildungVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`AusbildungBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Ausbildungsdauer`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`PraxisVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`PraxisBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Praxisdauer`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Vertrag`**

:   [`CHAR(1) `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Vertragsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Vertragsnr`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`VertragVorgelegtAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Neuanfaenger`**

:   [`CHAR(1) `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `DEFAULT 'DEFAULT 'J''`

    

**`Bemerkung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_SCHUELERAB`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 9 Fremdschlüssel.

**`FK_SCHUELERAB_BERUF`**

:   `Beruf` » [`Berufe (Kuerzel)`](../../tables/berufe) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERAB_BETRIEB`**

:   `Betrieb, Mandant` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_SCHUELERAB_BILDUNGSGANG`**

:   `Bildungsgang` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERAB_ORGANISATION`**

:   `Organisation` » [`Organisationen (Kuerzel)`](../../tables/organisationen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERAB_PRAXISBETRIEB`**

:   `Mandant, PraxisBetrieb` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

**`FK_SCHUELERAB_PRAXISKONTAKT`**

:   `Mandant, PraxisKontakt` » [`BetriebeKontakte (ID, Mandant)`](../../tables/betriebekontakte) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

**`FK_SCHUELERAB_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

**`FK_SCHUELERAB_SCHULFORM`**

:   `Schulform` » [`Schulformen (Kuerzel)`](../../tables/schulformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERAB_VERTRAGSART`**

:   `Vertragsart` » [`Vertragsarten (Kuerzel)`](../../tables/vertragsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 11 Indizes.

**`FK_SCHUELERAB_AUSBILDERKONTAKT`**

:   `Mandant, AusbilderKontakt`

    

**`FK_SCHUELERAB_BERUF`**

:   `Beruf`

    

**`FK_SCHUELERAB_BETRIEB`**

:   `Mandant, Betrieb`

    

**`FK_SCHUELERAB_BILDUNGSGANG`**

:   `Bildungsgang`

    

**`FK_SCHUELERAB_ORGANISATION`**

:   `Organisation`

    

**`FK_SCHUELERAB_PRAXISBETRIEB`**

:   `Mandant, PraxisBetrieb`

    

**`FK_SCHUELERAB_PRAXISKONTAKT`**

:   `Mandant, PraxisKontakt`

    

**`FK_SCHUELERAB_SCHUELER`**

:   `Mandant, Schueler`

    

**`FK_SCHUELERAB_SCHULFORM`**

:   `Schulform`

    

**`FK_SCHUELERAB_VERTRAGSART`**

:   `Vertragsart`

    

**`PK_SCHUELERAB`**

:   `Mandant, ID`

    
