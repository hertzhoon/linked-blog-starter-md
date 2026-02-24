
The boss just told me that after the external devs are gone, most of this app will fall on my shoulders. Need to really quicken up with the analysis of the app.


24-02-2026 Understanding
```
Copied from CNFL: 

- ČSOB ZameKEP – Portál pro správce (Administration portal): webová aplikace, zabezpečuje auditovatelné nahrávání údajů o zaměstnancích z bankovního systému a fyzické doověření totožnosti zaměstnance, pokud je toto vyžadováno 
    

- ČSOB ZameKEP –  Samoobslužný portál (Selfcare portal): webová aplikace, zajišťuje správu uživatelského účtu, tj. správu hesla/PIN, správu aplikací pro podepisování, správu certifikátů 
    

- Portály BE – zajišťují logiku a přístup k datovému úložišti pro oba portály výše
```
	

TECH DEBT
	Transactions
		They are missing in places.
		No @Transactional in a lot of services
		Custom TransactionManager, probably bs


