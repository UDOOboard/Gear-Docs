At the following link you can find the latest BIOS/UEFI Firmware and the BIOS/UEFI Update Utility to quickly and easily update the UDOO BOLT with the new BIOS/UEFI Firmware version.

<span class="label label-warning">Heads up!</span> Please read carefully all the following information in this page and in the documentation file inside the package before to flash the new BIOS/UEFI

Please be aware that using **Windows** programmer, it must be run in a Prompt CMD shell with Administrator privileges.

Using **Linux** programmer, *gcc compiler* and *Kernel-headers* are needed and every operation must be done with root/administrator privileges.  

<ul style="background-color: rgba(255, 170, 50, 0.3);padding: 20px;border-left: 5px solid orange; border-radius: 4px; color:rgb(45, 45, 45);">
  <li>DO NOT POWER OFF the board while flashing. DO NOT interrupt the process while is running.</li>
  <li>Please use <strong>19V Power Supply</strong>, not the USB-C power.</li>
  <li>After flashing is complete, power off the board, <strong>disconnect and reconnect the power cable</strong>.</li>
  <li>When you reconnect the power, wait <strong>up to 3 minutes and a couple of reboots</strong> until you see the newer version of the firmware of Embedded Controller and USB-C Controller in the configuration screen.</li>
  <li>It takes a few restarts for the update to be completely installed, and there's no visual feedback on that yet. In the meantime, the system and the boot phase might be slower.</li>
</ul>

Download here the [UEFI BIOS Firmware + Update Utility Tool]() package.

The package contains:
* Latest UEFI Firmware binary
  * BIOS version:  1.07
  * Release Date:  19/03/2020
  * SHA1 .zip file:  
* Update Utility Tool
  * EFI shell programming utility
  * Windows 32-bit BIOS programmer
  * Windows 64-bit BIOS programmer
  * Linux 32-bit programmer
  * Linux 64-bit programmer
* Update procedure documentation (.pdf)

Follow the procedure in the `APN - BIOS programming using AFU.pdf` file to update the BIOS/UEFI BIOS firmware using Windows, EFI shell or Linux running on your UDOO BOLT.

<span class="label label-info">Note</span> Remember that updating the BIOS/UEFI firmware will revert the saved configuration to Factory Default.