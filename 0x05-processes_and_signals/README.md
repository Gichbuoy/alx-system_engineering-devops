## Processes and Signals

### Process
* A process refers to an instance of a computer program that is being executed by the operating system.
- It represents the running state of a program and includes the program's code, data, and the resources allocated to it.
- When a program is executed, the operating system creates a process to manage its execution. Each process has its own memory space, which includes the program instructions, variables, and data specific to that instance of the program. The process also has its own stack, heap, registers, and other resources needed for execution.

- Processes are fundamental units of work in an operating system. They can run concurrently or sequentially, depending on the operating system's scheduling algorithm and available system resources. Multiple processes can run simultaneously, allowing users to multitask and run multiple programs concurrently.

- Processes communicate with each other through interprocess communication mechanisms provided by the operating system, such as shared memory, pipes, sockets, or message queues. They may also interact with system resources, such as files, devices, network connections, and other processes.

- Each process is identified by a unique Process Identification Number (PID) assigned by the operating system. This PID allows the operating system to track and manage the processes effectively, including process creation, termination, scheduling, resource allocation, and interprocess communication.

### Signal
* A signal is a software interrupt or notification sent to a process to notify it of a particular event or to request a specific action. Signals are a form of interprocess communication used by the operating system to handle various scenarios, such as process termination, user interruptions, or exceptional events.

- Signals can be sent by the operating system, other processes, or by the process itself. When a process receives a signal, it can either ignore it, perform a default action associated with the signal, or have a custom signal handler that executes a specific function in response to the signal.

* Some commonly used signals include:

- SIGINT (Signal Interrupt): This signal is typically sent by the operating system to a process when the user presses the interrupt key combination, which is usually Ctrl + C. By default, it requests the process to terminate gracefully. Processes can have custom signal handlers to handle SIGINT and perform any necessary cleanup or termination procedures.

- SIGKILL (Signal Kill): This signal is sent by the operating system to forcibly terminate a process. Unlike other signals, SIGKILL cannot be ignored or caught by the process. When a process receives SIGKILL, it is immediately terminated without any chance to perform cleanup or execute custom actions. The SIGKILL signal is often used as a last resort to terminate unresponsive or misbehaving processes.
