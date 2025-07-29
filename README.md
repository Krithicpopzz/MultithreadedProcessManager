## Project Overview

This project implements a **multithreaded process manager** capable of managing multiple processes and threads using various scheduling policies. It utilizes `std::thread`, `std::mutex`, and `std::condition_variable` for proper thread synchronization, and offers a basic, console-based real-time dashboard to monitor process statuses.

### Project Structure

- **`src/`**: Contains the main source files for the process manager, including modules for process handling, scheduling algorithms, and dashboard functionality.
- **`include/`**: Contains header files with shared declarations used across different parts of the project.
- **`build/`**: The directory where the compiled output files will be stored.

### How to Build the Project

To compile the project using `g++`, run the following command:

```bash
g++ -std=c++20 -I./include -pthread src/process.cpp src/scheduler.cpp src/dashboard.cpp src/main.cpp -o build/MultithreadedProcessManager


### Running the Project

To run the project on a Linux/macOS terminal:

1. Navigate to the build directory:

    ```bash
    cd build/
    ```

2. Execute the program:

    ```bash
    ./MultithreadedProcessManager
    ```
