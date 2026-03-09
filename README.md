# 🛡️ Zombie API Discovery and Defense Platform


A cybersecurity proof-of-concept (PoC) designed to demonstrate the automated discovery, classification, and management of "Zombie" and "Shadow" APIs.

📖 Overview

In modern microservices architectures, APIs are often created, deprecated, and forgotten. These Zombie APIs (inactive/legacy) and Shadow APIs (undocumented/internal) represent a significant attack surface for organizations.

This prototype demonstrates a simplified workflow for:

Discovery: Scanning OpenAPI specifications.

Analysis: Correlating endpoints with simulated traffic logs.

Classification: Identifying risk levels based on usage and naming conventions.

Visualization: Providing a security dashboard for rapid decommissioning.

🚀 Key Features

Automated Scanning: Parses API documentation to build a central inventory.

Risk Engine:

🧟 Zombie Detection: Flags legacy endpoints with zero traffic.

🕵️ Shadow API Alerts: Identifies internal/debug endpoints exposed to the system.

⚠️ Risk Scoring: Assigns scores based on traffic and exposure.

Interactive Dashboard: Built with Streamlit for real-time security monitoring.

Lifecycle Management: Interface to simulate decommissioning of high-risk assets.

🛠️ Technology Stack

UI/Frontend: Streamlit

Backend/Logic: Python 3.x

Database: SQLite (SQLAlchemy ORM)

Data Analysis: Pandas

⚙️ Installation & Setup

Clone the repository:

git clone [https://github.com/your-username/zombie-api-prototype.git](https://github.com/your-username/zombie-api-prototype.git)
cd zombie-api-prototype


Install dependencies:

pip install -r requirements.txt


Run the application:

python -m streamlit run Zom_project.py


🧪 How to Use the Prototype

Once the dashboard opens, the inventory will be empty.

Navigate to the Sidebar and click "🚀 Run API Discovery Scan".

The engine will ingest the mock specifications and traffic logs.

Review the High Risk Alerts for any detected Zombie APIs.

Use the Traffic Analysis charts to identify underutilized resources.

📂 Project Structure

Zom_project.py: The main monolithic application containing the engine, database logic, and UI.

zombie_api.db: Local SQLite database generated after the first scan.

requirements.txt: List of necessary Python packages.
