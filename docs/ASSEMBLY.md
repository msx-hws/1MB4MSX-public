# Assembly & Verification Guide - 1MB4MSX

## Soldering Order

1. **Decoupling Capacitors:**
   - Solder C1–C6 (100nF ceramic decoupling capacitors across each IC power pin).
2. **Sockets:**
   - Solder DIP sockets for U1–U2 (DIP-16), U3 (DIP-16), U4 (DIP-14), and U5–U6 (DIP-32). Sockets prevent thermal stress and simplify testing.
3. **Electrolytic Filter Capacitor:**
   - Solder C7 (22µF radial electrolytic capacitor, observe polarity: negative stripe to ground).
4. **Clean the Board:**
   - Thoroughly clean flux residue using isopropyl alcohol (IPA). Ensure edge connector fingers are clean.

---

## Pre-Power & Bus Checks

1. **Short Circuit Check:**
   - Before inserting any ICs, measure continuity/resistance between +5V (pins 45, 47 on the MSX connector) and GND (pins 41, 43).
   - Ensure there are no short circuits across the power rails.
2. **Dry Fit Test (Unpopulated Board):**
   - Insert the unpopulated cartridge PCB into an MSX cartridge slot.
   - Power on the computer. It should boot normally into BASIC without freeze or interference.

---

## Testing & Memory Detection

1. **Insert Logic and Memory ICs:**
   - Insert U1, U2 (74HCT670 mapper registers).
   - Insert U3 (74LS139 / 74HCT139 decoder).
   - Insert U4 (74HCT30 NAND gate).
   - Insert U5, U6 (AS6C4008 512KB SRAMs, total 1024 KB).
2. **Boot into MSX-DOS2 / Nextor:**
   - Start the MSX with MSX-DOS2 / Nextor.
   - Run memory detection utilities (such as `MEMMAN`, `MAPPER.COM`, or `RAMTEST.COM`).
   - The memory mapper will report a full 1024 KB (1 MB) of primary mapped RAM available across all four standard MSX 16KB pages.
