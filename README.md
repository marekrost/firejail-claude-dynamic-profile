# Firejail Sandbox Wrapper for Claude Code

This script runs Claude Code in a sandboxed firejail environment with filesystem isolation while maintaining access to the current directory and Claude configuration.

The script dynamically detects the active Node.js environment and thus cannot be encapsulated into a static firejail profile file.

Select branch depending on your closest environment style:
- main ... self-locate node via npm, normal environment
- linuxbrew ... dev tools in linuxbrew - requires tweaks to firejail config

## Requirements

The following must be available in PATH:
- Firejail
- Claude Code
- Node.js / NPM

## Installation

Copy the `claude-sandbox` file from the `bin/` directory into any convenient folder in your PATH. Execute from inside the folder where you wish Claude to remain restricted.
