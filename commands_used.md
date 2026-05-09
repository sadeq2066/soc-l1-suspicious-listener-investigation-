# Commands Used

## Create suspicious listener
nc -lvp 4444

## Check listening ports
ss -tulnp

## Filter for port 4444
ss -tulnp | grep 4444

## Verify using netstat
netstat -tulnp | grep 4444

## Identify process by PID
ps -fp 5147

## Save investigation evidence
ss -tulnp | grep 4444 > evidence/ss_tulnp_output.txt

netstat -tulnp | grep 4444 > evidence/netstat_output.txt

ps -fp 5147 > evidence/ps_process_output.txt

## Check firewall status
sudo ufw status verbose

## Block inbound port
sudo ufw deny 4444

## Display project structure
tree
