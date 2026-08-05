# Linker Scripts (.ld)

Defines memory layout for the linker.
Maps sections:
- .text: Code
- .rodata: Read-only data (const)
- .data: Initialized globals (copied from flash to RAM on boot)
- .bss: Uninitialized globals (zeroed on boot)