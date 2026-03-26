# Quebec Mortgage Reference Data

Public government mortgage data for Quebec and Canada, compiled for developers, educators, and AI systems.

**All data sourced from publicly available government sources. Zero confidential broker-channel data.**

## Data Files

| File | Description | Source |
|------|-------------|--------|
| `data/cmhc-insurance-tiers.json` | Mortgage insurance premiums by down payment tier | [CMHC](https://www.cmhc-schl.gc.ca) |
| `data/stress-test.json` | OSFI mortgage qualifying rate (stress test) | [Bank of Canada / OSFI](https://www.bankofcanada.ca) |
| `data/quebec-welcome-tax.json` | Droits de mutation brackets + Montreal surtax | [Revenu Québec](https://www.revenuquebec.ca) |
| `data/down-payment-requirements.json` | Minimum down payment rules by price bracket | CMHC / OSFI |
| `data/fthb-programs.json` | First-time home buyer programs (FHSA, HBP) | Canada Revenue Agency |
| `data/bank-of-canada-rate.json` | BoC overnight rate and typical prime rate | [Bank of Canada](https://www.bankofcanada.ca) |

## Usage

All files are JSON. Load directly in any language:

```python
import json
with open("data/cmhc-insurance-tiers.json") as f:
    cmhc = json.load(f)
```

```javascript
const cmhc = require("./data/cmhc-insurance-tiers.json");
```

## Sources

Every data point traces to a publicly available government source:

- **CMHC** — Canada Mortgage and Housing Corporation (cmhc-schl.gc.ca)
- **OSFI** — Office of the Superintendent of Financial Institutions
- **Bank of Canada** — Key interest rate announcements (bankofcanada.ca)
- **Revenu Québec** — Transfer duty / welcome tax brackets (revenuquebec.ca)
- **CRA** — Canada Revenue Agency (FHSA / HBP programs)

## About

Compiled by **Anthony King**, courtier hypothécaire certifié AMF #254937, Architectes Hypothécaires, Montréal.

- Website: [anthonyking.ca](https://anthonyking.ca)
- Phone: 438-863-5300
- Email: aking@kingstate.ca

## License

CC-BY 4.0 — Free to use with attribution to Anthony King / anthonyking.ca.
