# Modified Acer Predator Turbo and RGB Keyboard Linux Module

![Keyboard](keyboard.webp)

**Fork of [JafarAkhondali's Module](https://github.com/JafarAkhondali/acer-predator-turbo-and-rgb-keyboard-linux-module)**

This project is a modified fork of [JafarAkhondali's Acer Predator Turbo and RGB Keyboard Linux Module](https://github.com/JafarAkhondali/acer-predator-turbo-and-rgb-keyboard-linux-module). It closely adheres to the original [Linux kernel's Acer WMI driver](https://github.com/torvalds/linux/blob/master/drivers/platform/x86/acer-wmi.c) to enhance support for newer Acer Predator devices, specifically models **PHN16-71** and above.

## **Key Differences from Original Fork**

- **Alignment with Original Kernel Code:** Maintains closer adherence to the original Linux kernel driver (`acer-wmi.c`), ensuring better compatibility and stability.
- **Enhanced Support for Newer Models:** Improved functionality for newer Acer Predator V4 devices, including **PHN16-71** and later models.
- **Optimized for Predator V4 Devices:** Modifications to support the advanced features of Predator V4 series.

## **Warning**

### Use at Your Own Risk!

Acer was not involved in developing this driver. All development is based on reverse engineering the official Predator Sense app. This driver interacts with low-level WMI methods that haven't been tested on all series.

## **Compatibility**

**Supported Models:**

| Product Name | Turbo Mode (Implemented) | Turbo Mode (Tested) | RGB (Implemented) | RGB (Tested) |
|--------------|:------------------------:|:-------------------:|:-----------------:|:------------:|
| PHN16-71     | Yes                      | Yes                 | Yes               | Yes          |
| PHN16-72     | Yes                      | No                  | Yes               | No           |
| ...          | ...                      | ...                 | ...               | ...          |

*Please add your model if it's not listed by opening an issue.*

**Determine Your Model:**
```bash
sudo dmidecode -s system-product-name
