````markdown
# Interrupt Controller Simulation - IS2101

## Description
This Java program simulates an **Interrupt Controller** managing interrupts from multiple devices (Keyboard, Mouse, Printer) with prioritization and masking support. 
- Devices can be masked/unmasked to enable or disable interrupts.
- Interrupts are handled based on **priority**.
- ISR (Interrupt Service Routine) execution is logged with timestamps.

## Features
- Mask/unmask individual devices.
- Priority-based interrupt handling.
- ISR log display after simulation.
- Multi-threaded simulation for realistic device behavior.

## How to Compile and Run

### 1. Compile
Navigate to the `src` folder and run:
```bash
javac InterruptControllerShort.java
````

### 2. Run

```bash
java InterruptControllerShort
```

### 3. Expected Behavior

* Keyboard and Mouse interrupts are enabled.
* Printer interrupts are masked.
* Program runs for 8 seconds and then stops.
* ISR log is displayed at the end.

## Sample Output

```
Keyboard enabled
Mouse enabled
Printer masked
Mouse → ISR done
Keyboard → ISR done
Keyboard → ISR done
...
=== ISR Log ===
12:30:01 - Mouse
12:30:02 - Keyboard
12:30:03 - Mouse
...
Simulation complete.
```
