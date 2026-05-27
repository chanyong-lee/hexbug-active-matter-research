# Office Hours Notes — 2026/05/27

## Overview

Today, we discussed the scientific papers we read and connected them to our summer research project.  
The main focus was how Hexbug motion can be studied as a simple active matter system and how we can experimentally track its movement in different environments, especially mineral oil.

We talked about possible hypotheses, experimental setup, video tracking, and whether extra hardware such as a Raspberry Pi is necessary.

---

## Main Discussion Topics

### 1. Neutrally Buoyant Hexbug

One major question was:

**What would happen if we make the Hexbug neutrally buoyant?**

A neutrally buoyant Hexbug would not strongly sink or float. It would stay suspended or nearly suspended in the fluid.

Possible hypothesis:

- If the Hexbug is not touching the bottom surface, its normal walking motion may become weaker.
- This is because a normal Hexbug depends on friction between its angled legs and the surface.
- If it is floating freely in mineral oil, it may vibrate, rotate, wobble, or drift instead of moving forward normally.

Important question:

**Would it move clockwise or counterclockwise?**

At this stage, we should not assume the direction. The turning direction may depend on several factors:

- Weight symmetry
- Motor rotation direction
- Shape of the body
- Contact with the surface
- Fluid drag
- Whether the Hexbug is floating, sinking, or touching the bottom

Current hypothesis:

- If the Hexbug is still touching a surface, weight asymmetry may matter more.
- If the Hexbug is freely suspended in the fluid, the motor direction may become more important.
- We need experiments to test this instead of assuming the answer.

---

### 2. Hexbug in Mineral Oil

We discussed putting the Hexbug in mineral oil to study how its motion changes in a more viscous fluid.

Questions to investigate:

- Does the Hexbug still move forward?
- Does it turn more or less than on a dry surface?
- Does mineral oil slow down the motion?
- Does the Hexbug move in circles?
- Does the motion depend on whether it floats, sinks, or touches the bottom?

Important measurements:

- Position over time
- Speed
- Turning direction
- Radius of circular motion
- Angular velocity
- Reynolds number

---

### 3. Video Tracking Plan

We discussed how to track the Hexbug using code.

The basic plan is:

1. Record the experiment from above.
2. Put a clear colored marker on the Hexbug.
3. Use code to track the marker position frame by frame.
4. Save the tracked position data.
5. Plot the trajectory and calculate motion quantities.

Tracking will be easier if the Hexbug has a distinct mark, such as:

- Bright colored sticker
- Waterproof paint dot
- One marker for position
- Two markers for position and orientation

Using two markers would be better because it allows us to measure both the location and the direction the Hexbug is facing.

---

### 4. iPhone Camera vs Raspberry Pi

We discussed whether we need to use a Raspberry Pi as a video particle tracking device.

Current decision:

**A Raspberry Pi is probably not necessary at the beginning.**

The iPhone camera is good enough for the first experiments because:

- It has high-quality video.
- It can record slow-motion video.
- It can record up to 240 FPS.
- It is easier to set up quickly.
- We can analyze the video afterward using Python/OpenCV.

The Raspberry Pi could be useful later if we want:

- Real-time tracking
- Automated recording
- A fixed tracking system
- A cheaper permanent lab setup

For now, the simpler approach is better:

**Use iPhone first, analyze video later.**

---

### 5. Container Choice

We discussed what kind of container would be best for the experiments.

Best initial choice:

**A clear rectangular container with a flat bottom.**

Reasons:

- Easier to film from above
- Less image distortion than a curved container
- Easier to calibrate distance
- Easier to track the Hexbug
- Clear walls allow observation from the side if needed

Avoid for now:

- Round bowls
- Curved containers
- Containers with reflective or uneven bottoms
- Containers that are too small

A good first size would be around:

**30 cm × 20 cm or larger**

The container should be large enough that the Hexbug does not immediately hit the walls. If the container is too small, wall effects may dominate the motion.

---

### 6. TrackMate and Python/OpenCV

We talked about using TrackMate as a reference for tracking.

TrackMate could be useful because it is already designed for particle tracking, but Python/OpenCV may be better for this project because it gives us more control.

Possible tracking tools:

- TrackMate / Fiji / ImageJ
- Python
- OpenCV

Current plan:

- Use TrackMate as a reference or comparison.
- Start building our own simple Python/OpenCV tracking code.
- First goal: track one colored marker on the Hexbug.
- Later goal: track two markers and measure orientation.

---

### 7. Code Modification Plan

The first version of the code should be simple.

Initial code goals:

- Load a video file
- Detect a colored marker
- Find the marker center
- Track the marker position over time
- Save the data as a CSV file
- Plot the trajectory

Later code goals:

- Convert pixels to centimeters
- Calculate speed
- Calculate turning angle
- Calculate angular velocity
- Detect clockwise vs counterclockwise motion
- Calculate radius of curvature
- Compare motion in different fluids

---

### 8. Real-Time Video Tracking

We discussed the possibility of real-time tracking.

Setup idea:

- iPhone camera placed above the experiment
- Camera records top-down video
- The video is used to track the Hexbug motion

For now, real-time tracking is not the priority.

Current priority:

1. Record clean video.
2. Analyze video after recording.
3. Confirm that tracking works.
4. Then consider real-time tracking later.

Real-time tracking would be useful, but it may make the project more complicated too early.

---

## Main Takeaways

- The Hexbug’s motion depends strongly on surface contact, friction, vibration, weight balance, and fluid drag.
- If the Hexbug becomes neutrally buoyant, its motion may change completely because it may lose contact with the surface.
- We should not assume clockwise or counterclockwise motion before testing.
- Weight asymmetry may dominate when the Hexbug touches a surface.
- Motor direction may become more important if the Hexbug is freely suspended.
- The iPhone camera is enough for the first tracking experiments.
- A clear rectangular container is the best first experimental container.
- A bright marker on the Hexbug will make tracking much easier.
- Python/OpenCV is likely the best starting point for custom tracking code.
- Real-time tracking can be added later after basic video tracking works.

---

## Next Steps

1. Record a simple top-down video of a Hexbug moving on a dry surface.
2. Add a bright colored marker to the Hexbug.
3. Write or modify Python/OpenCV code to track the marker.
4. Save the trajectory data as a CSV file.
5. Plot the Hexbug path.
6. Repeat the experiment in a container.
7. Then test motion in mineral oil.
8. Compare dry-surface motion and mineral-oil motion.

---

## Short Summary

Today’s discussion connected the paper reading to our experimental plan.  
The next practical goal is to build a simple video tracking workflow before making the setup more complicated with neutral buoyancy, Raspberry Pi, or real-time tracking.
