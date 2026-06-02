# Lab Note — 2026/05/29
## Making the Hexbug Neutrally Buoyant

## Objective

The goal of this calculation was to estimate how much flotation material is needed to make the Hexbug neutrally buoyant in mineral oil.

A neutrally buoyant object does not strongly sink or float. Instead, its total weight is balanced by the buoyant force from the surrounding fluid.

---

## Measurements

| Quantity | Value |
|---|---:|
| Mass of Hexbug | 7.4 ± 0.1 g |
| Gravitational acceleration | 9.81 m/s² |
| Density of mineral oil | 0.8434 ± 0.018 g/mL |
| Volume of Hexbug | 5.665 ± 0.001 cm³ |
| Density of foam | 0.177 ± 0.026 g/cm³ |
| Density of cork | 0.199 ± 0.034 g/cm³ |

---

## Neutral Buoyancy Condition

For the Hexbug with flotation material to be neutrally buoyant:

> Total Mass = Total Volume × Density of Mineral Oil

The total mass is:

> Total Mass = Hexbug Mass + Float Mass

The float mass is:

> Float Mass = Float Density × Float Volume

So the full equation is:

> Hexbug Mass + Float Density × Float Volume  
> = Mineral Oil Density × (Hexbug Volume + Float Volume)

Solving for float volume:

> Float Volume = (Hexbug Mass - Mineral Oil Density × Hexbug Volume) / (Mineral Oil Density - Float Density)

---

## Foam Calculation

Using foam as the flotation material:

| Quantity | Value |
|---|---:|
| Hexbug mass | 7.4 g |
| Mineral oil density | 0.8434 g/cm³ |
| Hexbug volume | 5.665 cm³ |
| Foam density | 0.177 g/cm³ |

Calculation:

> Float Volume = (7.4 - 0.8434 × 5.665) / (0.8434 - 0.177)

Result:

> Required foam volume ≈ 3.93 cm³

Uncertainty estimate:

> ΔV ≈ 0.34 cm³

Final foam result:

> Required foam volume = 3.93 ± 0.34 cm³

---

## Practical Foam Design

To balance the Hexbug, the foam should be divided into two equal pieces.

Total required foam volume:

> 3.93 cm³

Volume per foam piece:

> 3.93 cm³ / 2 ≈ 1.97 cm³

A practical design is:

> Two foam blocks, each about 2.0 cm × 1.0 cm × 1.0 cm

This gives:

> Volume per block = 2.0 cm³  
> Total foam volume = 4.0 cm³

This is close to the calculated required volume.

---

## Cork Calculation

Using cork as the flotation material:

| Quantity | Value |
|---|---:|
| Cork density | 0.199 ± 0.034 g/cm³ |

Calculated result:

> Required cork volume ≈ 4.02 ± 0.38 cm³

---

## Result Summary

| Flotation Material | Required Volume |
|---|---:|
| Foam | 3.93 ± 0.34 cm³ |
| Cork | 4.02 ± 0.38 cm³ |

Both foam and cork require approximately 4 cm³ of material to make the Hexbug neutrally buoyant in mineral oil.

---

## Design Decision

Foam may be easier to cut and attach symmetrically.

The first prototype should use:

- Two foam pieces
- Each piece: approximately 2.0 cm × 1.0 cm × 1.0 cm
- Total volume: approximately 4.0 cm³

This setup should be tested experimentally in mineral oil.

---

## Next Steps

1. Cut two equal foam pieces.
2. Attach one foam piece to each side of the Hexbug.
3. Place the Hexbug in mineral oil.
4. Observe whether it sinks, floats, or stays close to neutrally buoyant.
5. Adjust foam size if needed.
6. Record video from above.
7. Use tracking code to analyze the Hexbug's motion.

---

## Notes

The calculation assumes that the flotation material is fully submerged and that the mineral oil density is uniform.

In the actual experiment, the result may differ because of:

- Trapped air bubbles
- Tape or waterproofing material
- Uneven foam shape
- Imperfect symmetry
- Oil sticking to the robot
- The Hexbug touching the bottom or side walls

The experimental test will be necessary to confirm whether the calculated foam volume works.
