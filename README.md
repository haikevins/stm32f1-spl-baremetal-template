## Repo Structure
project/
├── app/                          # Application layer
│   ├── inc/
│   └── src/
│       └── main.c
│
├── bsp/                          # Board Support Package
│   ├── inc/
│   │   ├── bsp_led.h
│   │   ├── bsp_button.h
│   │   └── bsp_uart.h
│   └── src/
│       ├── bsp_led.c
│       ├── bsp_button.c
│       └── bsp_uart.c
│
├── middleware/                   # RTOS, FS, protocol stack nếu có
│   ├── inc/
│   └── src/
│
├── lib/                          # Utility libraries tự viết
│   ├── inc/
│   └── src/
│
├── third_party/                  # Code vendor / external, hạn chế sửa
│   ├── CMSIS/
│   └── STM32F10x_StdPeriph_Driver/
│       ├── inc/
│       └── src/
│
├── system/                       # Startup, system init, interrupt, syscall
│   ├── inc/
│   │   ├── stm32f10x_conf.h
│   │   └── stm32f10x_it.h
│   ├── src/
│   │   ├── system_stm32f10x.c
│   │   ├── stm32f10x_it.c
│   │   └── syscalls.c
│   └── startup/
│       └── startup_stm32f10x_md.s
│
├── linker/                       # Linker script
│   └── STM32F103C8Tx_FLASH.ld
│
├── scripts/                      # Flash/debug/helper scripts
│   ├── flash.sh
│   └── debug.sh
│
├── build/                        # Output: .elf, .hex, .bin, .map
│
├── Makefile
├── README.md
└── .gitignore
