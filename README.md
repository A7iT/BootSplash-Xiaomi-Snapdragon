# BootSplash-Xiaomi-Snapdragon

## Description
Custom BootSplash / BootLogo for Xiaomi devices running Snapdragon chipsets. Swap out that boring stock splash screen with something custom — make your phone boot up with style.

## ⚙️ Tech Stack
- No programming needed
- Pre-built `logo.img` files
- Flashable zips for recovery installs

## Features
- Replaces stock bootsplash with a custom image
- Simple fastboot or recovery-based installation
- Flashable zips provided for convenience
- No root required

## Requirements
- Xiaomi smartphone with a **Snapdragon** chipset
- **Unlocked bootloader** (mandatory)
- Optional: Custom recovery installed (TWRP, OrangeFox, PitchBlack)
- USB cable & platform-tools (for fastboot flashing)

## Installation

### Method 1: Fastboot (PC)
1. Go to the [Releases](../../releases) tab and download your desired **`...-logo.img`** file.  
   Each `...-logo.img` contains a different custom splash image — pick the one you like.
3. Reboot your device into **Fastboot mode**:
   - Power off your phone  
   - Hold **Volume Down + Power**
4. Connect the phone to your PC via USB.
5. On your PC, navigate to your **platform-tools** folder.
6. Open a terminal (or CMD) in that folder.
7. Run the following command:

```bash
fastboot flash logo <path-to-your-custom-logo.img>
```

> **Important:** Replace `<path-to-your-custom-logo.img>` with the actual path to the `.img` file you downloaded from Releases. Or you can just drag & drop the `.img` into the terminal window.

7. Wait for the flash to complete.
8. Type `fastboot reboot` or manually reboot the phone.
9. Enjoy your new custom splash screen.

---

### Method 2: Custom Recovery (Phone Only)
1. Download the desired **flashable ZIP** from the [Releases](../../releases) tab directly to your device.
2. Reboot into custom recovery (TWRP, OrangeFox, or PitchBlack).
3. Locate the ZIP file in your file browser within recovery.
4. Flash the ZIP.
5. Reboot your device.
6. Done — new bootlogo should be in place.

## Usage
This project is used to customize or completely replace the default boot splash image on Xiaomi devices with Snapdragon chipsets.  
It's purely cosmetic — no performance change, no root required. Just style.

## Contributing
This is a solo hunter's job. No contributions needed — but feel free to drop an issue or suggestion if you find a bug or got an idea.

Though I stole the `update-binary` from https://t.me/im_the_batman_who_laughs

## License
```
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
