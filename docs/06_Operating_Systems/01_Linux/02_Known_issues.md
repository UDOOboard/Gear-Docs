<p style="background-color: rgba(255, 170, 50, 0.3);padding: 20px;border-left: 5px solid orange; border-radius: 4px; color:rgb(45, 45, 45);">
The reported known issue in this page is solved in newer versions of Ubuntu from 19.04 onwards
</p>

## amdgpu drivers issue in Ubuntu 18.04 - 'nomodeset' procedure

<span class="label label-info">Info!</span> Newer versions of Ubuntu than 18.04 are not affected by this issue so you don't need to use this procedure.

There is a *known issue* with **amdgpu driver** which comes with **Ubuntu 18.04 LTS** (and maybe others Linux distros). During and after OS installation it is possible that you may receive a UI after login or you may not.

You can find all the references about this issue in the amdgpu Documentation (amdgpu_UserGuide) in the driver packages downloadable from the AMD official website.
Check the [**Linux Drivers**](!Operating_Systems/Linux/Drivers) section to download the latest driver package.

If you experience this problem during the installation of Ubuntu 18.04 LTS (or in a different Linux distro) follow the instructions below or install a newer version of Ubuntu or the optimized version of Ubuntu 19.04 we've published in the start page of the [Linux section](!/Operating_Systems/Linux/index)

To workaround this issue you need to start the installation by adding `nomodeset` parameter to grub.

Adding `nomodeset` doesn’t load amdgpu driver which comes with Ubuntu 18.04 LTS and you will get the UI after login.

Procedure to add `nomodeset` to grub:
* Stop the installation to the grub menu.
* Press `e` to edit the menu entry you choose (e.g *Install Ubuntu*) and it will lead to edit the boot parameters.
* Find the line which ends with `quiet splash` and add `nomodeset` in front of it. So it becomes `nomodeset quiet splash`. Whatever is there in front of it leave it as it is just add `nomodeset` in front of `quiet splash`.
* Press Ctrl+X or F10 to boot with this new parameter.

You can check [this post](https://askubuntu.com/questions/38780/how-do-i-set-nomodeset-after-ive-already-installed-ubuntu/38782#38782) or [this other post](https://askubuntu.com/questions/1029624/ubuntu-18-04-live-boot-leads-to-blank-screen) to see an image that will let better understand where to put the `nomodeset` parameter.

Editing the grub like this is just a temporary fix, you probably will need to repeat the procedure after the installation to boot the system.  

After you've installed Ubuntu 18.04 LTS you can install the AMD drivers following the [Linux Drivers](!Operating_Systems/Linux/Drivers) section, to have a proper working system.

If you don't need the AMD drivers you can set the fix the `nomodeset` boot option permanently so that you don't have to go through this manual procedure again following the instructions in [this post](https://askubuntu.com/a/38782/88802).
