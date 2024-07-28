
# WebVM App1 - webapp-dev-web-linuxvm-1

## Overview
Welcome to the WebVM App1 hosted on the `webapp-dev-web-linuxvm-1` virtual machine. This server is part of the cloud marathon project and serves a simple web application.

## Server Details
- **VM Hostname:** webapp-dev-web-linuxvm-1
- **IP Address:** 52.226.122.181
- **SSH Port:** 1022 (Default SSH access)
- **Web Application Port:** 80 (Default HTTP)

## Web Application
The main webpage for the application is located at `/var/www/html/index.html`. It displays a welcome message and other relevant information.

### Directory Structure
- `/var/www/html`: Contains the web application's HTML files.
  - `index.html`: The main landing page.
  - `app1`: Directory for additional application files and resources.

## How to Access
1. **SSH Access**:
   - To access the server via SSH, use the following command:
     ```bash
     ssh azureuser@52.226.122.181 -p 1022
     ```
   - Use the provided password or SSH key for authentication.

2. **Web Access**:
   - The web application can be accessed via a web browser at `http://52.226.122.181/`.

## Maintenance and Updates
- **System Updates**: Regularly update the system using the package manager.
  ```bash
  sudo yum update -y
  ```
- **Web Application Updates**: Place updated files in the appropriate directories under `/var/www/html`.

## Additional Information
- This system is not registered with Red Hat Insights. You can register it by following the instructions at [Red Hat Cloud](https://cloud.redhat.com/).
- To enable the web console, run:
  ```bash
  sudo systemctl enable --now cockpit.socket
  ```

## Contact
For any issues or inquiries, please contact the system administrator.

---

**Note**: Ensure to secure the server and regularly back up important data.
