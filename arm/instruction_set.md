# ARM Instruction Set Reference (Thumb-2)

## Data Processing
`ssembly
ADD R0, R1, R2  ; R0 = R1 + R2
SUB R0, R1, #1  ; R0 = R1 - 1
AND R0, R1, R2  ; R0 = R1 & R2
`

## Memory Access
`ssembly
LDR R0, [R1]    ; Load word from address in R1 into R0
STR R0, [R1]    ; Store word from R0 to address in R1
`

## Branching
`ssembly
B label         ; Branch to label
BL label        ; Branch with Link (subroutine call)
CMP R0, #0      ; Compare R0 with 0
BEQ label       ; Branch if equal (Z flag set)
`
"@

Upload-File -path "arm/interrupts_nvic.md" -message "Add NVIC and interrupts notes" -contentStr @"
# Interrupts and NVIC

The Nested Vectored Interrupt Controller (NVIC) manages all interrupts and exceptions in Cortex-M.

## Key Features
- Configurable priorities
- Tail-chaining for fast interrupt handling
- Late arrival handling

## Priority Grouping
Priority is divided into preemption priority and sub-priority.
- Preemption Priority: Higher priority preempts lower priority ISR.
- Sub-priority: If preemption is same, higher sub-priority executes first (no preemption).