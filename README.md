 SOC L1 Suspicious Listener Investigation

 Objective
Investigate a suspicious TCP listener running on port 4444 on a Linux host.

Tools Used
- ss
- netstat
- ps
- tree
- nano

 Investigation Summary
A suspicious listener was identified on TCP port 4444 using Linux monitoring tools.
The process was linked to netcat (nc), which could allow unauthorized remote access.

 Key Findings
- Port 4444 listening on all interfaces
- Associated process identified
- Medium security risk
- Potential unauthorized remote shell access

 Skills Demonstrated
- Linux command line
- Incident investigation
- Process analysis
- Port analysis
- Documentation
- Basic remediation planning
