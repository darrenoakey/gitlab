# GitLab Opener

[![Banner Image](banner.jpg)](banner.jpg)

## Purpose

This script simplifies opening your GitLab repository in your web browser directly from your terminal. It automatically determines the correct URL based on your current Git repository's remote origin and current working directory.

## Usage

Navigate to your Git repository in the terminal. Then, execute the script. It will open the GitLab repository in your default web browser.

## Installation

1.  Save the script to a file named `gitlab` (or any name you prefer).
2.  Make the script executable: `chmod +x gitlab`.
3.  Move the script to a directory in your `$PATH` (e.g., `/usr/local/bin`): `sudo mv gitlab /usr/local/bin`.

## Examples

1.  **Open the repository in the browser:**

    ```bash
    gitlab
    ```
    This will open the GitLab repository's root directory in your browser, reflecting the current branch.

2.  **Open a specific file:**

    ```bash
    gitlab path/to/your/file.txt
    ```
    This will open the specified file as a blob in your browser on GitLab, showing the file's content for the current branch. The path is relative to the git repository root.

3. **Open a file using absolute path:**
    ```bash
    gitlab /absolute/path/to/your/file.txt
    ```
    This will open the specified file as a blob in your browser on GitLab, showing the file's content for the current branch. 

## Requirements

*   Git must be installed.
*   The script must be executed within a Git repository.
*   The Git repository must have a remote named 'origin' pointing to a GitLab repository.
