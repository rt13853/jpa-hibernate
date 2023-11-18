# TCP Dashboard

This project simulates a TCP Dashboard application for monitoring and configuring load patterns for multiple clients transmitting data to a server.

## Instructions

1. Run the `Main` class to start the TCP server, dashboard, and simulate clients.
2. Use the dashboard to configure load patterns for each client.

## Design Choices

- **JavaFX for Dashboard UI:** JavaFX was chosen for the dashboard's user interface due to its ease of use and capabilities for building interactive desktop applications.

- **Multi-Threading:** Each client simulator and client communication with the server are handled in separate threads to allow concurrent execution. Also tried different ports for each client for execution but due to system limitation opted this approach.

## Challenges Faced

- **Real-Time Statistics:** Implementing real-time statistics on the dashboard proved to be challenging. A dedicated mechanism needs to be implemented for updating the UI in real-time based on the server's and clients' activities.

- **Load Pattern Execution:** Ensuring seamless transition between load patterns and executing them as per the configured schedule requires careful synchronization and handling of time intervals.

- **Dynamic Configuration:** Dynamically configuring and adding clients at runtime while ensuring proper communication and simulation presented some complexities.
