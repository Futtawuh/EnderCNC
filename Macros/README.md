# E3CNC Macros for Workspace XYZ0 Positioning

## What These Macros Do and Why

These macros are designed to **manually set the workspace XYZ0** for basic milling tasks.

When you press a `ZERO` macro, the machine’s current position is saved into a **variables file**. This acts as a backup in case of:

- MCU failure
- Emergency Stop (E-stop) had to be pressed
- Firmware reset or crash

This removes the need to manually record XYZ coordinates before zeroing — everything is saved automatically!

---

## Failed Mid-Job? Firmware Restarted?

>  **Note:** This recovery method only works if you’re using the same workpiece and want to **resume** the job.

### Scenario:
Your job is running, and the MCU crashes, causing a firmware restart.  
Follow these steps to recover:

1. Press the `LOAD_OFFSETS` macro.
    - This will re-home the CNC and move it to the **last saved machine position**.
2. Press the `ZERO_ALL` macro.
    - This re-applies your previous workspace XYZ0.
3. Restart the original job.
    - If you're lucky, this might **save the workpiece** from becoming scrap!

---

## Manual Workpiece ZERO Position Setup

>  **Make sure the Dremel/Spindle is NOT spinning during setup!**

---

### Step-by-Step Guide Manual ZERO:

1. Attach the workpiece securely.
2. Home the CNC machine.
3. Move the CNC via Mainsail to position the bit roughly at the center of the workpiece.
4. Lower the Z-axis until the bit is about **1mm above** the workpiece.
5. Place a **thin sheet of paper** under the bit and slowly lower the Z-axis:
    - Stop when the bit **grabs the paper slightly** (you feel friction).
    - Press the `ZERO_Z` macro — this sets Z0.
6. Raise Z by **2–3mm** to avoid crashing into the workpiece if it’s not perfectly flat.
7. Move the CNC using XY controls to the corner you've defined as the origin in Fusion/CAM.
8. Press `ZERO_X` and `ZERO_Y` macros.
    - ✅ X and Y are now set to workpiece XY0.
    - ❌ Do **not** press `ZERO_Z` again.
9. Start your job from Mainsail.

> **Use PPE, dont crash and stay safe.**

---
