Load Average
============

* 0.00 to 1.00 means the processor is not backed up, and processes get CPU time right away. 1.00 means the CPU is at 100% utilization. Above 1.00 means processes are waiting.
* 1.00 is full utilization of 1 core. A box with multiple cores is safe below `1.00 * num_cores`.
* When considering load average, a single core processor is effectively treated the same as a single processor core.

