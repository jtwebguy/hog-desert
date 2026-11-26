# Hog Desert

A low-poly A-10C Thunderbolt II flight sim that runs in the browser. One HTML file, Three.js from a CDN, no build step.

**Play:** https://jtwebguy.github.io/hog-desert/ (or open `index.html` locally).

## Flight model

- Six-degree-of-freedom rigid body integrated at 240 Hz.
- A-10C figures: 16,000 kg gross, 47 m² wing, 17.53 m span, 2 × 40.3 kN TF34-GE-100A with thrust lapse and slow spool-up.
- Lift curve with stall at 16° AoA, post-stall flat-plate behaviour, nose-down pitch break and wing drop.
- Stability and damping derivatives for pitch, roll and yaw; sideslip, dihedral effect, adverse yaw.
- Flaps (UP / MVR / DN) with nose-down trim change, drag, and approximate overspeed blow-up (DN above 185 KIAS, MVR above 220); split-aileron speed brakes, landing gear drag, ground effect, light thermal turbulence.
- Spring-damper landing gear with nosewheel steering (offset right, as on the real jet), wheel brakes, parking brake, runway vs. dirt friction.
- Field elevation 2,297 ft, standard atmosphere.

## World

Procedural low-poly desert: dunes, mesas, a mountain ring. Runway 18/36 with markings, numbers, PAPI, taxiways, apron, hangars, tower and parked A-10s.

## Controls

| Action | Keyboard |
|---|---|
| Pitch (↓ = pull back) | ↑ / ↓ |
| Roll | ← / → |
| Rudder / nosewheel | A / D |
| Throttle | W / S |
| Wheel brakes (first press releases parking brake) | Space |
| Flaps | F |
| Gear | G |
| Speed brakes | B |
| Pitch trim | [ / ] |
| Camera (chase, cockpit, orbit, tower) | C |
| Restart on runway / air start | R / T |
| Pause / help / mute | P / H / M |

Gamepad: left stick pitch and roll, right stick X rudder, triggers throttle, A brakes, B gear, X flaps, Y speed brakes, bumpers trim, Back camera, Start pause.

## Takeoff and landing

Takeoff: release the brake, full throttle, track the centerline, rotate gently around 115–120 KIAS, gear up once climbing, flaps up above 160 KIAS.

Landing: gear down, flaps DN, 130–140 KIAS on final. The PAPI left of runway 36 shows two white and two red on a 3° glide path.
