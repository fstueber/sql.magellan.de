# Tabelle **KlassenbuchVermerke**



## Spalten

Diese Tabelle hat 16 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Klassenbucheintrag`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Eintragungsdatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`EintragNr`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`EintragNrSchueler`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Eintragungskategorie`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Eintragungstext`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Bemerkung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Massnahmenkategorie`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`LogErsteintrag`**

:   [`TIMESTAMP`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`LogErsteintrag_Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`LogLetzteAenderung`**

:   [`TIMESTAMP`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`LogLetzteAenderung_Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_KBVERMERKE`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 4 Fremdschlüssel.

**`FK_KBV_EINTRAGUNGSKATEGORIE`**

:   `Eintragungskategorie` » [`Eintragungskategorien (Kuerzel)`](../../tables/eintragungskategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_KBV_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KBV_MASSNAHMENKATEGORIE`**

:   `Massnahmenkategorie` » [`Massnahmenkategorien (Kuerzel)`](../../tables/massnahmenkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_KBV_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

## Indizes

Diese Ansicht hat 6 Indizes.

**`FK_KBV_EINTRAG`**

:   `Mandant, Klassenbucheintrag`

    

**`FK_KBV_EINTRAGUNGSKATEGORIE`**

:   `Eintragungskategorie`

    

**`FK_KBV_KLASSE`**

:   `Mandant, Klasse`

    

**`FK_KBV_MASSNAHMENKATEGORIE`**

:   `Massnahmenkategorie`

    

**`FK_KBV_SCHUELER`**

:   `Mandant, Schueler`

    

**`PK_KBVERMERKE`**

:   `Mandant, ID`

    
