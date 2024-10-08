# 📊 Server Health Monitoring - Python Automation 🛠️

## Overview

This project monitors server health, visualizes metrics, and sends notifications. It uses Python for backend tasks and Dash for a web-based dashboard.

## Setup

### Prerequisites

- Python 3.x
- Required Python packages (listed in `requirements.txt`)

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Eswari123-cloud/system_health_monitoring
   cd system_health_monitoring
   
2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt

4. **Set Up the Database**
   ```python
   from database.db_utils import create_table_if_not_exists

   db_filename = 'servers.db'
   create_table_if_not_exists(db_filename)

6. **Import Server Data**
   Prepare a CSV file named servers.csv with columns hostname and ip.
   Import data into the database
   ```python
   from database.db_utils import insert_servers_from_csv

   csv_filename = 'servers.csv'
   insert_servers_from_csv(csv_filename, db_filename)

## Running the Application
**Start the Web Dashboard**

**To run the web application and view the dashboard**:
 - python app.py
 - Access the dashboard at http://127.0.0.1:8050/
## Features
1. **Real-Time Monitoring**
  - View CPU, memory, and disk usage metrics.
2. **Visualizations**
  - Interactive graphs for server performance.
3. **Anomaly Detection**
  - Detect and highlight anomalies in system metrics.
4. **Notifications**
  - Send alerts via email and Microsoft Teams.
5. **Automatic Cleanup**
  - Perform disk cleanup if usage exceeds a threshold.
6. **Dashboard**
  - Comprehensive web-based interface for monitoring and visualizing server health.

## Code Overview
- **database/db_utils.py:** Functions for database operations.

    - **create_table_if_not_exists(db_filename):** Creates the servers table.
    - **insert_servers_from_csv(csv_filename, db_filename):** Imports server data from a CSV file.
- **utils/data.py:** Generates sample data for testing.

     - **generate_sample_data(server_name):** Creates synthetic data for a given server.
- **app.py:** Initializes the Dash web application and handles interactive visualizations.

- **plot/figures.py:** Contains functions for generating charts and graphs.

## Contributing
1. **Fork the repository.**
2. **Create a new branch:** git checkout -b feature-branch.
3. **Make your changes.**
4. **Commit and push:**
   ```bash
   git commit -am 'Add new feature'
   git push origin feature-branch.
5. **Open a Pull Request.**

## License

This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details.

## Contact

### For questions, open an issue on GitHub or email smsivasankaraeswari@outlook.com
---

## Made with passion and code by [⭐ Sivasankara Eswari Mahalingam ⭐ ](https://github.com/Eswari123-cloud)

Coding is my passion. Your feedback is always welcome. ✨

🚀 Happy Coding! 🚀



