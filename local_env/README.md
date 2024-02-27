# Local Environment Setup

This README provides instructions for setting up the local development environment.

## Prerequisites

ensure you have the following installed on your local machine:

- Docker
- PostgreSQL
- Python
- Pip

## Setup Instructions

Follow these steps to set up your local environment:

1. **Install Docker:**
   - Download and install Docker from the official website: [Docker](https://www.docker.com/get-started)

2. **Install PostgreSQL:**
   - You can install PostgreSQL by downloading and installing it from the official website: [PostgreSQL](https://www.postgresql.org/download/)
   - Alternatively, you can use Docker to run a PostgreSQL container:
     ```bash
     docker run --name postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres
     ```

3. **Install Python:**
   - Download and install Python from the official website: [Python](https://www.python.org/downloads/)

4. **Install Pip:**
   - Pip usually comes installed with Python. If not, you can install it using the following command:
     ```bash
     python -m ensurepip --default-pip
     ```

5. **Clone the Repository:**
   - Clone this repository to your local machine using Git:
     ```bash
     git clone <repository-url>
     ```

6. **Navigate to Project Directory:**
   - Change directory to the project folder:
     ```bash
     cd <project-folder>
     ```

7. **Run Ansible Playbook:**
   - Execute the provided Ansible playbook to check the installed dependencies:
     ```bash
     ansible-playbook -i inventory.ini check_prerequisites.yaml
     ```

8. **Verify Setup:**
   - Once the playbook completes, verify that all dependencies are installed correctly by checking the output.

## Troubleshooting

If you encounter any issues during the setup process, refer to the following troubleshooting tips:

- Ensure that Docker, PostgreSQL, Python, and Pip are installed correctly and accessible from the command line.
- Double-check the versions of installed dependencies to ensure compatibility with the application.
- Review the Ansible playbook output for any error messages or warnings that may indicate issues with the setup process.

If you're unable to resolve the issue, feel free to reach out for assistance.

## Contributors

- [Your Name](https://github.com/yourusername)

## License

This project is licensed under the [MIT License](LICENSE).

