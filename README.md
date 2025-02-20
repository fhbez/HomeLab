# HomeLab

Setup Proxmox on Hosts

Create VMS:

Ubuntu CT Templates

Kasm Workspaces
https://kasmweb.com/docs/latest/install/single_server_install.html
cd /tmp
curl -O https://kasm-static-content.s3.amazonaws.com/kasm_release_1.16.1.98d6fa.tar.gz
tar -xf kasm_release_1.16.1.98d6fa.tar.gz
sudo bash kasm_release/install.sh

Containers
sudo apt update
sudo apt upgrade
sudo apt install docker.io
docker volume create portainer_data
docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:lts

Home Assistant OS from Proxmox VE Helper Scripts
https://community-scripts.github.io/ProxmoxVE/
bash -c "$(wget -qLO - https://github.com/community-scripts/ProxmoxVE/raw/main/vm/haos-vm.sh)"
Restore from Gdrive Backup

Media
Network
