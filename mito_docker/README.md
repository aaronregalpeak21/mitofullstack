# Mito Docker Project

## Overview
The Mito Docker project is designed to provide a comprehensive environment for developing and deploying various modules related to educational management, enterprise resource planning, human resource management, lending, insights, and more. This project utilizes Docker to manage services and dependencies efficiently.

## Project Structure
The project consists of the following directories and files:

- **apps_custom/**: This directory contains the source code and resources for the custom modules.
  - **lms/**: Source code and resources for the LMS module.
  - **erpnext/**: Source code and resources for the ERPNext module.
  - **hrms/**: Source code and resources for the HRMS module.
  - **lending/**: Source code and resources for the Lending module.
  - **insights/**: Source code and resources for the Insights module.
  - **charts/**: Source code and resources for the Charts module.
  - **frappe_whatsapp/**: Source code and resources for the Frappe WhatsApp module.
  - **anything-llm/**: Source code and resources for the Anything LLM module.
  - **OCEANAI/**: Source code and resources for the OCEANAI module.
  - **FinRobot/**: Source code and resources for the FinRobot module.

- **docker-compose.yml**: This file defines the services, networks, and volumes for the Docker application. It includes configurations for the MariaDB, Redis, site-creator, Frappe, worker, scheduler, and n8n services, along with their dependencies and environment variables.

## Setup Instructions
1. **Clone the Repository**: Clone this repository to your local machine.
2. **Navigate to the Project Directory**: Open a terminal and navigate to the `mito_docker` directory.
3. **Create Custom Apps Directory**: Run the following commands to create the `apps_custom` directory and clone the necessary repositories:
   ```bash
   mkdir apps_custom
   cd apps_custom
   git clone https://github.com/aaronregalpeak21/lms.git
   git clone https://github.com/aaronregalpeak21/erpnext.git
   git clone https://github.com/aaronregalpeak21/hrms.git
   git clone https://github.com/aaronregalpeak21/lending.git
   git clone https://github.com/aaronregalpeak21/insights.git
   git clone https://github.com/aaronregalpeak21/charts.git
   git clone https://github.com/aaronregalpeak21/frappe_whatsapp.git
   git clone https://github.com/aaronregalpeak21/anything-llm.git
   git clone https://github.com/aaronregalpeak21/OCEANAI.git
   git clone https://github.com/aaronregalpeak21/FinRobot.git
   cd ..
   ```
4. **Start the Docker Services**: Run the following command to start all services defined in the `docker-compose.yml` file:
   ```bash
   docker-compose up -d
   ```

## Usage Guidelines
- Access the Frappe application at `http://localhost:8000`.
- Access the n8n automation tool at `http://localhost:5678`.

## Additional Information
For any issues or contributions, please refer to the respective module repositories or contact the project maintainers.