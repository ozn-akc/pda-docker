# Installations

To set up and run the program, follow the steps below:

1. Run the following command to start the Docker containers:

    ```bash
    docker-compose up
    ```

2. For local testing, the following services will be available:

    - **MQTT**: `localhost:1883`
    - **Rhasspy**: `localhost:12101`

3. When running the agent in local mode, make sure to activate the "local" Spring Boot profile for testing purposes. You can typically set the active profile as an environment variable or within your application configuration.

    Example:

    ```bash
    gradle build
    java -jar /folder/agent.jar --spring.profiles.active=local
    ```
    
## Setup

Train the Dataset in Rhasspy

## Local Testing


1.  Install Python 3.11 for the IO-Interface.

2. For the Python I/O interface, navigate to the `io-interface/` directory and run the following commands:

    ```bash
    cd io-interface/
    pip install -r requirements.txt
    python3 main.py
    ```

```bash
