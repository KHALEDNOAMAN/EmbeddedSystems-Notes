# FreeRTOS API Reference

## Task Creation
`c
xTaskCreate(
    vTaskCode,       /* Function */
    "NAME",          /* Name */
    STACK_SIZE,      /* Stack depth */
    NULL,            /* Parameters */
    PRIORITY,        /* Priority */
    &xHandle         /* Task handle */
);
`
"@

Upload-File -path "rtos/semaphores_mutexes.md" -message "Add Synchronization notes" -contentStr @"
# Semaphores and Mutexes

## Mutex
Used for mutual exclusion. Protects shared resources. Includes priority inheritance to prevent priority inversion.

## Semaphore
Used for signaling (Binary Semaphore) or counting resources (Counting Semaphore).