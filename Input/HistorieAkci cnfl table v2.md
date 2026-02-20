| Enum                                    | Popis pro FE                                                        |
| --------------------------------------- | ------------------------------------------------------------------- |
| EMP_DATA_IMPORT_MANUAL_UPLOADED         | Manuální import souboru zaměstnanců proběhl úspěšně.                |
| EMP_DATA_IMPORT_AUTO_UPLOADED           | Automatický denní import zaměstnanců proběhl úspěšně.               |
| EMP_DATA_IMPORT_FAIL_INVALID_FILE       | Manuální import selhal – neplatný formát nebo velikost souboru.     |
| EMP_DATA_IMPORT_FAIL_DATA_INCONSISTENCY | Manuální import selhal – chybná nebo nekonzistentní data v souboru. |
| EMP_DATA_IMPORT_AUTO_FAIL               | Automatický import selhal – systémová nebo datová chyba.            |

| Enum             | Popis pro FE                                                                                      |
|------------------|--------------------------------------------------------------------------------------------------|
| PASSWORD_CHANGE  | Uživatel úspěšně změnil své heslo nebo PIN pro autorizaci/podpis.                                |
| PASSWORD_FORGOTTEN | Uživatel spustil proces „Zapomenuté heslo“ – účet a zařízení byla deaktivována, QC pro manuál revokován. |
| BIO_SETTING_ENABLED  | Uživatel v autorizační aplikaci povolil použití biometriky pro manuální podpis.            |
| BIO_SETTING_DISABLED | Uživatel v autorizační aplikaci zakázal použití biometriky pro manuální podpis.            |

| Enum                               | Popis pro FE                                                                                           |
|------------------------------------|---------------------------------------------------------------------------------------------------------|
| PUBLISH_DOCUMENT_SIGNEE_RESULT_SIGNED   | Do UPK byl odeslán výsledek, že objednávka byla úspěšně podepsána (včetně odkazů na podepsané dokumenty). |
| PUBLISH_DOCUMENT_SIGNEE_RESULT_REJECTED | Do UPK byl odeslán výsledek, že uživatel objednávku odmítl podepsat (bez odkazů na dokumenty).         |
| PUBLISH_DOCUMENT_SIGNEE_RESULT_FAIL     | Do UPK byl odeslán výsledek, že došlo k chybě (expirace, chyba podpisu, chyba uložení) bez odkazů na dokumenty. |

| Enum                      | Popis pro FE                                                                                             |
|---------------------------|-----------------------------------------------------------------------------------------------------------|
| MANUAL_AUTH_ORDER_CREATED | Byla vytvořena objednávka k manuální autorizaci (UPK nebo servisní, např. pro QC nebo aktivaci zařízení). |
| MANUAL_AUTH_ORDER_CONFIRMED | Uživatel nebo ověřovatel objednávku v autorizační aplikaci potvrdil.                                 |
| MANUAL_AUTH_ORDER_REJECTED | Uživatel nebo ověřovatel objednávku v autorizační aplikaci odmítl.                                    |
| MANUAL_AUTH_ORDER_EXPIRED | Objednávka k manuální autorizaci expirovala (uživatel potvrdil po povoleném čase).                      |
| MANUAL_AUTH_ORDER_FAIL    | Zpracování manuální objednávky selhalo (technická chyba nebo chyba při podpisu/autorizaci).            |

| Enum                    | Popis pro FE                                                                 |
|-------------------------|-------------------------------------------------------------------------------|
| AUTO_SIGN_ORDER_SIGNED  | Objednávka k automatickému podpisu byla úspěšně zpracována a dokumenty jsou podepsané. |
| AUTO_SIGN_ORDER_FAIL    | Automatický podpis objednávky selhal (např. chybějící QC nebo chyba při podpisu).     |

| Enum                    | Popis pro FE                                                                 |
|-------------------------|-------------------------------------------------------------------------------|
| APP_DEACTIVATION_REVOKED| Zařízení bylo deaktivováno a nelze ho dále používat pro autorizaci/podpis.  |

| Enum                               | Popis pro FE                                                                                  |
|------------------------------------|------------------------------------------------------------------------------------------------|
| APP_ACTIVATION_REGISTRATION_REQUESTED | Uživatel požádal o aktivaci nového zařízení (mobilní nebo desktop aplikace).               |
| APP_ACTIVATION_CODE_GENERATED     | Pro aktivaci zařízení byl vygenerován QR / aktivační kód.                                     |
| APP_ACTIVATION_CODE_INSERTED      | Uživatel zadal nebo naskenoval aktivační kód v autorizační aplikaci.                          |
| APP_ACTIVATION_COMPLETED          | Zařízení bylo úspěšně aktivováno a je připravené k používání pro autorizaci/podpis.           |
| APP_ACTIVATION_FAIL               | Aktivace zařízení selhala (např. chybný nebo expirovaný kód, technická chyba).                |

| Enum                           | Popis pro FE                                                                                 |
|--------------------------------|-----------------------------------------------------------------------------------------------|
| PERSON_PROPERTIES_UPDATED      | Byly aktualizovány identifikační údaje osoby (např. jméno, příjmení, organizace, IČO…).     |
| PERSON_LONGFIDU_REGISTRATION_FINISHED | Registrace osoby v systému ZameKEP byla dokončena (uživatel je technicky „zaveden“). |
| PERSON_ONBOARDING_COMPLETED    | Uživatel má dokončený onboarding – má potřebné certifikáty a aktivní zařízení pro podpis.  |

| Enum                              | Popis pro FE                                                                                 |
|-----------------------------------|-----------------------------------------------------------------------------------------------|
| AUT_QC_CREATE_REQUEST_CREATED     | Uživatel v portálu požádal o vydání QC pro automatický podpis.                               |
| CERT_RENEWAL_FORCED              | Byla spuštěna vynucená obnova kvalifikovaného certifikátu (mimo běžný plán obnov).          |
| QC_REVOKE_CERT_REVOKED           | Certifikát byl revokován (varianta eventu specifická k revokaci daného certifikátu).         |
| QC_REVOKE_CERT_ALREADY_REVOKED   | Pokus o revokaci konkrétního certifikátu, který už byl dříve zneplatněn.                     |
| MAN_QC_CREATE_REPEAT_REQUEST_CREATED | Oprávněný pracovník nebo systém vytvořil žádost o znovuvydání QC pro manuální podpis.    |
| QC_DATA_CHANGE_CONTRACT_UPDATED  | Identifikační údaje kontraktu/žadatele byly změněny a byly vyhodnoceny pro další kroky (revokace / znovuvydání QC). |

| Enum                      | Popis pro FE                                                                 |
|---------------------------|-------------------------------------------------------------------------------|
| QC_REVOKE_REQUESTED       | Byl podán požadavek na revokaci (zneplatnění) kvalifikovaného certifikátu.  |
| QC_REVOKE_ALREADY_REVOKED | Revokace se nepodařila – certifikát je už zneplatněný.                      |
| QC_REVOKE_SUCCESS         | Kvalifikovaný certifikát byl úspěšně revokován (zneplatněn).                |
| QC_REVOKE_FAIL            | Revokace kvalifikovaného certifikátu selhala.                               |

| Enum                              | Popis pro FE                                                                 |
|-----------------------------------|-------------------------------------------------------------------------------|
| EMP_DATA_IMPORT_MANUAL_UPLOADED  | Manuální import souboru zaměstnanců proběhl úspěšně.                         |
| EMP_DATA_IMPORT_AUTO_UPLOADED    | Automatický denní import zaměstnanců proběhl úspěšně.                        |
| EMP_DATA_IMPORT_FAIL_INVALID_FILE| Manuální import selhal – neplatný formát nebo velikost souboru.              |
| EMP_DATA_IMPORT_FAIL_DATA_INCONSISTENCY | Manuální import selhal – chybná nebo nekonzistentní data v souboru. |
| EMP_DATA_IMPORT_AUTO_FAIL        | Automatický import selhal – systémová nebo datová chyba.                     |

| Enum                         | Popis pro FE                                                                 |
|------------------------------|-------------------------------------------------------------------------------|
| AUTH_CODE_GENERATED          | Ověřovací SMS kód pro telefonní číslo byl vygenerován a odeslán uživateli.  |
| AUTH_CODE_VERIFICATION_SUCCESS| Telefonní číslo bylo úspěšně ověřeno zadaným SMS kódem.                    |
| AUTH_CODE_VERIFICATION_FAIL  | Ověření telefonního čísla selhalo – chybný nebo expirovaný SMS kód.        |
| AUTH_CODE_MAX_ATTEMPTS_REACHED | Ověření telefonního čísla selhalo – dosažen maximální počet pokusů.      |

| Enum                                   | Popis pro FE                                                                                         |
|----------------------------------------|-------------------------------------------------------------------------------------------------------|
| QC_ISSUANCE_REQUEST_CREATED_MANUAL     | Zahájena žádost o vydání kvalifikovaného certifikátu (QC) pro manuální podpis.                       |
| QC_ISSUANCE_REQUEST_CREATED_AUTO       | Zahájena žádost o vydání kvalifikovaného certifikátu (QC) pro automatický podpis.                    |
| QC_ISSUANCE_REQUEST_CREATED_MANUAL_REPEAT | Zahájena žádost o znovuvydání QC pro manuální podpis (další kontrakt).                          |
| QC_ISSUANCE_REQUEST_CREATED_RENEWAL    | Zahájen proces obnovy stávajícího kvalifikovaného certifikátu (QC).                                  |
| QC_ISSUANCE_SUCCESS                    | Vydání / znovuvydání / obnova kvalifikovaného certifikátu (QC) proběhla úspěšně.                     |
| QC_ISSUANCE_FAIL                       | Vydání / znovuvydání / obnova kvalifikovaného certifikátu (QC) selhala.                              |