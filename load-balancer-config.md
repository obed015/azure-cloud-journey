# Azure Load Balancer Config

## Key Steps:
1. Created Public IP (Static, Standard SKU)
2. Created Load Balancer (HA-Web-LB)
3. Backend Pool: WebVM1 & WebVM2
4. Health Probe: HTTP on port 80
5. Load Balancing Rule: TCP 80 → Backend Port 80

## Validation:
- Accessed HA-LB public IP → NGINX page loads
- Stopped VM1 to simulate failure → traffic routed to VM2
- Restarted VM1 → traffic rebalanced
