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