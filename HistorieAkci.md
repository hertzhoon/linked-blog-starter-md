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
	Dulezite jsou na zacatek hodnoty, ktere 

vytvorim enum a nacpu ho do databaze misto setEvent()


substring akce - filtrovat jinak kvuli ceske lokaizaci na FE
	
kdyz nastane vchyba, UC failne na necem konkretnim ---> errorove kody  do db (nejsou nutne resit teraz)


ENUM misto eventu na hi_event

Porovnat ACCEPTANCE CRITERIA s tim co ted je. NA FE to jeste neni

FE ked neco prijde UC fail -> na pozdeji pridavat error code do db a FE bude vedet vse.

projit vsechny UC a doplnit tu historii kde se nezapisuje

CODEBASE JE COOKED - PTAT SE

