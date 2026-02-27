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

EMP_IMPORT_DATA_AUTO_FAIL and MANUAL fail ---> jak rozlisovat?

PERSON_PROPERTIES_UPDATED a CONTRACT_PROPERTIES_UPDATED ---> proc jsem pochopil, ze to ma jit na uroven endpointu ---> Controller? -- porad je to business logika



Zakladni pravidlo
	Jde o logovani pripadu, kde se neco uklada do databaze. Vetsinou.






