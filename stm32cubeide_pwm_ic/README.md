# stm32cubeide_pwm_ic
unable to run itcallback function, why is this happen?

TIM1 Channel 1 is configured for PWM generation (CH1). Then, TIM2 is set up for merged channel PWM input on CH1. In this configuration, TIM2's CH1 captures the high level and triggers an interrupt, while CH2 captures the low level. However, when running the main function, the inability to enter the interrupt callback function is perplexing. (All three channels are enabled, and TIM2 interrupts are also enabled.)