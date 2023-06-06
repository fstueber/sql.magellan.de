# Tabelle **SchuelerMedizinDaten**



## Spalten

Diese Tabelle hat 11 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Kategorie`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Art`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Medikamente`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Medikationen`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Bemerkung1`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Bemerkung2`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`AblaufAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_SCHUELERMEDIZINDATEN`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_SCHUELERMEDIZINDATEN_ART`**

:   `Art, Mandant` » [`MedizinArten (ID, Mandant)`](../../tables/medizinarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERMEDIZINDATEN_KAT`**

:   `Kategorie, Mandant` » [`MedizinKategorien (ID, Mandant)`](../../tables/medizinkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 4 Indizes.

**`FK_SCHUELERMEDDAT_SCHUELER`**

:   `Mandant, Schueler`

    

**`FK_SCHUELERMEDIZINDATEN_ART`**

:   `Mandant, Art`

    

**`FK_SCHUELERMEDIZINDATEN_KAT`**

:   `Mandant, Kategorie`

    

**`PK_SCHUELERMEDIZINDATEN`**

:   `Mandant, ID`

    
