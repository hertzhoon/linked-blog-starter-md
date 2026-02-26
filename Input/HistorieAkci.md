HistoryController - getHistory()

Entita History

hi_event je text pretvorit na enum
hi_source_type --- 

nemusim resit - kde se zapisuje a nezapisuje

**history.setEvent()**

jednak chci aby jeden zaznam enumu ---
	budeme rozlisovat case (auth code - bude mit atributy succesful nebo failed dle )


Confluence
	kody use casu (KOD UC)
	tam kde se pise do historie database 
		identifikovat use case -> vytvorit enum -> nastavit do eventu spravnou hodnotu enumu ->  CNFL idk nejak se prizpusobim


certSN do eventu nepsat -> zahodit


definovane resp. nedefoinovane
	auth code failed


Priorita 1:
	enum parametry budou ty UC z CNFL
	dve enum hodnoty (succ, fail) pro kazde UC
	kazda hodnota enumu bude mit parametr name, coz bude ten UC
	enum bude mit ten samy UC, jeden bude succ a jeden fail	

vytvorim enum a nacpu ho do databaze misto setEvent()


substring akce - filtrovat jinak kvuli ceske lokaizaci na FE
	
kdyz nastane vchyba, UC failne na necem konkretnim ---> errorove kody  do db (nejsou nutne resit teraz)


ENUM misto eventu na hi_event

Porovnat ACCEPTANCE CRITERIA s tim co ted je. NA FE to jeste neni

FE ked neco prijde UC fail -> na pozdeji pridavat error code do db a FE bude vedet vse.

projit vsechny UC a doplnit tu historii kde se nezapisuje


Structured
	ENUM name -> popisne vuci tomu, co dela UC -> rozdeleno na PASS a FAIL




25-02-2026
	Filtrovani dle substringu akce
	Davat do ENUMu CZ nazvy je blbost
	EVent filtering dle ENUM listu, simple bimple
	Idealne chceme vyhledavat v DB.
	FE dropdown --> FE posila jmena ENUMu zrejme.....


QC_ISSUANCE_SUCC/FAIL

updatePerson a updateContract se vola v jednom z FE

CONTRACT UPDATE 

REVOKACE_QC REQUESTED a SUCCESS

Password stuff logovat na urovni endpointu

vsechno co logujeme, budou triggernute pres REST api, 

kdyz mame priklad: person_properties_updated --- zalogovat vsechno kde se napric celym kodem zmenila nejaka vec v person

import succ/fail --> byla zmena udaju na revokaci? --> budeme logovat ANO, zmenily se udaje
odstranit logovani z nejnizsi urovne, protoze se triggeruje z vice mist