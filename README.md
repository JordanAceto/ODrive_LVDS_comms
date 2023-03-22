# Set of small PCBs for Odrive ◄► motor encoder comms

- One board sits on an Odrive
- The other goes inside a gimbal motor
- They are connected with twisted pair wire
- The goal is to increase noise immunity and have convenient connectors
- One Odrive board can connect to two encoder boards

---

### Connectors used
- JST GH series 9 pin

---

### IMPORTANT NOTE 1
- The encoder board PCB should be 1mm thick
- The ODRive board can be any thickness you like

---

### IMPORTANT NOTE 2
- The two SN65LVDS050PW chips on the ODrive board will conflict if you use only one motor at a time
- Setting the chip select line high for a given SN65LVDS050PW chip puts its SDI pin into a high impedance state
- If the chip select line is low or not active, the SN65LVDS050PW chip will assert its output on the shared SDI line
- When using only 1 motor there are two options:
  - set the chip select line for the unused SN65LVDS050PW permanently high
  - only solder one SN65LVDS050PW chip

---

### Status
- test build done, safe to order boards
