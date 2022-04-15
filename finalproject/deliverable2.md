### What is Virtualization?

  *    Virtualization is running a computer inside another computer, but with a difference. The computer running in the virtual machine has a low risk of damage or loss if you break it. A virtual machine can also make it instantly without the worry of getting stolen on the internet because virtual machines are always used for general purposes in case of loss. So you only delete it and create a new one. Furthermore, a virtual machine can store it in remote sources like servers that are computers. The main reason to exist is only to save and store data of any network or user worldwide.

![Virtualization](Virtualization.jpg)

### Types of virtualization



* **Client-side Virtualization** IS a Virtual machine, but with the differences that are the focus in use with users only with applications. For example, suppose you use your phone daily, and that phone uses an application, you. In that case, the regular user doesn't have access to the server. Instead, you have access to the server, a computer that stores information on the net, to access an application. So your phone as a cloud gaming app like Nvidia cloud or Xbox cloud from your phone, and use the resources. From the server using the app like memory ram, etc. but can't modify what is shown to you. You can't install anything or use anything that the server owner does not predetermine.
  
  ![client-side](client-Side.png)
  
*  **Server-side Virtualization** IS the technique of transforming one powerful computer into a machine that stores data and use it from just one device to avoid the excess power consumption and hardware overcrowding do it, but the excessive amount of racks or spaces that need for this task also is not the best idea since server virtualization tends to use the hardware or physical components of a machine and share with all the others virtual servers going to be overwhelming at some point still have many advantages since you can use as regular Server and modified as much as you need it 

![Serverside](Serverside.png)

### Hypervisor 

* Hypervisor is software that creates also manages virtual machines (Vms). The hypervisor allows a computer to run multiple virtual computers using the same resources as the host computer. Also, these VMS acts as independent computers or servers that control apps as a regular computer does. Hypervisors also use the same memory and configuration from the shot. Still, they can be variable, not the same as the host since it can use the hypervisor to do specific tasks. Such as turning on a machine that makes products or cars or even an ATM that typically uses hypervisors.

### Types of hypervisors

## Virtual Manager

* Virtual Manager or virtual-manager is a graphical front-end hypervisor that supports different types of virtualization such as Qemu, Zen, and Xen used in Linux and Windows. Its primary purpose is to virtualize a virtual machine making it. It is easy to use without going into the terminal using a graphical interface that makes the user install it and manage it easily.
  
![Virtual-Manager](virtManager_logo.webp)

## Installing Endeavour os  in Virtual  Manager

* Installing Endeavour os is a process that takes several steps First one is installing and configure Libvirt and Qemu. 

* 1. Installing all the packages to run virt-manager.

Basic install:

```sudo pacman -S virt-manager libvirt qemu```

Full-featured install:

```sudo pacman -S --needed virt-manager qemu libvirt edk2-ovmf dnsmasq vde2 bridge-utils openbsd-netcat iptables-nft dmidecode```


2. After installation completes you need to enable libvirtd service.

```sudo systemctl enable --now libvirtd.service```

3. Check for the status to make sure the service is running.

```systemctl status libvirtd.service```

The output should look something like below.

○ libvirtd. service - Virtualization daemon
     Loaded: loaded (/usr/lib/systemd/system/libvirtd.service; enabled; vendor preset: disabled)
     Active: inactive (dead) since Tue 2021-08-31 20:33:58 +0530; 1h 14min ago
TriggeredBy: ● libvirtd-admin.socket
             ● libvirtd-ro.socket
             ● libvirtd.socket
       Docs: man:libvirtd(8)
             https://libvirt.org
    Process: 21412 ExecStart=/usr/bin/libvirtd $LIBVIRTD_ARGS (code=exited, status=0/SUCCESS)
   Main PID: 21412 (code=exited, status=0/SUCCESS)
      Tasks: 2 (limit: 32768)
     Memory: 18.5M
        CPU: 423ms
     CGroup: /system.slice/libvirtd.service
             ├─982 /usr/bin/dnsmasq --conf-file=/var/lib/libvirt/dnsmasq/default.conf --leasefile-ro --dhcp-script=/usr/lib/libvirt/libvirt_leaseshelper
             └─983 /usr/bin/dnsmasq --conf-file=/var/lib/libvirt/dnsmasq/default.conf --leasefile-ro --dhcp-script=/usr/lib/libvirt/libvirt_leaseshelper
To use our normal user without entering the root password we need to configure KVM to enable it. This will also enable the libvirt networking components as well without doing this it won’t work.
You need to open the libvirt configuration file located at /etc/libvirt/libvirtd.conf. To open you can use your favorite text editor (vi, vim, or nano).
sudo nano /etc/libvirt/libvirtd.conf
Now we need to set UNIX domain socket ownership to libvirt. Scroll down till you see the below line and uncomment it.
unix_sock_group = 'libvirt'
Let’s set the UNIX socket permission to R/W. Scroll down till you see the below line and uncomment it.
unix_sock_rw_perms = '0770'
Add your user account to the libvirt group.
sudo usermod -a -G libvirt $(whoami) or sudo usermod -a -G libvirt (your user name)
– `whoami` is a function that put the current user name in the placeholder
Now we need to add our user to `qemu.conf`. Otherwise, QEMU will give a `permission denied` error when trying to access local drives. You can use your favourite text editor to edit the file.
sudo nano /etc/libvirt/qemu.conf
Scroll down or search for `user = “root”` or `group = “root”`. Then uncomment both entries and change the root to your user name or ID and then save and exit. Once edited it should look something like below.

4. You could restart your service, but it’s best to reboot the entire system.

```sudo shutdown -r now```



Network:
If Network is disabled after rebooting the host machine and you do not find a way to enable it, you can have it enabled per default from the command line. This will work after rebooting the host:

```sudo virsh net-autostart default```


5. after this you need to Download the iso file from endeavour page and start the installation as regularly you do in a virtual machine 

![How-to-Install-Endeavour-os](How-to-install-Endeavouros-In-Virtual-Manager.png)

Link in the source Down Below

### Updating Endeavour os 


### Installing Software in Endeavour os

* Installation command examples
* Searching for software
* Deleting software

### Basic linux Commands
Nothing here remember it 

### Navigating the filesystem

### Managing files and directories

#### Mkdir

* Description:
* Usage:
* Examples
  

### Sources

* Endeavour os Wiki: https://discovery.endeavouros.com/applications/how-to-install-virt-manager-complete-edition/2021/09/

* Virtualization Basics: https://www.cnblogs.com/popsuper1982/p/3800230.html

* computer hope: https://www.computerhope.com/jargon/s/server-side-scripting.htm

* How to install Endeavour os : https://youtu.be/N1kfFkSKCOw

* Hypervisor : https://www.serverwatch.com/virtualization/hypervisor-server/