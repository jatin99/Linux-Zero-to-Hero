# Linux System Administration: User Management

## Introduction
User management is a crucial aspect of system administration in Linux, involving tasks such as creating, modifying, and deleting user accounts, as well as managing their permissions and access levels. This document provides detailed study notes for key user management commands.

## Commands

### useradd
This command is used to add a new user to the system.

**Syntax:**
useradd [options] username


- Options:
  - `-c, --comment`: Add a comment to the user account (usually the user's full name).
  - `-d, --home HOME_DIR`: Specify the home directory for the new user.
  - `-g, --gid GROUP`: Specify the primary group for the new user.
  - `-s, --shell SHELL`: Specify the login shell for the new user.
  - `-m, --create-home`: Create the user's home directory if it doesn't exist.
  - `-u, --uid UID`: Specify the user ID for the new user.

**Example:**
useradd -m -s /bin/bash john


### userdel
This command is used to delete a user account from the system.

**Syntax:**
userdel [options] username


- Options:
  - `-r, --remove`: Remove the user's home directory and mail spool.

**Example:**
userdel -r john


### passwd
This command is used to change the password for a user account.

**Syntax:**
passwd [username]


- If no username is specified, it changes the password for the current user.
- If a username is provided, it changes the password for that specific user (requires root privileges).

**Example:**
passwd john


### usermod
This command is used to modify user account properties.

**Syntax:**
usermod [options] username


- Options:
  - `-c, --comment COMMENT`: Add or modify the comment (usually the user's full name).
  - `-d, --home HOME_DIR`: Change the user's home directory.
  - `-g, --gid GROUP`: Change the user's primary group.
  - `-s, --shell SHELL`: Change the user's login shell.
  - `-L, --lock`: Lock the user account.
  - `-U, --unlock`: Unlock the user account.

**Example:**

- Options:
  - `-c, --comment COMMENT`: Add or modify the comment (usually the user's full name).
  - `-d, --home HOME_DIR`: Change the user's home directory.
  - `-g, --gid GROUP`: Change the user's primary group.
  - `-s, --shell SHELL`: Change the user's login shell.
  - `-L, --lock`: Lock the user account.
  - `-U, --unlock`: Unlock the user account.

**Example:**
usermod -s /bin/zsh john


### su
This command is used to switch to another user account.

**Syntax:**
su [options] [username]


- If no username is provided, it switches to the root user.
- If a username is specified, it switches to that user (requires the user's password unless executed as root).

**Example:**
su mary


