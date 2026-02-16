
---

MISS% + HIT% + CRIT_MISS% + CRIT_HIT% = 1
CRIT_MISS% + CRIT_HIT% = CRIT%

NOTE: |EXPR| means between 0 and 1

HIT% = |((TPC + (21 - CRIT_RNG) - CA) x 1/20)|
CRIT% = (CRIT_RNG x 1/20)
CRIT_CONFIRMATION% = |(TPC + 21 - CA + (HAS_CRIT_FOCUS x 4))|
CRIT_HIT% = CRIT% x CRIT_CONFIRMATION%
CRIT_MISS% = 1-CRIT_HIT%

DMG = (HIT% + CRIT_MISS%) x AD + CRIT_HIT x CRIT_MUL x AD

DMG = 
	(
		|((TPC + (21 - CRIT_RNG) - CA) x 1/20)| + 
		1 - 
		(
			(CRIT_RNG x 1/20) x 
			|(TPC + 21 - CA + (HAS_CRIT_FOCUS x 4))|
		)
	) x AD + 
	(
		(CRIT_RNG x 1/20) x 
		|(TPC + 21 - CA + (HAS_CRIT_FOCUS x 4))|
	) x CRIT_MUL x AD

DMG = (((TPC + (21 - CRIT_RNG) - CA) x 1/20) + 1 - ((CRIT_RNG x 1/20) x (TPC + 21 - CA + (HAS_CRIT_FOCUS x 4)))) x AD + ((CRIT_RNG x 1/20) x (TPC + 21 - CA + (HAS_CRIT_FOCUS x 4))) x CRIT_MUL x AD

---

### Nakoa
TPC: 28/19/14
DPS: ((TPC+21-CA) x AD) + (CRIT%) x (CRIT_MUL-1) x AD

TPC: 28
CA: 35
CRIT_RNG: 6
PF: 201
CA: 28
TS:
- TEM: 16
- RIF: 16
- VOL: 20

### Ael'Sol
TPC: 27/18/13, 33 (Carica)
DPS: 
PF: 
CA:
TS:
- 
- 
- 

### Zemenis
TPC:
DPS:
CA:
TS:
- 
- 
- 

