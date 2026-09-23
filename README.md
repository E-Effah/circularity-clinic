[README.md](https://github.com/user-attachments/files/32558671/README.md)
# Circularity Clinic — Build and Break a Stack

An interactive teaching tool for **H2VE Module 4: Circular Design of Hydrogen Systems**
(German Centre of Vocational Excellence, EQF 6).

**Live page:** https://YOUR-USERNAME.github.io/h2ve-circularity-clinic/

## What it does

Students assemble a single cell of a PEM electrolyser or a PEM fuel cell, decide how each
interface is joined, make four design decisions, and then run an end-of-life test. The test
reports:

- a design-for-disassembly score, and how many joints must be destroyed to open the stack;
- which R-strategies remain available (a single irreversible joint removes everything above recycling);
- the recycling route the design forces, and the material value recovered per MW.

A **facilitator view** turns short result codes into a class scoreboard, so no accounts,
logins or network connection between devices are needed.

## Use

Open the live page in any browser. It also runs offline: download `index.html` and
double-click it. There are no external dependencies, no tracking and no data leaves the device;
the only stored value is the user's own best score, kept in the browser.

## Data and sources

| Quantity | Source |
|---|---|
| Material masses per MW of PEMWE and PEMFC | Uekert, Wikoff & Badgett (2024), *Advanced Sustainable Systems* 8, 2300449, Table 1 (CC BY) |
| Recycling yields (85 % hydrometallurgy, 98 % pyrohydrometallurgy, 81 % PFSA solvent dissolution, 91 % Ti, 92 % stainless steel) | Uekert et al. (2024), Table S1 |
| Climate comparison between routes | Uekert et al. (2024), Figure 2 |
| Platinum price, 58.5 USD/g | Trading Economics, 22 September 2026 |
| Iridium price, 278 USD/g | Johnson Matthey-referenced quotation, 10 September 2026 |

Titanium and stainless steel scrap prices, the design-score weightings and the 15 % price
penalty for unmarked material are **teaching assumptions**, not published values. They are
stated as such inside the page.

## Editing

Everything is in `index.html`: markup, styles and logic. Material masses, prices, joint types
and design options are defined in the `PRICE`, `TECH`, `JOINTS` and `OPTIONS` objects near the
top of the script, so the figures can be updated without touching the rest of the code.

## Licence and attribution

Co-funded by the European Union (Erasmus+, 101194163 — H2VE — ERASMUS-EDU-2024-PEX-COVE).
Views and opinions expressed are those of the author(s) only and do not necessarily reflect
those of the European Union or the European Education and Culture Executive Agency (EACEA).

Developed at the Sustainable Technologies Laboratory (STL), Hochschule Bochum.
