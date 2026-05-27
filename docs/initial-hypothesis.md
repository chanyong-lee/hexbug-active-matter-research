# Initial Hypothesis: Hexbug Motion in Mineral Oil

## Research Question

What happens to the motion of a Hexbug when it is placed in mineral oil and modified to become closer to neutrally buoyant?

More specifically, we want to understand whether the Hexbug will continue to move forward, whether it will rotate clockwise or counterclockwise, and which physical factors control its motion: surface contact, weight symmetry, motor direction, fluid viscosity, or temperature.

## Background

A normal Hexbug moves using a vibration-based mechanism. Its internal motor creates rapid vibrations, and its angled rubber legs convert those vibrations into forward motion through friction with a solid surface. Therefore, the Hexbug's normal motion is not true swimming. It is closer to a walking or crawling motion driven by vibration and surface friction.

This is different from bacterial swimming. For example, *E. coli* uses rotating helical flagella to move through fluid. Near a solid boundary, bacteria can swim in circular trajectories because the rotating flagella interact hydrodynamically with the nearby wall. This creates asymmetric viscous drag and a torque that turns the bacterium.

Because of this difference, the Hexbug should not be considered a perfect mechanical model of bacteria. Instead, it can be used as a macroscopic active matter system that helps us study general behaviors such as persistent motion, chirality, surface interaction, confinement, and changes in motion due to fluid environment.

## Hypothesis 1: Neutrally Buoyant Motion

If the Hexbug becomes close to neutrally buoyant in mineral oil and loses strong contact with the bottom surface, its normal forward motion will become weaker.

This is because the Hexbug's usual propulsion depends on contact between its legs and a solid surface. If buoyancy reduces the normal force between the legs and the surface, then the friction-based walking mechanism should become less effective. Instead of moving forward in a stable path, the Hexbug may mainly vibrate, wobble, rotate, or drift.

## Hypothesis 2: Clockwise vs. Counterclockwise Motion

The direction of circular motion will depend on the experimental condition.

If the Hexbug remains in contact with the bottom surface, the turning direction will likely be dominated by mechanical asymmetry, especially weight placement and leg-surface friction. Adding more weight to one side should create an imbalance in vibration and friction, causing the Hexbug to turn preferentially in one direction.

If the Hexbug is freely suspended or nearly neutrally buoyant, weight asymmetry may become less important because the legs are no longer strongly pushing against a surface. In that case, the internal motor direction and asymmetric fluid drag may have a larger influence on rotation.

Therefore, the initial prediction is:

- Bottom-contact motion: weight symmetry and leg friction may dominate.
- Freely suspended motion: motor direction and fluid drag may become more important.

## Hypothesis 3: Effect of Mineral Oil and Temperature

Mineral oil is more viscous than air and may significantly slow down the Hexbug's motion. The increased viscous drag should reduce speed and may change the turning radius or angular velocity.

Temperature should also be tracked because the viscosity of mineral oil can change with temperature. If the Hexbug motor or battery heats the surrounding oil during operation, the oil viscosity may decrease, which could affect the measured speed and trajectory. For this reason, temperature data should be recorded during experiments using the Arduino temperature sensor.

## Experimental Variables to Separate

To understand the cause of the motion, the following conditions should be tested separately:

1. Hexbug on a dry surface  
   - Baseline motion without mineral oil.

2. Hexbug in mineral oil while touching the bottom  
   - Tests how viscosity affects friction-based motion.

3. Hexbug floating near the surface of mineral oil  
   - Tests partial buoyancy and surface/interface effects.

4. Hexbug adjusted toward neutral buoyancy  
   - Tests whether motion persists when strong surface contact is removed.

5. Hexbug with added weight on different sides  
   - Tests how weight asymmetry affects clockwise or counterclockwise motion.

6. Multiple Hexbugs or repeated trials  
   - Tests whether the motion is consistent or specific to one robot.

## Expected Measurements

For each trial, we should record:

- Position over time
- Speed
- Direction of motion
- Turning radius
- Angular velocity
- Clockwise or counterclockwise rotation
- Temperature of the fluid
- Experimental condition, including fluid, depth, buoyancy state, marker position, and added weight

## Main Interpretation

If the Hexbug moves in circles in mineral oil, we should be careful about the explanation. Circular motion alone does not mean the Hexbug is moving by the same mechanism as bacteria.

A better interpretation is:

The Hexbug can serve as a macroscopic active matter model for studying how self-propelled objects respond to viscosity, chirality, surface contact, and confinement. However, its propulsion mechanism is different from bacterial flagellar swimming, so the comparison should focus on general active matter behavior rather than exact biological similarity.
