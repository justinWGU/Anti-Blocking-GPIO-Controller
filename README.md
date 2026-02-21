# GPIO Control using Priority-Based Interrupts

## An STM32 project written in C using priority-based interrupts to control a GPIO pin.

### About

This project was created to solve the problem of long-running ISRs causing delays for more important ones. This project consists of the following:

- two interrupts of varying priority (buttons)
- a GPIO out (red LED)
- lower priority button lights the LED in a busy loop
- higher priority button preempts the lower priority ISR and turns off LED

#### Technologies Used

- C
- HAL library
- STM32F401RE Microcontroller
- STM32CubeIDE

#### License

#### Contact

#### References
