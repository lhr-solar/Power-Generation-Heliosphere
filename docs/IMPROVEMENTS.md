# IMPROVEMENTS

- [IMPROVEMENTS](#improvements)
  - [Digital PWM control](#digital-pwm-control)

---

## Digital PWM control

After verifying that v0.1.0 works with analog trimpots, the next step would be
using a digital PWM controller to control brightness. This is useful in a couple
ways:

- Removes dependency on Dale trimpots, which don't appear to exist anymore
  outside of Hallock's lab
- The trimpots are large, which restricts the lighting density and therefore the
  maximum uniform irradiance incident upon the surface (e.g. farther the
  spacing, the more vertical distance required for even spread). Switching to a
  SOT-23-3 or similar package MOSFET hooked up to a controller reduces the size
  restriction drastically. Ideally we can get back to 40x40 mm instead of 50x50 mm.
- The digital control enables automagic feedback control. Hook up to the PV
  Curve Tracer and the Blackbody B, and then we can automatically tune segment
  brightness as well as emulate various PVEnvironment regimes that are only
  usable in Eclipse simulation.