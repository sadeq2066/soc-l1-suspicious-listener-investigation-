# Findings

A suspicious TCP listener was discovered on port 4444.

The listener was identified using:
- ss -tulnp
- netstat -tulnp

The process responsible was identified as netcat (`nc`).

The listener was active on all interfaces:
0.0.0.0:4444

This could allow remote inbound connections and unauthorized shell access.
