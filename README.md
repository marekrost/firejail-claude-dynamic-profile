# Firejail sandbox wrapper for Claude Code

This is a simple attempt to isolate Claude code from the rest of the filesystem without the need to trust it's own policing tools.

The script expects dynamic Node.js install location in order to function with tools like NVM (Node Version Manager) and thus the function cannot be encapuslated into a static firejail .profile file.

## Installation

Simply copy the file claude-sandbox into your PATH and execute.
