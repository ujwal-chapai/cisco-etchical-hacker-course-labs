# Lab: Deploy a Pre-Built Kali Linux Virtual Machine (VM)

## Course
Cisco Ethical Hacker

## Objective
In this lab, I set up a pre-built Kali Linux virtual machine on my CachyOS system and practiced basic Linux commands, shortcuts, and privilege-related tasks inside the terminal.

---

## Setup on CachyOS

Since I use CachyOS, I followed the Intel/AMD path and installed VirtualBox using `pacman`.

First, I refreshed the package databases with:

```bash
sudo pacman -Syy
```

Then I installed VirtualBox and the required host modules with:

```bash
sudo pacman -S virtualbox virtualbox-host-dkms
```

After the installation finished, I opened VirtualBox and imported the pre-built Kali Linux `.ova` file provided for the course. Once the import was done, I started the VM and confirmed that Kali booted properly.

---

## Part 1: Deploying the Kali VM

After opening VirtualBox, I used the import appliance option and loaded the `.ova` file.

The VM was created successfully, and I was able to start it without major issues. This made the setup process much faster than installing Kali manually from scratch.

---

## Part 2: Exploring Linux

### Root Privileges

One of the first things I tested in the Kali terminal was the difference between normal user access and root access.

I first tried:

```bash
visudo
```

This returned a permission denied message, which made sense because editing the sudoers file requires administrative privileges.

After that, I used:

```bash
sudo visudo
```

This worked after entering the password `kali`. That showed how `sudo` temporarily gives root privileges for a single command.

To confirm that the `kali` user was part of the sudo group, I ran:

```bash
grep sudo /etc/group
```

The output showed:

```bash
sudo:x:27:kali
```

That confirmed the `kali` user had sudo access.

---

### Keyboard Shortcuts and Command History

This part of the lab was useful because it showed how much easier the terminal becomes once you know a few shortcuts.

Using the **up arrow** lets me move backward through previous commands, and the **down arrow** moves forward again.

I also checked my command history by running:

```bash
history
```

The output listed the commands I had used recently, including `visudo`, `sudo visudo`, `grep sudo /etc/group`, and `history`.

Then I tested command recall with:

```bash
!3
```

This repeated the third command from history, which was:

```bash
grep sudo /etc/group
```

I also tried:

```bash
!his
```

That expanded to:

```bash
history
```

These shortcuts are small, but they save time and make terminal use much smoother.

---

### Tab Completion

Another useful feature I practiced was tab completion.

When I typed:

```bash
hi
```

and pressed **Tab**, the system completed it to `history` once the command became unique.

I also tried:

```bash
ls /me
```

and pressed **Tab**, which completed it to:

```bash
ls /media
```

Then I pressed Enter to view the contents of the `/media` directory.

This made it clear that tab completion is very helpful when typing commands and file paths in Linux.

---

## Reflection

Using a pre-built Kali VM made the process much easier because I did not have to install the operating system manually. The image was already prepared, so I could focus on learning instead of spending time on setup.

On CachyOS, installing VirtualBox through `pacman` was straightforward, and importing the `.ova` file was also simple. Compared to using a full installer image, the pre-built VM saved time and reduced the chances of making setup mistakes.

For a lab like this, the pre-built image is the better option because it gets the environment ready quickly and lets me practice Linux and virtualization right away.

---

## Conclusion

This lab helped me understand how to run Kali Linux in a virtual machine on my CachyOS system and use some important Linux terminal features more comfortably. I practiced working with root privileges, checking command history, reusing commands, and using tab completion. These are basic but important skills for future cybersecurity and Linux work.
