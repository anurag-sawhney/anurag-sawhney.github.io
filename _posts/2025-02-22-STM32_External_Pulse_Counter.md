title: "STM32_External_Pulse_Counter"
date: 2025-02-22
CubeMX Setup for a timer to operate in external clock mode in order to count an input pulse rate and store it in a buffer.

Usually, STM32 controllers have 32 bit timers viz. TIM2 and TIM5. 
Using 32 bit timers is preferable in order to prevent timer overflow due to high frequency input. 

As an example, TIM5 Mode and Configuration (in STM32CUBEMX)
Slave Mode: External Clock Mode 1
Trigger Source: TI1_ED
Channel 1: Input Capture triggered by TRC.
Prescaler: 0
Counter Mode: Up
Counter Period: 0xFFFFFFFF
Internal Clock Division: No Division
Auto-reload preload: Disable
Slave Mode Controller: ETR mode 1
IC Selection: TRC

