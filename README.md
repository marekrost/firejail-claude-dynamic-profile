# Firejail Sandbox Wrapper for Claude Code

This script runs Claude Code in a sandboxed firejail environment with filesystem isolation while maintaining access to the current directory and Claude configuration.

The script dynamically detects the active Node.js environment to function with tools like NVM (Node Version Manager) and thus cannot be encapsulated into a static firejail profile file.

## Requirements

The following must be available in PATH:
- Firejail
- Claude Code
- Node.js / NPM

## Installation

Copy the `claude-sandbox` file from the `bin/` directory into your PATH and execute it from the folder where you wish Claude to remain restricted.
