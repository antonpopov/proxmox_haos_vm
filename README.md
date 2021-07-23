# Proxmox (6 & 7) VM with Home Assistant OS

To create a new Proxmox VM with the latest version of Home Assistant OS, run the following from Proxmox web shell

```
bash -c "$(wget -qLO - https://github.com/tteck/proxmox_haos_vm/raw/master/install.sh)"
```

After script completes, click on the new VM, click on the `Hardware` tab for the VM and change the `Memory` and `Processors` settings to what you desire. The network MAC address can be changed by selecting `Network Device` and clicking `Edit` above. Once all changes have been made, click `Start` above.

## Root Prompt

To get to the root prompt
- Open the console after the VM has been started
- When the messages slow down press the `Enter` key a couple of times until you see the following
```

Welcome to Home Assistant
homeassistant login:
```
- Login using `root`, no password is requested
- When you see the `hassio > ` prompt, type `login`
- You should now see a `# ` prompt.
