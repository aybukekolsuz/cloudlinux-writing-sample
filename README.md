# CloudLinux - Technical Writing Internship Application Task

This repository contains the completed submission for the technical writing task, as part of my application for the Technical Writing Internship position at CloudLinux.

The original developer notes have been rewritten into clear, user-friendly documentation sections as requested.

---

## Task 1: Installation Instructions

### Installation

These instructions outline the steps to install the package on RPM-based Linux systems (e.g., RHEL, CentOS, Fedora). The process involves running a setup script and then installing the package using `yum`.

#### Prerequisites

* `git` and `yum` (or `dnf`) must be installed on your system.
* You must have `sudo` or root privileges.

#### Installation Steps

1.  **Clone the Repository**
    Clone the repository containing the installation script.

    ```bash
    git clone [https://github.com/company/example-repo.git](https://github.com/company/example-repo.git)
    ```

2.  **Run the Installation Script**
    Navigate to the cloned directory and execute the `install` script. This will prepare your system for the package installation.

    ```bash
    cd example-repo
    sudo sh install.sh
    ```

3.  **Install the Package**
    After the script finishes, use `yum` to install the specific version of the package.

    ```bash
    sudo yum install package-name-1.2.3
    ```

### Clarifying Questions for the Team

To improve this documentation, I would need the following information from the development team:

* **Repository URL:** What is the correct URL for the git repository? (`https://github.com/company/example-repo.git` is a placeholder).
* **Script Name:** Is the script's name exactly `install` or does it have an extension (e.g., `install.sh`)?
* **Script Function:** What does the `install.sh` script do? (e.g., Does it add a YUM repository, install dependencies, or modify system configurations?)
* **Package Name:** What is the exact "needed package" name? (`package-name` is a placeholder).
* **Version:** Why is a "specific version" required? How does the user find this version number? Can the user simply run `sudo yum install package-name`?
* **Privileges:** Does the `sh install.sh` command require `sudo`? (It is assumed in the guide but needs confirmation).

---

## Task 2: Uninstalling the Package

### Uninstalling the Package

If you need to remove the package from your system, you can use the `yum` package manager.

1.  Open your terminal.
2.  Run the following command with `sudo` privileges to remove the package.

    > **Note:** Use the package name (e.g., `mypackage`), not the `.rpm` filename you may have used to install it.

    ```bash
    sudo yum remove mypackage
    ```

3.  `yum` will list the package to be removed along with any dependencies that are no longer required.
4.  To confirm the uninstallation, press `y` and then **Enter**.
