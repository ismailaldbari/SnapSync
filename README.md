# SnapSync

SnapSync is a simple and efficient command-line tool for creating, updating, and restoring system snapshots using `rsync`. It is designed to simplify backup and restore operations, making it easy to manage your system's snapshots.

---

## Features

- **Create New Snapshots**: Create a new system snapshot with a custom or default name.
- **Update Existing Snapshots**: Update an existing snapshot to reflect the latest system state.
- **Restore Snapshots**: Restore your system from a previously created snapshot.
- **Exclusion List**: Automatically excludes unnecessary files and directories (e.g., `/dev`, `/proc`, `/tmp`).
- **Metadata**: Generates a JSON file with metadata about each snapshot.

---

## Prerequisites

SnapSync relies on `rsync` for its operations. Make sure `rsync` is installed on your system before using SnapSync.

### Install `rsync`

On most Linux distributions, you can install `rsync` using your package manager:

- **Debian/Ubuntu**:
  ```bash
  sudo apt update
  sudo apt install rsync

Usage

    Create a Backup:

        Choose option 1 from the menu.

        Select N to create a new snapshot or U to update an existing one.

        Follow the prompts to complete the backup process.

    Restore a Backup:

        Choose option 2 from the menu.

        Enter the number of the snapshot you want to restore.

        Confirm the restore operation.

    Exit:

        Choose option 3 to exit the script.

Configuration

    Backup Directory: Modify the BACKUP_DIR variable in the script to specify where snapshots should be stored.

    Exclusions: Edit the EXCLUSIONS array to add or remove directories/files from the exclusion list.

Why SnapSync?

SnapSync is designed to be a lightweight and user-friendly alternative to tools like Timeshift. It relies on rsync, a powerful and reliable utility, to handle backup and restore operations. Unlike Timeshift, SnapSync is entirely command-line based, making it ideal for advanced users and automation.
Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
License

This project is licensed under the MIT License. See the LICENSE file for details.
