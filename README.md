# solar-charger-pwm
Work in progress lead-acid solar charge controller...

Using circuitlab (https://www.circuitlab.com/circuit/vx6fj82sf5gy/12v-solar-charger-pwm/) for basic testing of circuit.

I originally designed this as part of a LoRa based wiresless sensor, but I decided to go back to 3.7V with 12V boost conversion for that project.

This project will hopefully grow into a functional PWM lead-acid solar charger and maybe an MPPT solar charger if I have time.

Current testing was focused on a fixed input voltage of 18V with small lead-acid batteries between 1.2Ah and 7.2Ah. The arduino code does take the battery through its different charge stages (bulk, absorption and float), but the the current code the length absorption phase it still too short.

The circuit will also have to change when using a PV source: extra protection on MOSFET gate; better reverse polarity protection, smaller current sense resistor, etc.
