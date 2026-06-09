# Ethne workstation enrollment

## Install tailscale vpn

1. Download windows client from https://login.tailscale.com/admin/machines
2. Click Add device
3. Navigate to <https://tailscale.com/download/windows>
4. Click `Download Tailscale for Windows` to download
5. Run download
6. Sign in to your network via credentials
7. Enable unattended access
    * Right-click Tailscale icon in task
    * Select `Preferences` -> `Run unattended`

## Install saltstack minion

1. Download saltstack minion
    * https://docs.saltproject.io/salt/install-guide/en/latest/topics/install-by-operating-system/windows.html#major-one-version-text-downloads
    * [Download latest 3006 version (v3006.26 currently) for AMD64, MSI](https://packages.broadcom.com/artifactory/saltproject-generic/windows/3006.25/Salt-Minion-3006.25-Py3-AMD64.msi)
2. Open Powershell as Administrator
    * Search powershell in start bar
    * Click `Run as Administrator`
    * `cd ~\Downloads`


