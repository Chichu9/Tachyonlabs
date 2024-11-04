---
description: VPS Setup Guide on Hetzner Cloud
---

# Hetzner VPS Setup & NoMachine RDP Guide

![Click on "\*\*New project\*\*"](<.gitbook/assets/0 (1) (1).png>)

![Click here](<.gitbook/assets/1 (1) (1).png>)

![Click on "\*\*Add project\*\*"](<.gitbook/assets/2 (1) (1).png>)

![Click on  Project you want to create a VPS in](<.gitbook/assets/3 (1) (1).png>)

![Click on "\*\*Create Resource\*\*"](<.gitbook/assets/4 (1) (1).png>)

![Click on "\*\*Servers\*\*"](<.gitbook/assets/5 (1) (1).png>)

![Select your preferred region "\*\*Ashburn, VA\*\*"](<.gitbook/assets/6 (1) (1).png>)

![Select OS](<.gitbook/assets/7 (1) (1).png>)

![Select Architecture](<.gitbook/assets/8 (1) (1).png>)

![Select VM Size](<.gitbook/assets/9 (1).png>)

![Uncheck IPV6](<.gitbook/assets/10 (1).png>)

![Select a Unique Name for your VPS](<.gitbook/assets/11 (1).png>)

![Click on "\*\*Create & Buy now\*\*"](<.gitbook/assets/12 (1).png>)

![After your VPS is created - Launch the VPS Using the Console Button](<.gitbook/assets/13 (1).png>)

![Login using the Root Username & Password Provided in Email -- It will prompt you to change the password on initial login.](<.gitbook/assets/14 (1).png>)

Optionally - You can install Ubuntu Desktop on your VPS using "sudo apt-get install ubuntu-desktop"

NoMachine to enable a better Remote Desktop solution to manage your VPS.

To install NoMachine, you need to download the `.deb` package from its [official website](https://downloads.nomachine.com/linux/?id=1). Considering the modern infrastructure of _Hetzner Cloud_, you probably need to download the `amd64` architecture. If you're not sure, you can use `dpkg --print-architecture` to get your architecture.

At the time of writing this tutorial, the latest version (8.8) of NoMachine can be downloaded with the following command:

```bash
wget https://download.nomachine.com/download/8.8/Linux/nomachine_8.8.1_1_amd64.deb
```

Then, install the `.deb` package:

```bash
sudo dpkg -i nomachine_8.8.1_1_amd64.deb
```

Finally, check out the [NoMachine download page](https://downloads.nomachine.com/), and install the NoMachine client based on your local device that will connect to the server. Run the NoMachine client in the local device, click the `Add` button, fill the host with your server's public IP address, and leave other parameters as default.

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Next, click the `Connect` button and enter your Ubuntu username (e.g., `root` as default) and password. If you've not set the password yet, you can simply do it interactively with `passwd` command.

Link for More Advanced Instructions for NoMachine [https://kb.nomachine.com/DT07S00245](https://kb.nomachine.com/DT07S00245)
