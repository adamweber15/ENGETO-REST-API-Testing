# REST API Testing – ENGETO

**Language:** [Čeština](#CZ) | [English](#EN)

---

# CZ

## O projektu

Závěrečný projekt vzdělávací akademie ENGETO zaměřený na funkční testování REST API pro správu studentů, validaci HTTP odpovědí a ověřování integrity dat v databázi PostgreSQL.

## Cíle projektu

- Funkční testování metod GET, POST, PUT a DELETE.
- Ověření pozitivních, negativních a hraničních scénářů.
- Validace HTTP stavových kódů a JSON odpovědí.
- Ověření autentizace a práce s Bearer tokenem.
- Kontrola konzistence dat prostřednictvím SQL dotazů.
- Identifikace, reprodukce a dokumentace softwarových defektů.

## Použité technologie a nástroje

| Nástroj / technologie | Využití |
|---|---|
| Postman | Manuální testování REST API |
| Swagger / OpenAPI | Dokumentace a specifikace API |
| PostgreSQL | Databázové prostředí |
| DBeaver | Databázová validace |
| SQL | Kontrola integrity a konzistence dat |
| JSON | Struktura požadavků a odpovědí |
| GitHub | Dokumentace a verzování projektu |

## Výsledky testování

| HTTP metoda | Počet scénářů |
|---|---:|
| POST | 8 |
| GET | 7 |
| PUT | 11 |
| DELETE | 5 |
| **Celkem** | **31** |

| Výsledek | Počet |
|---|---:|
| PASS | 14 |
| FAIL | 16 |
| K posouzení | 1 |
| **Celkem** | **31** |

**Počet identifikovaných defektů: 10**

## Klíčová zjištění

- Nesprávné ukládání PSČ do databáze.
- Nežádoucí změny hodnot při částečné aktualizaci studenta.
- Nedostatečná kontrola duplicity e-mailových adres.
- Nesprávné HTTP stavové kódy.
- Nesoulad validačních odpovědí s dokumentací API.
- Potvrzení odstranění studenta bez skutečného odstranění z databáze.
- Nedostatečné ošetření hraničních číselných hodnot.

## Dokumentace projektu

Kompletní dokumentace je dostupná ve formátu PDF v tomto repozitáři a obsahuje:

- Zadání a metodiku testování.
- Testovací scénáře.
- Exekuci jednotlivých testů.
- HTTP požadavky a JSON odpovědi.
- SQL dotazy a výsledky databázové validace.
- Detailní bug reporty včetně kroků k reprodukci, testovacích dat a porovnání očekávaných a skutečných výsledků.
- Závěrečné vyhodnocení.

## Testované prostředí

- REST API: https://test-app.engeto.cz/students
- API dokumentace: https://test-app.engeto.cz/docs

Testování bylo provedeno s databázovým přístupem pouze pro čtení. Přihlašovací údaje ani platné autentizační tokeny nejsou součástí veřejné dokumentace.

## Autor

**Ing. Adam Weber**

ENGETO – Závěrečný projekt č. 2

Listopad 2026

---

# EN

## Project Overview

Final project completed as part of the ENGETO educational academy, focused on functional testing of a REST API for student management, HTTP response validation, and data integrity verification in a PostgreSQL database.

## Project Objectives

- Functional testing of GET, POST, PUT, and DELETE methods.
- Verification of positive, negative, and boundary test scenarios.
- Validation of HTTP status codes and JSON responses.
- Verification of authentication and Bearer token handling.
- Data consistency verification using SQL queries.
- Identification, reproduction, and documentation of software defects.

## Technologies and Tools

| Tool / Technology | Purpose |
|---|---|
| Postman | Manual REST API testing |
| Swagger / OpenAPI | API documentation and specification |
| PostgreSQL | Database environment |
| DBeaver | Database validation |
| SQL | Data integrity and consistency verification |
| JSON | Request and response structure |
| GitHub | Project documentation and version control |

## Test Results

| HTTP Method | Test Scenarios |
|---|---:|
| POST | 8 |
| GET | 7 |
| PUT | 11 |
| DELETE | 5 |
| **Total** | **31** |

| Test Result | Count |
|---|---:|
| PASS | 14 |
| FAIL | 16 |
| Requires clarification | 1 |
| **Total** | **31** |

**Total identified defects: 10**

## Key Findings

- Incorrect storage of ZIP codes in the database.
- Unintended changes to field values during partial student updates.
- Insufficient validation of duplicate email addresses.
- Incorrect HTTP status codes.
- Inconsistencies between validation responses and API documentation.
- Successful deletion responses without actual removal of student records from the database.
- Insufficient handling of numeric boundary values.

## Project Documentation

The complete project documentation is available as a PDF file in this repository and includes:

- Project requirements and testing methodology.
- Test scenarios.
- Detailed test execution.
- HTTP requests and JSON responses.
- SQL queries and database validation results.
- Detailed bug reports, including reproduction steps, test data, and comparisons of expected and actual results.
- Final test evaluation.

The PDF documentation is written in Czech.

## Test Environment

- REST API: https://test-app.engeto.cz/students
- API documentation: https://test-app.engeto.cz/docs

Testing was conducted using read-only database access. Login credentials and valid authentication tokens are not included in the public documentation.

## Author

**Ing. Adam Weber**

ENGETO – Final Project No. 2

November 2026
