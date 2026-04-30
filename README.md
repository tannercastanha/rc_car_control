This project implements manual control of a 2WD RC car using an STM32 microcontroller and a FlySky transmitter/receiver system.

The STM32 reads PWM signals from the receiver and converts them into motor commands using a differential drive model.

Hardware used: 
- STM32-Nucleo-F446RE
- FS-i6X
- FS-iA6B
- TB6612FNG
- Yikeshu DIY 2WD Kit

Config:
- PA0 - TIM2_CH1
- PA1 - TIM2_CH2
- PA2 - USART_TX
- PA3 - USART_RX
- PA6 - TIM3_CH1
- PA7 - TIM3_CH2
- PB0 - GPIO_Output
- PB1 - GPIO_Output
- PB2 - GPIO_Output
- PB10 - GPIO_Output
- PB12 - GPIO_Output

User Labels:
- PB0 - AIN1
- PB1 - AIN2
- PB2 - BIN1
- PB10 - BIN2

TIM2:
- Clock Source: Internal Clock
- Channel 1: Input Capture direct mode
- Channel 2: Input Capture direct mode
- Prescaler 83
- Counter Period: 65535

TIM3:
- Clock Source: Internal Clock
- Channel 1: PWM Generation CH1
- Channel 2: PWM Generation CH2
- Prescaler 83
- Counter Period: 100
