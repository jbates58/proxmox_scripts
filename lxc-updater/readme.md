This file is used to update specific LXC's in your environemnt and create a new template from them.

In my specific instance, I have some LXC's that i use as the base image template for creating future LXC's. I always want these LXC's kept up to date with the base packages etc.. So i created this script.

To use, edit the list of LXC id's at the top, and thats it. Its basic operation is
- Get the name of the LXC
- update the LXC (apt update)
- upgrade the packages (apt upgrade)
- remove un-needed packages (apt auto remove)
- Create a new template overiding the existing one using the name.

