# GitLab Open Script

![Banner Image](banner.jpg)

## Purpose

This script simplifies the process of opening the current file or directory in your GitLab repository directly from your terminal. It automatically determines the correct URL based on your Git configuration and opens it in your default web browser.

## Usage

1.  Navigate to the directory in your local Git repository that you wish to view on GitLab.
2.  Run the script `gitlab`.

The script will:
    *   Determine the GitLab remote URL.
    *   Identify the current branch.
    *   Construct the appropriate URL to the file or directory in GitLab.
    *   Open the URL in your default web browser.

If the script cannot open the URL in your browser, it will print the URL to the console.

## Examples

1.  To open the root directory of your repository:

    ```bash
    cd /path/to/your/repo
    gitlab
    ```

2.  To open a specific subdirectory:

    ```bash
    cd /path/to/your/repo/subdirectory
    gitlab
    ```

3.  To open a specific file:

    ```bash
    cd /path/to/your/repo/path/to
    gitlab
    ```

## Installation

1.  Save the script to a file named `gitlab` (or any name you prefer).
2.  Make the script executable:

    ```bash
    chmod +x gitlab
    ```

3.  Move the script to a directory in your `PATH` (e.g., `/usr/local/bin` or `~/bin`).  If you choose `~/bin`, ensure that `~/bin` is in your `PATH`.

    ```bash
    mv gitlab /usr/local/bin
    ```

    Or, for a user-specific installation:

    ```bash
    mkdir -p ~/bin
    mv gitlab ~/bin
    # Ensure ~/bin is in your PATH, e.g., by adding the following to your ~/.bashrc or ~/.zshrc:
    # export PATH="$HOME/bin:$PATH"
    ```

4.  Ensure the script is executable by typing `gitlab` in your terminal from within a git repository.
