# Raspberrypi pihole

Run pihole as docker: 

We need to download network manager because rapberrypi doesnt have it.
- https://raspberrypi.stackexchange.com/questions/29783/how-to-setup-network-manager-on-raspbian  

Also turn off dns service that runs or port .53
- `sudo systemctl disable systemd-resolved.service`
- `sudo systemctl stop systemd-resolved.service`

Then follow this:
- https://www.smarthomebeginner.com/run-pihole-in-docker-on-ubuntu-with-reverse-proxy/
  - go to: **Step 2b: PiHole on Docker without Reverse Proxy**


sudo docker-compose -f ./docker-compose.yml up -d ; docker-compose logs -tf --tail="50" pihole