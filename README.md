# STM32F407ZGT_RTthread
正点原子STM32F407ZGT探索者RT-Thread
STMCubeIDE

1.编译选项
  关闭浮点单元
2.startup.s
  屏蔽bl __libc_init_array
  bl main => bl entry
3.board.c
  rt_hw_board_init中增加HAL_Init、SystemClock_Config
