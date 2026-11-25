# REST API Testing – ENGETO

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

**Adam Weber**

ENGETO – Závěrečný projekt č. 2

Listopad 2026
