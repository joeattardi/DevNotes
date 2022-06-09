# Launch a new process with debugger
```bash
node --inspect-brk /path/to/script
```

Debugger will be listening on port 9229.

## Inspect options
- `--inspect` - Starts process immediately and listens on port 9229
- `--inspect-brk` - Starts process but pauses until debugger is attached

# Attach to a running process

[Stack Overflow thread](https://stackoverflow.com/questions/13052548/node-js-how-to-attach-to-a-running-process-and-to-debug-the-server-with-a-conso)

- Find the process ID:
```bash
pgrep node
```

- Send the `USR1` signal to the process:
```bash
kill -USR1 <node_pid>
```

- Open Chrome and go to chrome://inspect
- There should now be a link to connect to/inspect the running node process

# Resources
[Node.js Debugging](https://nodejs.org/en/docs/guides/debugging-getting-started/)

#nodejs