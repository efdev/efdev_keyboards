# PCBs

# Firmware

Based on zmk.

Basic setup see https://zmk.dev/docs/development/setup .

Extend zmk west.yml remotes list with the following 

```
- name: microsoft
      url-base: https://github.com/microsoft
```
and the projects list with
```
- name: uf2
      remote: microsoft
      path: tools/uf2
      clone-depth: 1
```
and run `west update`

Build firmware `west build -p -b <board> -- -DBOARD_ROOT=<path to cloned repo>/Firmware`

Example: `west build -p -b akortho -- -DBOARD_ROOT=/home/efdev/Documents/Keyboards/Firmware`
