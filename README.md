# STM32 Real-Time Embedded Control System

**Real-Time Embedded Firmware | STM32F407 | ARM Cortex-M4 | FreeRTOS | Embedded C**

A real-time embedded control system developed using the **STM32F407 microcontroller and FreeRTOS**, integrating multitasking, sensor acquisition, signal processing, motion estimation, control logic, and telemetry.

The firmware was developed and successfully operated on physical hardware in a real-world engineering application, demonstrating reliable execution of time-sensitive embedded operations.

The project showcases practical experience in **Embedded C programming, ARM Cortex-M microcontrollers, RTOS-based software architecture, peripheral configuration, communication protocols, and hardware–software integration**.

## Technical Stack

| Category | Technologies |
|---|---|
| Microcontroller | STM32F407, ARM Cortex-M4 |
| Programming | Embedded C, C/C++ |
| Development Environment | STM32CubeIDE, STM32CubeMX |
| Real-Time Operating System | FreeRTOS |
| Hardware Peripherals | GPIO, ADC, PWM, Timers, EXTI |
| Communication Interfaces | UART, SPI, I2C, USB CDC |
| Sensor Processing | Moving Average, Low-Pass Filter |
| Sensor Fusion | Madgwick Algorithm |
| Libraries | STM32 HAL, CMSIS |

## Key Engineering Highlights

### FreeRTOS-Based Multitasking Architecture

Designed and implemented a real-time firmware architecture using **five dedicated FreeRTOS tasks**:

- **Control Task:** System state management and control operations.
- **Navigation Task:** Sensor-based motion calculations and measurement processing.
- **IMU Task:** Inertial sensor acquisition and orientation processing.
- **Sensor Task:** Sensor monitoring and data acquisition.
- **Telemetry Task:** System data collection and communication.

The architecture separates time-sensitive operations into dedicated tasks, supporting modular software development and coordinated execution.

### STM32 Peripheral Programming

Configured and integrated STM32 hardware peripherals for embedded control and sensor communication.

Practical experience includes:

- GPIO configuration and digital I/O
- Hardware timers and microsecond-resolution timing
- PWM-based peripheral control
- ADC configuration
- External interrupts (EXTI)
- UART serial communication
- SPI and I2C peripheral communication

### Sensor Integration and Signal Processing

Developed sensor interfacing and measurement-processing functionality for multiple sensor types.

Implemented:

- Sensor acquisition and event processing
- Moving Average and Low-Pass filters
- Sensor noise reduction
- Timing-based measurement processing
- Integration of multiple measurement sources

### Motion Estimation and Sensor Fusion

Developed motion estimation functionality using sensor measurements and hardware timing.

Key implementations include:

- Instantaneous and average speed calculations
- Acceleration estimation
- Distance and elapsed-time calculations
- Microsecond-resolution timing using STM32 timers
- Madgwick sensor fusion algorithm
- Roll, pitch, and yaw orientation estimation

### Embedded Control and System Coordination

Implemented state-based control logic to coordinate system operations.

The firmware integrates control outputs, sensor feedback, timing mechanisms, and task execution within a unified embedded architecture.

### Telemetry and Communication

Integrated embedded communication interfaces for sensor data exchange and system monitoring.

- UART communication
- SPI and I2C device interfacing
- USB CDC communication
- Telemetry data preparation and transmission

## Reliability and Hardware Integration

The firmware was successfully deployed and operated on the target hardware during the original engineering application.

Development involved:

- Hardware–software integration
- Peripheral configuration and debugging
- Sensor datasheet analysis
- Measurement filtering and timing analysis
- Embedded firmware troubleshooting
- Real-time system integration

The project provided hands-on experience developing and validating embedded software in a practical hardware environment.

## Repository Structure

```text
Core/
├── Inc/                 # Application header files
├── Src/                 # Embedded application and RTOS logic
└── Startup/             # MCU startup configuration

Drivers/                 # STM32 HAL and CMSIS

Middlewares/             # FreeRTOS and USB middleware

USB_DEVICE/              # USB CDC implementation

STM32_Real_Time_Control_System.ioc
                         # STM32CubeMX configuration
```

## Selected Source Files

| File | Description |
|---|---|
| `Core/Src/main.c` | MCU initialization and application configuration |
| `Core/Src/freertos.c` | FreeRTOS tasks and application logic |
| `Core/Src/madgwick.c` | Madgwick orientation estimation implementation |
| `Core/Src/onewire.c` | OneWire sensor communication |
| `Core/Inc/FreeRTOSConfig.h` | FreeRTOS configuration |

## Engineering Competencies Demonstrated

**Embedded Systems Development · Embedded C · STM32 · ARM Cortex-M4 · FreeRTOS · Real-Time Systems · RTOS Task Management · Microcontroller Peripherals · Interrupts · UART · SPI · I2C · PWM · ADC · Timers · Sensor Integration · Digital Signal Filtering · Sensor Fusion · Embedded Debugging · Hardware–Software Integration**

## Third-Party Components

The repository includes STM32 HAL, CMSIS, FreeRTOS, and USB middleware components under their respective licenses.
