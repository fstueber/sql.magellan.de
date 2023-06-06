# Tabelle **tblCourses**



## Spalten

Diese Tabelle hat 14 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Term`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Subject`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`SubjectStatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`SubjectType`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`SubjectTeacher`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Focus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Level`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`CourseNo`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Attribute`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_COURSES`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 6 Fremdschlüssel.

**`FK_COURSE_FOCUS`**

:   `Focus` » [`Fachschwerpunkte (Kuerzel)`](../../tables/fachschwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_COURSE_LEVEL`**

:   `Level` » [`FachNiveaus (Kuerzel)`](../../tables/fachniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_COURSE_SUBJECT`**

:   `Mandant, Subject` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

    

**`FK_COURSE_SUBJECTSTATUS`**

:   `SubjectStatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_COURSE_SUBJECTTYPE`**

:   `SubjectType` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_COURSE_TERM`**

:   `Term` » [`Zeitraeume (ID)`](../../tables/zeitraeume) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

    

## Indizes

Diese Ansicht hat 8 Indizes.

**`FK_COURSE_BILINGUAL`**

:   `Bilingual`

    

**`FK_COURSE_FOCUS`**

:   `Focus`

    

**`FK_COURSE_LEVEL`**

:   `Level`

    

**`FK_COURSE_SUBJECT`**

:   `Mandant, Subject`

    

**`FK_COURSE_SUBJECTSTATUS`**

:   `SubjectStatus`

    

**`FK_COURSE_SUBJECTTYPE`**

:   `SubjectType`

    

**`FK_COURSE_TERM`**

:   `Term`

    

**`PK_COURSES`**

:   `Mandant, ID`

    
