# Recommendations
-Stop unauthorized listener processes, such as the netcat listener used in this lab, using `Ctrl + C` or by terminating the related PID.
- Restrict unnecessary inbound connections using firewall rules, such as `ufw`.
- Monitor listening ports regularly with `ss -tulnp` to identify unexpected services.
- Verify suspicious ports by mapping them to processes using `ps`.
- Review system and authentication logs for related suspicious activity.
- Maintain a baseline of approved services and open ports.
