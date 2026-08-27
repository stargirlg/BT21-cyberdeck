# BT21 Cyberdeck

A portable software engineering platform built from repurposed hardware, designed for learning and experimenting with Linux, Python development, Git, shell scripting, automation, and mobile-based software engineering.

The project uses an **OPPO A37 Android smartphone** as the main computing device and **Termux** to provide a Linux-like terminal development environment.

![BT21 Cyberdeck](images/cyberdeck.png)

---

## Project Goals

The main goal of this project is to build a functional portable development workstation using inexpensive and repurposed hardware.

* Build a portable development workstation
* Reuse existing hardware instead of buying a complete computer
* Configure a Linux-like development environment on Android
* Develop Python applications
* Use Git and GitHub for version control
* Practice Linux shell commands
* Experiment with automation and scripting
* Learn how hardware and software can be combined into a practical system
* Document the complete engineering process

---

## Hardware

### Main Computing Device

* **OPPO A37 smartphone**
* Android operating system
* Built-in display
* Built-in battery
* Wi-Fi connectivity

The smartphone acts as the main computer of the Cyberdeck.

### Additional Hardware

The remaining physical components are used to turn the smartphone into a portable workstation.

* External keyboard
* Cyberdeck enclosure/body
* Mounting material
* Cables/accessories required for the setup
* Recycled/repurposed materials where possible

> The hardware configuration may change as the project evolves.

---

## Software

### Operating Environment

The Cyberdeck uses Android as the base operating system.

**Termux** provides the terminal environment used for software development.

### Development Tools

* Termux
* Python 3.8
* Git
* GitHub
* Bash/Shell environment

---

# Step-by-Step Setup

## Step 1 — Prepare the Smartphone

The OPPO A37 is used as the main computing device.

Before starting:

1. Charge the phone.
2. Remove unnecessary applications if storage is limited.
3. Connect the phone to Wi-Fi.
4. Make sure there is enough storage for development tools and projects.
5. Keep the phone accessible for installing and configuring software.

The phone does not need to be rooted for the basic Cyberdeck setup.

---

## Step 2 — Install Termux

Install **Termux** on the Android phone.

After installation, open Termux.

The first objective is to make sure the terminal environment is working correctly.

Run:

```bash
pkg update
```

Then:

```bash
pkg upgrade
```

Confirm the installation when Termux asks for permission.

---

## Step 3 — Install Basic Development Tools

Install Git:

```bash
pkg install git
```

Check that Git is installed:

```bash
git --version
```

Install Python:

```bash
pkg install python
```

Check the Python version:

```bash
python --version
```

The current project environment uses Python 3.8.

---

## Step 4 — Configure Termux Storage

Allow Termux to access shared Android storage:

```bash
termux-setup-storage
```

Android will ask for storage permission.

Allow the permission.

Termux will then provide access through:

```text
~/storage/
```

You can check the available directories with:

```bash
ls ~/storage
```

---

## Step 5 — Create a Workspace

Create a directory for Cyberdeck projects:

```bash
mkdir ~/cyberdeck
```

Move into it:

```bash
cd ~/cyberdeck
```

Check the current directory:

```bash
pwd
```

---

## Step 6 — Test Python

Create a simple Python file:

```bash
nano hello.py
```

Add:

```python
print("Hello from BT21 Cyberdeck!")
```

Save the file and run:

```bash
python hello.py
```

Expected output:

```text
Hello from BT21 Cyberdeck!
```

This confirms that Python development is working.

---

## Step 7 — Configure Git

Check Git:

```bash
git --version
```

Configure your Git identity:

```bash
git config --global user.name "Your Name"
```

```bash
git config --global user.email "your-email@example.com"
```

Verify the configuration:

```bash
git config --global --list
```

---

## Step 8 — Clone the Cyberdeck Repository

Clone this repository:

```bash
git clone https://github.com/stargirlg/BT21-cyberdeck.git
```

Enter the project directory:

```bash
cd BT21-cyberdeck
```

Check the files:

```bash
ls
```

---

## Step 9 — Run the Project Environment

From the project directory, use the available Python scripts or development files.

For a Python script:

```bash
python filename.py
```

For example:

```bash
python hello.py
```

The exact command depends on the application being developed.

---

# Physical Assembly

The Cyberdeck is designed around the smartphone rather than a traditional single-board computer.

### Basic assembly process

1. Prepare the enclosure/body.
2. Create a secure mounting position for the OPPO A37.
3. Position the phone so the display remains visible.
4. Attach the external keyboard.
5. Organize the cables.
6. Secure loose components.
7. Check that the phone can be removed when necessary.
8. Test the complete setup before permanently fixing components.

The physical design can be modified as the project develops.

---

# Using the Cyberdeck

Once the hardware and software are ready:

### 1. Turn on the phone

Start the Android device.

### 2. Open Termux

Launch the Termux terminal.

### 3. Enter the project

```bash
cd ~/cyberdeck/BT21-cyberdeck
```

### 4. Check the repository

```bash
git status
```

### 5. Create or edit code

Python files can be created directly from Termux.

Example:

```bash
nano program.py
```

### 6. Run the program

```bash
python program.py
```

---

# Git Workflow

The Cyberdeck can also be used as a complete Git development environment.

Check changes:

```bash
git status
```

Add files:

```bash
git add .
```

Create a commit:

```bash
git commit -m "Update Cyberdeck project"
```

Push changes:

```bash
git push
```

Pull the latest changes:

```bash
git pull
```

This allows development directly from the Cyberdeck without requiring a traditional PC.

---

# Current Capabilities

The current Cyberdeck provides:

* Android-based computing
* Termux terminal environment
* Linux command-line environment
* Python development
* Git version control
* GitHub integration
* Shell scripting
* Portable development environment
* Repurposed hardware

---

# Technology Stack

| Category             | Technology          |
| -------------------- | ------------------- |
| Hardware             | OPPO A37            |
| Operating System     | Android             |
| Terminal Environment | Termux              |
| Programming          | Python 3.8          |
| Version Control      | Git                 |
| Repository           | GitHub              |
| Shell                | Bash / Termux Shell |

---

# Project Structure

```text
BT21-cyberdeck/
│
├── images/
│   └── cyberdeck.png
│
├── README.md
│
└── ...
```

Additional files and directories will be added as the Cyberdeck software develops.

---

# Troubleshooting

## Termux command not found

Update the package repository:

```bash
pkg update
pkg upgrade
```

Then install the required package.

For Python:

```bash
pkg install python
```

---

## Python is not working

Check:

```bash
python --version
```

If Python is missing:

```bash
pkg install python
```

---

## Git is not working

Check:

```bash
git --version
```

If Git is missing:

```bash
pkg install git
```

---

## Storage permission problem

Run:

```bash
termux-setup-storage
```

Then allow Android storage permission.

---

# Future Improvements

Planned improvements include:

* Better physical enclosure
* Improved keyboard integration
* Additional USB peripherals
* Portable power improvements
* More Python development tools
* Local web development
* Network utilities
* Automation scripts
* Hardware monitoring
* Custom Cyberdeck interface
* Improved cable management
* More software projects running directly on the Cyberdeck

---

# Project Philosophy

The BT21 Cyberdeck is not intended to compete with a modern laptop in raw performance.

The purpose is to demonstrate that useful software engineering work can be performed using **repurposed hardware, open-source software, and a small development environment**.

The project focuses on learning by building, experimenting, breaking things, fixing them, and documenting the process.

---

# License

This project is licensed under the **MIT License**.
