---
draft: true
description:
socialDescription:
title: DC to DC Converters
tags:
  - wiki/electrical
date: 2025-03-13
modified: 2025-08-21
---
![[Pasted image 20250313084400.png]]
[[Buck Converter]]
[[Boost Converter]]
[[Buck - boost Converter]]

[[(LDO) Low Dropout Regulator]]

# input [[Capacitor]] of DCDC
| Converter Type | Input Cap Importance | Output Cap Importance |
| -------------- | -------------------- | --------------------- |
| **Buck**       | ✅✅✅ High             | ✅ Moderate–High       |
| **Boost**      | ✅ Moderate           | ✅✅✅ High              |
| **Buck-Boost** | ✅✅✅ High (both!)     | ✅✅✅ High              |
## [[Buck Converter]]
- **Switch is between input and inductor**
- It **draws pulsed current** from the **input cap**
- Input cap must:
    - Absorb sharp switching pulses    
    - Prevent **VIN bounce, EMI**, and **ripple into the power rail**
- Output is **filtered through the inductor**, so **ripple is easier to manage**
✅ **Input cap is more stressed** → needs low ESR, tight placement, and enough capacitance
## [[Boost Converter]]
- Switch is between **ground and inductor**; **input current is continuous**
- But the **output cap sees pulsed current** every switch cycle
- Output cap must:
    - **Absorb charge dumps** from the inductor during switch-off    
    - Maintain output voltage during the switch cycle
✅ **Output cap is more stressed** → must be carefully sized to maintain voltage and limit ripple
