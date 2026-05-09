# Incident Report

## Incident Summary
A suspicious TCP listener was identified on port 4444 during a Linux-based investigation lab.

## Investigation Details
The listener was detected using:
- ss -tulnp
- netstat -tulnp

The associated process was identified using:
- ps -fp 5147
The process was confirmed to be a netcat (`nc`) listener running on port 4444.

## Findings
- Port 4444 was actively listening
- Listener was exposed on all interfaces (0.0.0.0)
- Netcat can be associated with reverse shells and unauthorized remote access

## Severity
Medium

## Evidence Collected
- ss_tulnp_output.txt
- netstat_output.txt
- ps_process_output.txt

## Remediation Actions
- Stop unauthorized listener processes
- Restrict inbound access using firewall rules
- Monitor listening ports regularly
- Review logs for suspicious activity

## Outcome
The listener was identified, documented, and remediation recommendations were provided as part of the SOC investigation workflow.
