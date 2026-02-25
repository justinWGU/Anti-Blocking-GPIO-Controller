# Anti-Blocking GPIO Controller using Priority-Based Interrupts

## An STM32 project written in C to prevent long-running ISRs from blocking more important ones.

### About

This project simulates a long-running ISR by using a busy loop, which is then 
preempted by a higher-priority interrupt to prevent blocking. This is known
as preemption. This firmware consists of the following:

- two interrupts of varying priority (buttons)
- a GPIO out (red LED)
- lower priority button lights the LED in a busy loop
- higher priority button preempts the lower priority ISR and turns off LED

#### Technologies Used

- C
- HAL library
- STM32F401RE Microcontroller
- STM32CubeIDE

#### References
- HAL API: UM1725 Description of STM32F4 HAL and low-layer drivers
- Peripheral registers: RM0368 Reference manual
