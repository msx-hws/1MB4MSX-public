# Bill of Materials (BOM) - 1MB4MSX

Interactive HTML BOM is available at: [**`bom/ibom.html`**](ibom.html) (open directly in your browser to inspect component placements on the PCB).

---

## Component List

| Reference | Value / Part | Description | Package / Footprint | Qty |
| :--- | :--- | :--- | :--- | :---: |
| **U1, U2** | **74HCT670** | 4x4 Register File (3-state) mapper registers | DIP-16 (300 mil / 7.62mm) | 2 |
| **U3** | **74LS139** (or 74HCT139) | Dual 2-to-4 Line Decoder / Demultiplexer | DIP-16 (300 mil / 7.62mm) | 1 |
| **U4** | **74HCT30** | 8-Input NAND Gate | DIP-14 (300 mil / 7.62mm) | 1 |
| **U5, U6** | **AS6C4008-55PCN** | 512K x 8 Low Power CMOS SRAM (Total 1024 KB) | DIP-32 (600 mil / 15.24mm) | 2 |
| **C1–C6** | **100nF (0.1µF)** | Ceramic decoupling capacitors | THT Disc (Lead Pitch 2.50mm) | 6 |
| **C7** | **22µF** | Electrolytic Filter Capacitor (16V+) | Radial (Lead Pitch 2.50mm, Dia 5.0mm) | 1 |
| **J1** | **MSX Cartridge** | 50-Pin MSX Cartridge Edge Connector | PCB Gold Fingers (Integrated) | 1 |

---

## Recommended Sockets
- **DIP-32 Sockets (600 mil):** 2x for U5, U6 (AS6C4008 SRAMs)
- **DIP-16 Sockets (300 mil):** 3x for U1, U2 (74HCT670), U3 (74LS139)
- **DIP-14 Sockets (300 mil):** 1x for U4 (74HCT30)
