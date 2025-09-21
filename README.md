# Kernel for Samsung Galaxy S24 Snapdragon Series

This is a high-performance custom kernel for the **Samsung Galaxy S24 Snapdragon Series**, built upon Samsung's official kernel source. It is designed to deliver exceptional stability and smoothness while integrating the latest KernelSU features for the ultimate user experience.

## 📌 Highlights

* **Official Source Base**: Built on the latest official kernel source from Samsung, ensuring optimal compatibility and stability.

* **Performance-Tuned**: Targeted performance and scheduling optimizations for a smoother daily usage and gaming experience.

* **KernelSU Integrated**: Comes with multiple KernelSU variants (Official, MKSU, SukiSU-Ultra) built-in for an out-of-the-box experience.

## 🧩 Available Variants Explained

* **LKM (Loadable Kernel Module)**

  * Does not include any built-in root solution, maintaining the purity of the stock kernel.

  * **Security**: Only essential Samsung security policies that affect modding (like RKP, KDP) are removed.

  * **Usage**: Requires you to manually patch your device's `init_boot` partition using the KernelSU Manager App to achieve root.

* **KSU (KernelSU)**

  * Built-in with the official, unmodified KernelSU for the most authentic root experience.

* **MKSU (Magic KernelSU)**

  * Features KernelSU modified by `5ec1cff`, which notably supports Magic Mount for easier module management.

* **SukiSUU (SukiSU-Ultra)**

  * Integrated with the powerful SukiSU-Ultra, supporting SUSFS and KPM modules, offering advanced features for power users.

## ⚙️ Installation Guide

1. **Unlock Bootloader**: Ensure your device's bootloader is unlocked.

2. **Flash Recovery**: It is recommended to use the latest version of TWRP or OrangeFox Recovery.

3. **Flash Kernel**: Flash the kernel `zip` package downloaded from the Releases page in this project via Recovery.

4. **(LKM Version Only) Patch `init_boot`**:

   * Back up your current `init_boot.img`.

   * Use the KernelSU Manager App to select and patch this image.

   * Flash the resulting `kernelsu_boot.img` to your device's `init_boot` partition via Fastboot or Recovery.

5. **Reboot your device** and enjoy the new kernel!
