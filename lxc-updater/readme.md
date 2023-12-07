This file is used to update specific LXC's in your environemnt and create a new template from them.

In my specific instance, I have some LXC's that i use as the base image template for creating future LXC's. I always want these LXC's kept up to date with the base packages etc.. So I created this script.

To use, edit the list of LXC id's at the top, and thats it. Its basic operation is
- Get the name of the LXC
- update the LXC (apt update)
- upgrade the packages (apt upgrade)
- remove un-needed packages (apt auto remove)
- Create a new template overiding the existing one using the name.

To automate this process, I put it in the /etc/cron.daily folder. This executes automatically at ~6AM daily (give or take)


![image](https://github.com/jbates58/proxmox_scripts/assets/7126355/e8fa3e9c-894e-42cc-9ed9-974266f2086d)

![image](https://github.com/jbates58/proxmox_scripts/assets/7126355/475e30e0-1ed9-4007-8eb4-0afe649815dd)

