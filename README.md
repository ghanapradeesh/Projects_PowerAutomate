The bot performs the following core functions:

Queue-Based Execution:
Designed as a Performer Bot, it picks items from a predefined queue and processes them sequentially.

Config File Validation:
On initialization, the bot validates the required configuration file to ensure all necessary parameters (e.g., credentials, paths, environment settings) are available before proceeding.

Centrix Application Integration:
The bot logs into the Centrix application and creates orders based on input data from each queue item. After successful creation, it extracts:

Order Value

Order Reference Number
These details are then updated back into the respective queue item for downstream processes.

Centralized Retry Mechanism:
A robust, reusable retry logic is implemented to handle transient failures, ensuring reliability across various stages of the process.

Error Handling & Logging:

Exception handling is implemented across all stages with clear fallback and termination points.

A detailed CSV log is generated to capture each step, aiding in troubleshooting and post-deployment debugging.
