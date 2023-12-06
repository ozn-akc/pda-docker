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
    java -jar your_agent.jar --spring.profiles.active=local
    ```

    Or if using a script:

    ```bash
    ./your_agent_script.sh --spring.profiles.active=local
    ```

## Setup

Train the Dataset in Rhasspy

## Local Testing

To test the agent locally, make sure the Docker containers are up and running, and then use the specified MQTT and Rhasspy endpoints mentioned above.

```bash
# Example command for local testing
java -jar your_agent.jar --spring.profiles.active=local
