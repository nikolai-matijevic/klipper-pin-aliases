# klipper-pin-aliases

Change your configuration from this:
```
[tmc2209 stepper_x]
uart_pin: P1.17
diag_pin:P1.29
step_pin: P2.2
dir_pin: P2.6
enable_pin: !P2.1
endstop_pin: P1.29
```

To this:
```
[tmc2209 stepper_x]
uart_pin: m0_uart
diag_pin:m0_diag
step_pin: m0_step
dir_pin: m0_dir
enable_pin: !m0_enable
endstop_pin: m0_min
```

The main reason I create those configurations is to make it easier to create, expand and change configurations while also making them easy to read by omitting the pin names themselves.

Using the provided configuration files as guides for naming the aliases can make it possible to switch boards with minimal changes needed in the ```printer.cfg```.

I will try and add more boards as I get to it. If you have made a configuration file with pin aliases you can help expand this repository by creating a pull request. Please make sure that you use the correct pins as I don't have the time to verify every configuration myself.

If you don't know how to create such a configuration file, you can make a board request.