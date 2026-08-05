# Register Access

Registers are accessed as volatile pointers.

`c
#define GPIOA_BASE  0x40020000
#define GPIOA_ODR   (*(volatile uint32_t *)(GPIOA_BASE + 0x14))

// Write to ODR
GPIOA_ODR |= (1 << 5);
`
"@

Upload-File -path "cheatsheets/common_mistakes.md" -message "Add Common Mistakes notes" -contentStr @"
# Common Pitfalls

- Forgetting olatile on ISR shared variables.
- Stack overflow from large local arrays.
- Memory leaks from dynamic allocation.
- Missing pull-up resistors on I2C lines.
- Unhandled default interrupts (HardFault).