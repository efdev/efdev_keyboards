# PCBs

# Firmware

Based on zmk.

Basic setup see https://zmk.dev/docs/development/setup .

Build firmware `west build -p -b <board> -- -DBOARD_ROOT=<path to cloned repo>/Firmware`

Example: `west build -p -b akortho -- -DBOARD_ROOT=/home/efdev/Documents/Keyboards/Firmware`
