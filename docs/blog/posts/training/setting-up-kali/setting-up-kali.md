---
date: 2023-09-11
categories:
  - Training
authors:
  - silk
slug: setting-up-kali
---

# Setting up your Kali Linux VM

Let's get started setting up your Kali Linux virtual machine.

## Why?

Kali Linux is a distribution of Linux that comes with many valuable tools for ethical hacking.

![Kali Linux](./images/kali-dragon-icon.svg){style="width: 50%; margin:0 35% 0 15%; display: block;"}

<!-- more -->

## What is a VM?

A virtual machine (VM) is a virtual computer running inside your computer. We use virtual machines for a couple of reasons:

1. To use a different operating system than is on our computer. For example, many tools we need to use are available on Linux, but many of us use Windows or Mac.
2. To protect ourselves. Sometimes, we may be running code which we are not 100% sure is safe. Keep your personal information safe by running it in a VM.

## What software run VMs?

Virtual machines are run using virtualization software. There are two free-to-use products you can choose from:

1. VirtualBox. Open-source and free. [Downloads available here](https://www.virtualbox.org/wiki/Downloads).
2. VMware Workstation Player. Not open-source, but free for personal, non-commercial use. [Downloads available here](https://www.vmware.com/ca/products/workstation-player.html).

You may choose either software to install. Both options are practically equivalent regarding features, and the difference is opinion-based.

![VM Software](./images/vmsoftware.png){style="width: 50%; margin: auto; display: block;"}

Choose the next section based on which software you decided to install.

### Installing VirtualBox

![VirtualBox](./images/virtualbox.png){ width=50% }

First, [download VirtualBox from here](https://www.virtualbox.org/wiki/Downloads).

Open the installer file.

![Installing VirtualBox 0](./images/installing-virtualbox-0.png)

Click **Next**.

![Installing VirtualBox 1](./images/installing-virtualbox-1.png)

Leave the feature selection as default. Click **Next**.

![Installing VirtualBox 2](./images/installing-virtualbox-2.png)

Click **Yes**.

![Installing VirtualBox 3](./images/installing-virtualbox-3.png)

Click **Install**.

![Installing VirtualBox 4](./images/installing-virtualbox-4.png)

Wait for the installation to complete.

![Installing VirtualBox 5](./images/installing-virtualbox-5.png)

The installation is done, you can click **Finish**.

![Installing VirtualBox 6](./images/installing-virtualbox-6.png)

Now you can launch VirtualBox from the desktop or start menu.

![Installing VirtualBox 7](./images/installing-virtualbox-7.png)

### Installing VMware

![VMware Workstation Player](./images/vmware.png)

First, [download VMware Workstation Player from here](https://www.vmware.com/ca/products/workstation-player.html).

Open the installer file.

![Installing VMware 0](./images/installing-vmware-0.png)

Click **Next**.

![Installing VMware 1](./images/installing-vmware-1.png)

~~Read the EULA~~ and click accept. Then click **Next**.
m
![Installing VMware 2](./images/installing-vmware-2.png)

Check **Install Windows Hypervisor Platform (WHP) automatically**. Click **Next**.

![Installing VMware 3](./images/installing-vmware-3.png)

Click **Next**.

![Installing VMware 4](./images/installing-vmware-4.png)

Uncheck **Join the VMware Customer Experience Improvement Program** if you want to. Click **Next**.

![Installing VMware 5](./images/installing-vmware-5.png)

Click **Next**.

![Installing VMware 6](./images/installing-vmware-6.png)

Click **Install**.

![Installing VMware 7](./images/installing-vmware-7.png)

Wait for VMware to finish installing.

![Installing VMware 8](./images/installing-vmware-8.png)

The installation is done, you can click **Finish**.

![Installing VMware 9](./images/installing-vmware-9.png)

Now you can launch VMware from the desktop or start menu. If prompted, select the non-commercial option.

![Installing Vmware 10](./images/installing-vmware-10.png)

## How do I get a Kali Linux VM?

You can download pre-built Kali virtual machines from the Kali Linux website. [Download the VM matching your chosen software (VMware or VirtualBox).](https://www.kali.org/get-kali/#kali-virtual-machines)

![Download Kali Linux](./images/download-vms.png)

## How do I install a Kali Linux VM?

Extract the downloaded archive to a folder you will remember. Common virtual machine folders are:

- `C:\Users\[username]\VirtualBox VMs`
- `C:\Users\[username]\Documents\Virtual Machines`
- `C:\VirtualBox VMs`

![Extracting Kali Linux](./images/extracting-vm.png)

After you have extracted the virtual machine, you must open it.

If you are using VirtualBox, simply double-click the `kali-linux-...-virtualbox-amd64.vbox` file.

If you are using VMware:

1. Open VMware.
2. Click **Open a Virtual Machine**.
3. Navigate to the folder where you extracted the VM.
4. Select the `kali-linux-...-vmware-amd64.vmx` file.
5. Click **Open**.

After you have opened the file once, you can simply launch the VM from the VM software going forward.

![Installing Kali Linux](./images/installing-vm.png)

You may wish to increase the amount of RAM and CPU threads allocated to the VM to improve its performance.

Simply right click on your virtual machine and click **Settings**.

![VirtualBox Settings Right Click](./images/virtualbox-settings-right-click.png)

![VirtualBox Settings](./images/virtualbox-settings.png)

![VMware Settings Right Click](./images/vmware-settings-right-click.png)

![VMware Settings](./images/vmware-settings.png)

Now your VM is installed and ready to be ran.

## How do I run a Kali Linux VM?

With your newly installed VM, click **Run** or **Start** in your preferred VM software.

**Note:** Once you click on your VM, it will capture your keyboard and mouse. To get out of the VM, click:

- **Right Ctrl** if using VirtualBox.
- **Ctrl + Alt** if using VMware.

![VM Starting](./images/vm-starting.png)

When met with the login screen, the default username and password are both `kali`.

![VM Login](./images/vm-login.png)

One final recommendation is to install the package `kali-linux-large`, which contains many useful tools. You can install the package by opening a terminal and running the following commands:

1. `sudo apt update`
2. `sudo apt -y install kali-linux-large`

When prompted, enter the password in the terminal.

![Kali Terminal](./images/kali-terminal.png)

![Kali Installing kali-linux-large](./images/kali-installing-large.png)

## What now?

Feel free to explore the operating system and tools within it. Plenty of free materials on the internet can help guide you. We plan to post more club training materials soon. We will also be using Kali extensively in our club meetings.

Happy Hacking!
