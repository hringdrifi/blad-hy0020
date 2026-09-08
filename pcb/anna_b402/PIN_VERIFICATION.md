# Pin verification - ANNA-B402-00B

Checked 2026-09-08 against u-blox UBX-20032372 R06, Figure 3 and Table 4 (pp. 18-20).
Source: https://content.u-blox.com/sites/default/files/ANNA-B402_DataSheet_UBX-20032372.pdf

- All 56 symbol pin numbers and names match Table 4.
- Symbol and footprint each contain numbers 1-56 exactly once.
- Pad ordering and orientation visually checked against Figure 3 (top view): no mirrored or swapped numbering found, including center GND pads 53-56.
- Pad widths 0.350 mm (1-52), 0.420 mm (53-56), and outer row separation 5.680 mm agree with package dimensions in Figure 6. Full land-pattern dimensional validation is pending.
- Electrical pin types assigned on 2026-09-08 from Table 4: VCC/VBUS and GND = power_in; RESET_N/SWDCLK = input; GPIO (including multiplexed SWO/XL/NFC), USB data and SWDIO = bidirectional; RF/antenna terminals 1, 2, 3, 5, 6 = passive. Antenna grounding terminals are configuration-dependent and are not ordinary supply-ground pins. RF terminals use passive to avoid applying digital ERC direction rules to the antenna network.
- Module GPIO names differ from Nordic ports; e.g. GPIO_10 = P0.20.
- Antenna keepouts and connection layout were not verified.
- Only symbol electrical pin types were changed; pin numbers, names, geometry, and footprint are unchanged. All 56 pins have assigned types (13 power_in, 2 input, 36 bidirectional, 5 passive).

| Pin | Symbol name | Result |
| --- | --- | --- |
| 1 | ANT_PCB | Match |
| 2 | ANT_GND1 | Match |
| 3 | ANT_GND2 | Match |
| 4 | GND | Match |
| 5 | ANT_INT | Match |
| 6 | ANT | Match |
| 7 | GND | Match |
| 8 | GND | Match |
| 9 | VCC | Match |
| 10 | GPIO_10 | Match |
| 11 | GPIO_11 | Match |
| 12 | RESET_N | Match |
| 13 | GPIO_13 | Match |
| 14 | GPIO_14 | Match |
| 15 | GPIO_15 | Match |
| 16 | SWO/GPIO_16 | Match |
| 17 | XL1/GPIO_17 | Match |
| 18 | XL2/GPIO_18 | Match |
| 19 | GPIO_19 | Match |
| 20 | GPIO_20 | Match |
| 21 | VBUS | Match |
| 22 | NFC1/GPIO_22 | Match |
| 23 | NFC2/GPIO_23 | Match |
| 24 | GPIO_24 | Match |
| 25 | GPIO_25 | Match |
| 26 | GPIO_26 | Match |
| 27 | GPIO_27 | Match |
| 28 | GPIO_28 | Match |
| 29 | GPIO_29 | Match |
| 30 | GPIO_30 | Match |
| 31 | GPIO_31 | Match |
| 32 | GPIO_32 | Match |
| 33 | GPIO_33 | Match |
| 34 | USBDP | Match |
| 35 | USBDM | Match |
| 36 | GPIO_36 | Match |
| 37 | GPIO_37 | Match |
| 38 | GPIO_38 | Match |
| 39 | GPIO_39 | Match |
| 40 | GPIO_40 | Match |
| 41 | SWDCLK | Match |
| 42 | SWDIO | Match |
| 43 | GND | Match |
| 44 | GND | Match |
| 45 | GND | Match |
| 46 | GND | Match |
| 47 | GPIO_47 | Match |
| 48 | GPIO_48 | Match |
| 49 | GPIO_49 | Match |
| 50 | GPIO_50 | Match |
| 51 | GPIO_51 | Match |
| 52 | GPIO_52 | Match |
| 53 | GND | Match |
| 54 | GND | Match |
| 55 | GND | Match |
| 56 | GND | Match |
