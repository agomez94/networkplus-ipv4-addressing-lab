# Exercise 1 – APIPA Addressing

## Objectives
- Investigate network adapter configuration
- Check APIPA connectivity

## Steps
1. Run `ipconfig` on ACIWIN11 → observe APIPA address (169.254.x.x).
2. Run `ipconfig /all` on ACIDM01 → confirm DHCP Enabled = Yes, but APIPA assigned.
3. Ping external (8.8.8.8) from APIPA → fails.
4. Ping local APIPA peer → succeeds.

## Evidence
- Screenshot: `../screenshots/apipa-ipconfig.png`
- Output: [apipa-ipconfig-all.txt](../apipa-ipconfig-all.txt)

## Reflection
APIPA provides local-only connectivity within 169.254.0.0/16 when DHCP is unavailable.
