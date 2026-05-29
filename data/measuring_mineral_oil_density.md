# Lab Note: Measurement of Mineral Oil Density

**Date:** May 29, 2026  
**Project:** Hexbug Active Matter / Neutral Buoyancy Experiment  
**Location:** Biophysics Lab 317  

---

## Research Goal

The goal of this experiment was to measure the density of the mineral oil used in the Hexbug active matter experiment.

This density value will be used to estimate the buoyant force acting on the Hexbug and to calculate the amount of additional flotation material needed to make the Hexbug system close to neutrally buoyant.

---

## Background

A submerged object experiences an upward buoyant force equal to the weight of the fluid it displaces. Therefore, to design a neutrally buoyant Hexbug system, we need to know the density of the surrounding fluid.

Density is calculated as:

```text
Density = Mass / Volume
```

where:

```text
Density: g/mL
Mass: g
Volume: mL
```

For neutral buoyancy:

```text
Buoyant force = Weight
```

or equivalently:

```text
Density of fluid × Displaced volume = Total mass of object
```

For this experiment, the surrounding fluid is mineral oil.

---

## Materials

- Mineral oil
- Graduated cylinder
- Pipette
- Funnel
- Electronic balance

---

## Procedure

1. Cleaned and dried the graduated cylinder.
2. Measured the mass of the empty graduated cylinder.
3. Added 20.0 mL of mineral oil to the graduated cylinder using a pipette and funnel.
4. Measured the mass of the graduated cylinder containing the mineral oil.
5. Calculated the mass of the mineral oil:

```text
Mass of oil = Mass of cylinder with oil − Mass of empty cylinder
```

6. Calculated the density of the mineral oil:

```text
Density = Mass of oil / Volume of oil
```

7. Repeated the same procedure using 30.0 mL and 40.0 mL of mineral oil.
8. Calculated the average density from all trials.

---

## Data

| Trial | Cylinder Mass (g) | Volume of Oil (mL) | Cylinder + Oil Mass (g) | Oil Mass (g) | Density (g/mL) |
|---:|---:|---:|---:|---:|---:|
| 1 | 54.21 | 20.0 | 71.02 | 16.81 | 0.8405 |
| 2 | 54.21 | 30.0 | 79.53 | 25.32 | 0.8440 |
| 3 | 54.21 | 40.0 | 88.04 | 33.83 | 0.8458 |

---

## Result

The average measured density of the mineral oil was:

```text
Average density = 0.8434 g/mL
```

The three trials gave similar density values, suggesting that the measurement was reasonably consistent.

---

## Conclusion

The experimentally measured density of the mineral oil was **0.8434 g/mL**.

This value is close to commonly reported mineral oil density values, which are usually around **0.85–0.87 g/mL**, depending on the exact type and grade of mineral oil. The small difference may come from experimental uncertainty, air bubbles, reading the liquid level, or variation in the specific mineral oil sample.

This measured value will be used in later buoyancy calculations for the Hexbug experiment.

---

## Sources of Uncertainty

Several sources of uncertainty may have affected the density measurement:

1. **Air bubbles in the mineral oil**  
   Air bubbles were visible in the mineral oil. These bubbles occupy volume but add very little mass, which may cause the measured density to be slightly lower than the true value.

2. **Oil sticking to the graduated cylinder wall**  
   Some mineral oil remained on the inside wall of the graduated cylinder. This made the liquid level harder to read accurately and introduced uncertainty in the volume measurement.

3. **Balance uncertainty**  
   The electronic balance had a measurement uncertainty of approximately ±0.01 g. This uncertainty affects the measured oil mass and therefore the calculated density.

4. **Meniscus / volume reading uncertainty**  
   Mineral oil is more viscous than water, so reading the exact volume in the graduated cylinder was less precise.

Despite these uncertainties, the repeated measurements were consistent, so the average density of **0.8434 g/mL** is reliable enough for the next stage of buoyancy calculations.

---

## Connection to the Hexbug Neutral Buoyancy Experiment

The measured density will be used to estimate how much mineral oil must be displaced for the Hexbug system to become neutrally buoyant.

The measured mass of the Hexbug is:

```text
Mass of Hexbug = 7.4 ± 0.1 g
```

The density of the mineral oil is:

```text
Density of mineral oil = 0.8434 g/mL
```

For neutral buoyancy:

```text
Density of oil × Displaced volume = Total mass of Hexbug system
```

Therefore:

```text
Required displaced volume = Total mass of Hexbug system / Density of mineral oil
```

Using only the Hexbug mass as a first estimate:

```text
Required displaced volume = 7.4 g / 0.8434 g/mL
Required displaced volume ≈ 8.77 mL
```

Since:

```text
1 mL = 1 cm³
```

the Hexbug system would need to displace approximately:

```text
8.77 cm³ of mineral oil
```

to be neutrally buoyant.

---

## Next Step

The next step is to measure the actual displaced volume of the Hexbug system.

This can be done by placing the Hexbug and attached flotation material into a container filled with mineral oil, collecting the overflow oil, and measuring the overflow volume.

The overflow volume will tell us the displaced volume of the full Hexbug system.

If:

```text
Displaced volume < 8.77 mL
```

then the Hexbug system is too dense and needs more flotation material.

If:

```text
Displaced volume > 8.77 mL
```

then the Hexbug system is too buoyant and needs less flotation material or added mass.

If:

```text
Displaced volume ≈ 8.77 mL
```

then the Hexbug system is close to neutrally buoyant in mineral oil.

---

## Notes for Future Work

- Measure the volume of the bare Hexbug.
- Measure the volume of the Hexbug with attached Styrofoam.
- Keep the Styrofoam attachments symmetric to avoid unintentionally creating rotational bias.
- Record whether the Hexbug is floating, sinking, touching the bottom, or suspended in the oil.
- Use video tracking to compare speed, trajectory, and turning radius under different buoyancy conditions.
