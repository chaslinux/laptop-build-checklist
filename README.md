# laptop-build-checklist
Computer Recycling checklist for refurbishing laptops with Linux Mint.

This is a LibreOffice Writer document that includes most of the steps the Computer Recycling Project @ The Working Centre uses to refurbish laptops with Linux Mint XFCE. 

Note: We use a custom PXE network server for our installs, but purposefully chose not to automate on the server the process beyond the PXE live installation. By using 
a post-install BASH script stored on github we encourage others (both within and outside our organization) to participate/add/improve some of our processes.

The mint-setup.sh script mentioned in this checklist is a BASH script that pulls several other BASH scripts with the following functions:
* hardware.sh - installs LaTeX support and software to query the hardware the script is being run on. A PDF with the specs of this hardware appears on the desktop. The PDF
  includes a barcode to make it easier to add hardware to a Point-Of-Sale system.
* mint-extras.sh - installs extra software we think helps make Linux Mint more usable for the average computer user. Also installs tlp to help manage laptop thermals.
* geekbench-dl - downloads geekbench6, a standard CPU benchmark, and runs the benchmark
* pts - downloads and installs phoronix-test-suite, then runs the game OpenArena at 1024x768 high settings. Since laptops vary in screen resolutions we chose this smaller
  resolution as a base.

This script and several others related to refurbishing are publically available on github via https://github.com/chaslinux


