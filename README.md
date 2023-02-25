EchOS is an operating system licensed under the gnu public v2.

About:
EchOS is designed to simulate DOS all over again.

Install:

Virtualbox:
You should see an ISO Called: EchOS.iso .
Where in order to run on virtualbox
you have to run this command:
VBoxManage convertfromraw --format VDI [filename].img [filename].vdi

[filename] - "EchOS.iso"
[filename(2)] - "EchOS.vdi"

qemu:

Running this in qemu is pretty straight forward!
qemu-system-x86_64 EchOS.iso -m 2000 (in the same directory)

-m 2000 (gives 2G's of memory. Without giving qemu some 
memory it can result in a kernel panic )

vmware:
Running this in vmware should be as simple as popping in the ISO.
However if this doesn't work you may have to convert to an VMDK.

Bare metal:
Pretty easy! Just burn the iso to an CD/USB
then go into bios and boot from the CD/USB.

Note: if you see a debian grub menu press enter.
EchOS is built on java and it uses debian as a 
base to startup the java virtual machine 
in order to run the bytecode.

Also if you don't see the CD/USB showing the boot options
make sure legacy boot is ticked on!

Native:

In case you don't have Java you can always use the bootable iso version.
However if you do have java then Native can work out!
The native version is exactly the same however instead of booting
into an entirely new OS you run this command to boot up the OS:

java -jar EchOS.jar (Jar file is located in the native folder)

Note: fullscreen for an full DOS Experience!

I hope you enjoy EchOS and updates are there on our offical github
page at least every month!
