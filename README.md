# Minimal Multi-Tasking OS Kernel for ARM

## Prerequisites
- [QEMU with STM32 support](http://beckus.github.io/qemu_stm32/)
- [GNU Toolchain for ARM](https://launchpad.net/gcc-arm-embedded)
- Set `$PATH` accordingly

## Steps
1. **Hello World:** Basic semihosted ARM Cortex-M output
2. **USART:** Enable STM32 USART for printing
3. **Context Switching:** Switching between user/kernel mode
// (tbd)
5. **System Calls:** Implement basic system calls
6. **Multitasking:** Switch between multiple tasks
7. **Preemptive Scheduling:** Enable SysTick for scheduling
8. **User-Level Threads:** Implement threading
9. **CMSIS Integration:** Hardware abstraction layer (HAL) support

## Build & Run
```sh
make
make qemu
```

## Flash to STM32F429i-Discovery
```sh
make f429disco
make st-flash
```

## Debugging
- QEMU GDB: `make qemu_GDBstub`
- Real Device GDB: `make gdb_ST-UTIL`
