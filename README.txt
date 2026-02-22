TBLINC: Unified OpenStack Deployment CLI
=========================================

TBLINC (Tunnel, Build, License, Install, Network, Container) is a professional 
orchestrator for Kolla-Ansible OpenStack deployments. It automates the setup 
of Stable 2025.2 OpenStack environments on Ubuntu servers.

--- DIRECT INSTALLATION ---

Copy and paste this command to install TBLINC system-wide immediately:

 wget -qO tblinc_v4.deb "https://github.com/tblinc810/tblinc/raw/main/tblinc_v4.deb" &&
 sudo apt install ./tblinc_v4.deb -y && rm tblinc_v4.deb

--- LOCAL INSTALLATION ---

If you have downloaded the .deb file manually:

    sudo dpkg -i tblinc_v4.deb

--- QUICK START ---

After installation, run:

    tblinc install

--- CORE COMMANDS ---

- tblinc install   : Fully automate the OpenStack 2025.2 deployment.
- tblinc status    : Check the health of all system components.
- tblinc tunnel    : Setup/Manage Cloudflare Tunnels for Horizon dashboard.
- tblinc remove    : Safely uninstall and purge all OpenStack data.

--- MODULAR COMMANDS ---

- tblinc network   : Manual control for networking and sysctl optimizations.
- tblinc docker    : Manual control for Docker engine & Kolla optimizations.
- tblinc license   : View the deployment license documentation.

--- SCRIPTS OVERVIEW ---

1. deployment.sh : The master engine for Kolla-Ansible automation.
2. network.sh    : Handles kernel optimizations and dummy interfaces.
3. docker.sh     : Installs and optimizes Docker for OpenStack.
4. tunnel.sh     : Exposes private Horizon Dashboard to a public domain.

=========================================
GitHub: https://github.com/tblinc810/tblinc
