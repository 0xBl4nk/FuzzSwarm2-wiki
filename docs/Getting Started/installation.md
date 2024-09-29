# Installation Guide

Follow the steps below to install and build FuzzSwarm on your system.

## Prerequisites

Ensure you have the following tools installed:

- **Golang** (version 1.23.1 or higher)
- Git
- Make

## Steps to Install

1. Clone the FuzzSwarm repository from GitHub:
   ```bash
   git clone https://github.com/0xBl4nk/FuzzSwarm2
   ```
2. Navigate to the project directory:
   ```bash
   cd FuzzSwarm2
   ```
3. Build the application using make:
   ```bash
   make build
   ```
This command will create the FuzzSwarm binary in the current directory.

4. To verify the installation, run the following command:
   ```bash
   ./FuzzSwarm --help
   ```

---

You're now ready to start using FuzzSwarm. Learn how to use it in the [Usage Guide](Usage/overview.md).