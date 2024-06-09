# Project Workspace Initialization

This project workspace is organized to efficiently manage and deploy infrastructure and backend services. The structure includes necessary Ansible playbooks and the backend project.

## Prerequisites

Ensure you have the following installed on your machine:
- Python 3.x
- Ansible
- Docker
- Git

## Setup Instructions

### Backend Project (ilef_cloud)

1. **Navigate to the `ilef_cloud` directory**:
   ```bash
   cd ilef_cloud
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run database migrations**:
   ```bash
   python manage.py migrate
   ```

4. **Start the development server**:
   ```bash
   python manage.py runserver
   ```

### Ansible Playbooks

1. **Navigate to the `playbooks` directory**:
   ```bash
   cd playbooks
   ```

2. **Run a playbook** (e.g., to set up Jenkins):
   ```bash
   ansible-playbook jenkins_playbook.yml
   ```

## Usage

- The backend project (`ilef_cloud`) provides the necessary APIs and functionalities.
- The Ansible playbooks in the `playbooks` directory automate the deployment and configuration of various services.
