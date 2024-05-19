
---

# iScale

iScale is a Flutter application that utilizes MQTT (Message Queuing Telemetry Transport) for real-time weight monitoring using an IoT device. This application provides a user-friendly interface to display the current weight received from the MQTT broker.

## Features

- **Real-time Weight Monitoring**: Continuously updates and displays the current weight from the MQTT broker.
- **Simple Interface**: Provides a clean and intuitive user interface for easy interaction.

## Getting Started

### Prerequisites

- Flutter SDK installed on your system.
- MQTT broker (such as HiveMQ Cloud) set up for communication with the IoT device.

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone <repository_url>
   ```

2. Navigate to the project directory:

   ```bash
   cd iScale
   ```

3. Install dependencies:

   ```bash
   flutter pub get
   ```

### Usage

1. Open the project in your preferred Flutter IDE (such as VSCode or Android Studio).

2. Configure the MQTT broker connection settings in the `MQTT.dart` file:

   ```dart
   client = MqttServerClient.withPort('your_broker_address', 'your_client_id', 8883);
   client.secure = true; // Enable secure connection (if required)
   client.securityContext = SecurityContext.defaultContext;
   ```

3. Run the application:

   ```bash
   flutter run
   ```


## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to help improve this project.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

---


