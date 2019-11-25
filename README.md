# Raspberrypi pihole

Run pihole as docker: 

We need to download network manager because rapberrypi doesnt have it.
- https://raspberrypi.stackexchange.com/questions/29783/how-to-setup-network-manager-on-raspbian 

Then follow this:
- https://www.smarthomebeginner.com/run-pihole-in-docker-on-ubuntu-with-reverse-proxy/
  - go to: **Step 2b: PiHole on Docker without Reverse Proxy**


docker-compose -f ./docker/docker-compose.yml up -d ; docker-compose logs -tf --tail="50" pihole