# Firejail Sandbox Wrapper for Claude Code

> **This repository is no longer maintained.** Claude Code is now distributed as a standalone binary and no longer requires a Node.js installation, so dynamic environment detection is unnecessary. Use the replacement repo with a static firejail profile instead: https://github.com/marekrost/firejail-claude-static-profile

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
