# Bash/SH Commands

Frequently used Bash/Shell commands for managing processes and network resources.

## Kill a process using PID:
1. **Find the process ID (PID)**:
    ```bash
    sudo lsof -t -i:<port>
    ```

2. **Kill the process**:
    ```bash
    sudo kill -9 <PID>
    ```

