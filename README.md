# Network Discovery Tool

## Overview
The Network Discovery Tool is a Flask application designed for network scanning and management. It provides functionalities for device discovery, service detection, and network topology mapping.

## Installation

1. **Clone the Repository** (if applicable):
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Dependencies**:
   Ensure you have Python installed, then install the required packages:
   ```bash
   pip install flask scapy nmap apscheduler reportlab
   ```

3. **Set Up the Database**:
   The application initializes the database when it starts. Ensure that the `network.db` file is in the same directory as `app.py`.

## Running the Application

1. **Set the FLASK_APP Environment Variable**:
   ```bash
   set FLASK_APP=app.py
   ```

2. **Start the Flask Application**:
   ```bash
   flask run
   ```

3. **Access the Application**:
   Open your web browser and navigate to `http://127.0.0.1:5000` to interact with the application.

## Features

- **Device Discovery**: API endpoint to list devices on the network.
- **Service Detection**: Identify services running on devices.
- **Network Topology Mapping**: Visualize the network structure.
- **Alerting System**: Monitor for anomalies in the network.

## Usage

- Use the `/api/devices` endpoint to retrieve a list of devices.
- Export data in CSV format using the `/export/csv` endpoint.
- Manage schedules through the `/schedules` endpoint.

## License
This project is licensed under the MIT License.
