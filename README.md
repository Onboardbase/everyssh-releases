
# EverySSH App Server

This repository contains the source code for the EverySSH App Server.

## Overview

The EverySSH App Server is a lightweight server application written in Go. Users need to authenticate via CLI before starting the server.

## Installation

To download and install the latest release of the EverySSH App Server binary, visit the [releases page](https://github.com/Onboardbase/everyssh-app-server/releases).

### Example Installation

1. **Download the Binary**:

    ```sh
    wget https://github.com/Onboardbase/everyssh-app-server/releases/download/v0.2/everyssh-server
    ```

2. **Make the Binary Executable**:

    ```sh
    chmod +x everyssh-server
    ```

3. **Authenticate**:

    ```sh
    ./everyssh-server auth
    ```

    Follow the prompts to enter your Machine Key and Machine Secret. The authentication details will be saved securely.

4. **Run the Server**:

    ```sh
    ./everyssh-server
    ```

