# Developer Documentation for Network Discovery Tool

## Project Structure
```
/network-discovery-tool
│
├── app.py                # Main application file
├── network.db            # SQLite database file
├── templates/            # Directory for HTML templates
│   └── dashboard.html     # Dashboard template
└── README.md             # User documentation
└── DEVELOPER.md         # Developer documentation
```

## Key Components

### app.py
- **Flask Application**: The main entry point for the application, where the Flask app is initialized and routes are defined.
- **Database Initialization**: The `init_db` function sets up the SQLite database schema.
- **NetworkScanner Class**: Handles network scanning and service discovery functionalities.

### Database Schema
The application uses SQLite for data storage. The following tables are defined:
- `networks`: Stores network information.
- `device_services`: Records services running on devices.
- `topology`: Maps the network topology.
- `alerts`: Logs alerts related to devices.
- `device_meta`: Stores metadata for devices.

### Web Routes
- **/api/devices**: API endpoint to retrieve a list of devices.
- **/export/csv**: Endpoint to export data in CSV format.
- **/schedules**: Endpoint to manage schedules for network scans.

## Development Guidelines
- Follow PEP 8 for Python code style.
- Use meaningful commit messages when making changes to the repository.
- Ensure that all new features are covered by unit tests.

## Testing
- To run tests, ensure that the testing framework is installed (e.g., `pytest`).
- Execute tests using the command:
  ```bash
  pytest
  ```

## License
This project is licensed under the MIT License.
