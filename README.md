
# EverySSH App Server

This repository contains the source code for the EverySSH App Server.

## Overview

The EverySSH App Server is a lightweight server application written in Go. Users need to authenticate via CLI before starting the server.

## Installation

To download and install the latest release of the EverySSH App Server binary, visit the [releases page](https://github.com/Onboardbase/everyssh-app-server/releases).

### Example Installation

1. **Download the Binary and Installation Script**:

    ```sh
    wget https://github.com/Onboardbase/everyssh-releases/releases/download/v0.4/everyssh-server
    wget https://github.com/Onboardbase/everyssh-releases/releases/download/v0.4/install.sh
    ```

2. **Make the Binary and Installation Script Executable**:

    ```sh
    chmod +x everyssh-server
    chmod +x install.sh
    ```

3. **Run the Installation Script**:

    ```sh
    sudo ./install.sh
    ```

    This script will:
    - Copy the binary to `/usr/local/bin`.
    - Create the config directory and config file at `/etc/everyssh`.
    - Create and enable the systemd service.

4. **Authenticate**:

    ```sh
    ./everyssh-server auth
    ```

    Follow the prompts to enter your Machine Key and Machine Secret. The authentication details will be saved securely.

5. **Run the Server**:

    The server will run as a daemon and start automatically at boot time. You can check its status using:

    ```sh
    sudo systemctl status everyssh-server
    ```

