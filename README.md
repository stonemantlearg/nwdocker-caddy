# nwdocker-caddy handy commands


# Caddy Installation
sudo apt install -y debian-keyring debian-archive-keyring apt-transport-https<br>
curl -1sLf 'https://dl.cloudsmith.io/public/caddy/stable/gpg.key' | sudo gpg --dearmor -o /usr/share/keyrings/caddy-stable-archive-keyring.gpg<br>
curl -1sLf 'https://dl.cloudsmith.io/public/caddy/stable/debian.deb.txt' | sudo tee /etc/apt/sources.list.d/caddy-stable.list<br>
sudo apt update<br>
sudo apt install caddy<br>

# Caddy Format & Config
First: caddy stop<br>
caddy fmt -overwrite /path/to/caddyfile<br>
caddy adapt -config /path/to/caddyfile<br>
caddy run<br>
