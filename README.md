# CC2 Dryer-to-Chamber Heat Mod (Budget Tier)

**Goal**: Active drying of Canvas lanes 3 & 4 via Creality Space Pi Plus (lid off) + controlled warm dry air feed into the Centauri Carbon 2 chamber using a damper, while isolating CF wear.

This is the minimal-cost, fully reversible solution. No extra chamber heater required.

## Architecture Summary

- Space Pi Plus sits external, next to the printer.
- Modular printed enclosure surrounds dryer + Canvas posts 3 & 4 so those spools stay in the warm/dry air stream.
- Short 50 mm (2") high-temp flex duct from dryer outlet/port → new printed inlet flange + baffle in a replacement Canvas top "hump".
- Manual damper in the duct controls airflow into the chamber (target 45–55 °C, peak ≤60 °C).
- Capricorn XS PTFE from dryer to Canvas channels 3/4.
- Dedicated CF path (post 4) uses hardened gears + spare 4-in-1 hub + spare tubes.

## Printed Parts Needed

1. **Modular dryer + reel enclosure** (side of CC2 for posts 3/4 + Space Pi Plus)
2. **Canvas top hump / inlet flange + internal baffle** (replaces or sits over factory cover)
3. Optional short duct adapters / flanges

Print in **ASA** (preferred) or high-temp PETG for prototypes.

### Existing Models to Source & Modify

**Canvas / Top Cover related**
- Centauri Carbon 2 Top Cover w/Canvas Relocation (Printed Raw Designs) – good base for shorter cover + inlet addition  
  https://www.printables.com/model/1741573-centauri-carbon-2-cc2-top-cover-172mm-tall-v1  
  https://makerworld.com/en/models/2873763-centauri-carbon-2-top-cover-w-canvas-relocation
- Other CC2 top risers / covers (search Printables / MakerWorld for "Centauri Carbon 2 top cover" or "Canvas riser")

**Side / Dry-box enclosures for CC2**
- Centauri Carbon 1 and 2 MFS Dry Box (Lee Christopher / OneBruceleroy) – excellent side-mount starting point  
  https://makerworld.com/en/models/2950346-centauri-carbon-1-and-2-mfs-dry-box  
  https://www.printables.com/model/1759212-centauri-carbon-1-and-2-dry-box-for-mfs
- Modular Spool Drybox for Centauri Carbon 2 (theStonefox)  
  https://www.printables.com/model/1621621-modular-spool-drybox-for-centauri-carbon-2
- Drybox Holder for Elegoo Centauri Carbon 2 (Georg Pichler)  
  https://www.printables.com/model/1648046-drybox-holder-for-elegoo-centauri-carbon-2
- Other cereal-box / parametric vault style mounts on Printables / Cults

**Space Pi Plus accessories** (desiccant, lid mods, PTFE adapters)
- Multiple desiccant boxes on Printables & MakerWorld (search "Space Pi Plus desiccant")
- PTFE connector adapters for Space Pi lid (Printables)

**Action**: Download the closest models, then modify in CAD for:
- Exact Space Pi Plus clearance (measure your unit – packing size ~343×226×300 mm)
- 50 mm duct inlet flange + baffle on the Canvas top piece
- Magnet mounts, filament exit paths aimed at posts 3/4, and dryer heat capture

## Bought Parts List (Amazon priority, budget tier)

### Heat & Air Path
| Item | Notes / Search Terms | Approx. Price |
|------|----------------------|---------------|
| 50 mm (2") high-temp flexible duct (silicone-coated fiberglass or equivalent, ≥150–300 °C) | "2 inch high temp flexible duct silicone" or "50mm high temperature air duct" | $15–30 for 1–3 m |
| 2" manual volume / butterfly damper with handle | "2 inch HVAC duct damper" or "50mm manual volume damper" | $10–25 |
| Hose clamps (stainless preferred) | 2" or 50–60 mm range | $5–10 |
| High-temp foil / silicone tape | for sealing joints | $5–10 |

### Chamber Insulation & Sealing
| Item | Notes | Approx. Price |
|------|-------|---------------|
| Closed-cell silicone or high-temp foam sheets (thin) | | $10–20 |
| Gold-colored high-temp reflective foil / fiberglass-backed tape | "gold reflective heat tape" or "fiberglass reflective insulation" | $10–20 |
| Rare-earth magnets (neodymium, various sizes) | for removable foam panels | $8–15 |
| High-temp foam weatherstrip / gasket tape | door gap, lid seams, Canvas joints | $8–15 |

### CF Isolation & Feed Path
| Item | Notes | Approx. Price |
|------|-------|---------------|
| Capricorn XS or equivalent low-friction PTFE (extra length + spares) | 4 mm OD | $15–25 |
| Hardened steel drive gears (Canvas feed modules + toolhead) | search CC2 / Canvas compatible hardened gears | $15–40 |
| Spare 4-in-1 filament hub / inlet for toolhead | | $10–25 |
| Spare PTFE segments for CF path | | included above |

### Filament Starter (Earth-tone focus)
- 1–2 kg black ASA-CF or PA-CF (core)
- 1–2 kg plain nylon (PA6 / PA6.6 / PA12 compatible with CC2)
- Earth-tone ASA multipack or individual (ranger green / olive / coyote / black)

### Misc
- High-temp adhesive / silicone for magnets & seals
- Simple digital thermometer (or rely on printer sensor)

**Total estimated hardware cost (excluding filament & printed parts)**: $80–150 depending on exact choices and existing inventory.

## Operating Notes

1. Load nylon/CF into dryer (lanes 3 & 4).
2. Set dryer 50–70 °C as appropriate for the material.
3. Open damper partially; monitor chamber temp and throttle to 45–55 °C.
4. For pure ASA work, reduce or close damper and rely on enclosure + residual heat.
5. Use dedicated CF channel + swap hub/gears as wear appears.

## Safety

- Keep chamber ≤60 °C peak to protect stock belts/electronics.
- Ensure duct joints are secure and heat-rated.
- Monitor first few runs closely.
- All mods are reversible.

## Repo Structure (planned)

```
/
├── README.md                  (this file)
├── docs/
│   ├── plan.md
│   ├── parts-list.md
│   └── measurements.md        (fill with your actual dryer & lid measurements)
├── models/
│   ├── sources.md             (links + notes on base models)
│   ├── enclosure/             (your modified STLs / STEP)
│   ├── canvas-hump/           (inlet + baffle)
│   └── adapters/
└── shopping/
    └── amazon-links.md
```

## Next Steps

1. Measure your exact Space Pi Plus external dimensions (lid off) and the factory Canvas top cover footprint / clearance.
2. Download the base models listed above.
3. Modify for duct inlet + dryer clearance.
4. Print prototypes in PETG, then final in ASA.
5. Update this repo with your measured dimensions and final STLs.

---

Created for Tyler Zervas (tzervas) – CC2 engineering filament workflow (CF + nylon skinning + earth-tone ASA).
