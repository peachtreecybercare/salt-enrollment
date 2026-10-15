# Ethne workstation enrollment

## Install tailscale vpn

1. Download windows client from <https://login.tailscale.com/admin/machines> (`Sign in with GitHub`)
2. Navigate to <https://tailscale.com/download/windows>
3. Click `Download Tailscale for Windows` to download
4. Run download
5. Sign in to your network via credentials (Github -> 'ptcdevs')
  - `ptcdevs.org.github` -> `Connect`
6. Enable unattended access
  - Right-click Tailscale icon in task
  - Select `Preferences` -> `Run unattended`
7. On <https://console.tailscale.com/machines>
  - click 3-dots next to machine name
  - `Disable key expiry`

## Install saltstack minion

1. Download saltstack minion
    * <https://docs.saltproject.io/salt/install-guide/en/latest/topics/install-by-operating-system/windows.html#major-one-version-text-downloads>
    * [Download latest 3006 version (v3006.26 currently) for AMD64, MSI](https://packages.broadcom.com/artifactory/saltproject-generic/windows/3006.25/Salt-Minion-3006.25-Py3-AMD64.msi)
2. Open Powershell as Administrator
    * Search powershell in start bar
    * Click `Run as Administrator`
    * `cd ~\Downloads`
    * `./Salt-Minion-3006.29-Py3-AMD64.msi` (your file name may be different.  list files with `ls`)
    * master: `salt`
    * minion: same as hostname
      * run `hostname` from powershell
    * checkbox: `Remove configuration and cache: On uninstall`
    * Install
3. Accept salt minion key on salt server

