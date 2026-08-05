# Priority Inversion

When a high-priority task is blocked waiting for a resource held by a low-priority task, and a medium-priority task preempts the low-priority task.

## Solution
**Priority Inheritance**: The low-priority task temporarily inherits the priority of the high-priority task waiting on the resource.