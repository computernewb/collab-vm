# CollabVM
This page contains details about CollabVM, what it is, the links to the source code, how to host it, the requirements for hosting it, and other things.

## What's CollabVM?

CollabVM is a website that allows users to take turns controlling virtual machines with strangers on the internet! You can access the flagship instance at [computernewb.com](https://computernewb.com/collab-vm/)

## Where is the source code?
CollabVM is fully open source and you can find the source code in the following repositories:

* [collabvm-1.2.ts](https://github.com/computernewb/collabvm-1.2.ts) - The backend server for CollabVM, written in TypeScript with some Rust modules. It handles pretty much all of the behind-the-scenes magic that makes CollabVM work.

* [collab-vm-1.2-web-app](https://github.com/computernewb/collab-vm-1.2-web-app) - This contains the source to the CollabVM webapp, which is the public frontend accessible on our website.

## Requirements for hosting
* The CollabVM Server is officially targeted to the latest releases of Debian and Arch Linux, and officially supports any modern Linux distro. While it technically can run on Windows, we do not support this.

* You should probably have at least 4-8 GB of RAM available.

* Your server should support hardware-assisted virtualization (KVM), or your VM will be very, very slow.

## FAQs

### If I make a fork of CollabVM Server/Webapp/etc, can it be closed source?
Under the terms of the GNU General Public License (which both the server and webapp are licensed under), you do not need to publish your changes to the source code unless you are distributing it in compiled form. If you are, you must release the source also licensed under the GPL. Also, if it contains bug fixes, really cool new features, or something else, we always appreciate the help!

### Can my CollabVM instance be private?
Your CollabVM instance may be private or public; it's up to you.

### Is there any risk to hosting this?
As with any server software that you open to the internet, there is always an inherent risk of vulnerabilities. While we try our very best to make the server as secure as possible, we strongly recommend running CollabVM as a depriviliged user with as few permissions as possible.

Also, if your VM is connected to the internet, anyone will be able to do anything from your IP address. We recommend putting your VM behind a VPN to prevent this.

### Is it possible to host Collab VM for my family / on my LAN?
Yes, although there is no official "LAN" mode for Collab VM, just keep the port closed to the internet and it will effectively achieve the same thing.
