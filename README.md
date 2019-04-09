# Message Passing Analyzer

`mpa` - analyze message passing between arbitrary processes by monitoring IPC
calls.

## Usage

Analyzing short-lived client and long-lived server processes:

```
mpa -p "$(pidof server)" client [client-args ...]
```

Analyzing long-lived client and server processes:

```
mpa -p "$(pidof server)" -p "$(pidof client)"
```
