# Qt LGPL Compliance Notice

This repository provides open source compliance information for **DJI Studio**,  
which uses the Qt framework under the **GNU Lesser General Public License v3 (LGPLv3)**.

---

## Qt Version Used

| Item          | Details                                                           |
|---------------|-------------------------------------------------------------------|
| Framework     | Qt                                                                |
| Version       | **6.5.3**                                                         |
| License       | LGPLv3                                                            |
| Official Site | https://www.qt.io                                                 |
| Source Code   | https://code.qt.io/cgit/qt/qt5.git/tag/?h=v6.5.3                  |
| Release Notes | https://doc.qt.io/qt-6/whatsnew65.html                            |

---

## Our Modifications to Qt

DJI Studio has made modifications to certain Qt 6.5.3 libraries.  
In compliance with LGPLv3, we have made these modifications publicly available
in the following repositories:

| Repository | Branch | Description |
|------------|--------|-------------|
| [DJIStudio/qt5](https://github.com/DJIStudio/qt5) | `6.5.3_DJIStudio` | Modified Qt 6.5.3 source code (top-level) |
| [DJIStudio/qtbase](https://github.com/DJIStudio/qtbase) | `6.5.3_DJIStudio` | Modified Qt 6.5.3 base module source code |
| [DJIStudio/qtdeclarative](https://github.com/DJIStudio/qtdeclarative) | `6.5.3_DJIStudio` | Modified Qt 6.5.3 declarative module source code |

> The branch `6.5.3_DJIStudio` is based on the official **Qt 6.5.3** release tag  
> and contains all modifications made by DJI Studio.  
> You are free to review, use, and rebuild these modified Qt libraries  
> in accordance with the terms of LGPLv3.

---

## How DJI Studio Uses Qt

- DJI Studio is built against **Qt 6.5.3** under the LGPLv3 license.
- DJI Studio links against Qt libraries **dynamically**, ensuring that  
  end users can replace the Qt libraries with their own versions.
- DJI Studio's own application source code remains proprietary,  
  as permitted under LGPLv3.
- No GPL-only Qt modules are used in DJI Studio.

---

## Replacing Qt Libraries

In accordance with LGPLv3, users have the right to replace the Qt 6.5.3 libraries  
used by DJI Studio with modified versions.

**Steps to replace Qt libraries:**

1. Clone our modified Qt 6.5.3 source from the `6.5.3_DJIStudio` branch:
   ```bash
   git clone -b 6.5.3_DJIStudio https://github.com/DJIStudio/qt5.git
   git clone -b 6.5.3_DJIStudio https://github.com/DJIStudio/qtbase.git
   git clone -b 6.5.3_DJIStudio https://github.com/DJIStudio/qtdeclarative.git
   ```

2. Build the Qt 6.5.3 libraries following the official Qt build instructions:  
   https://doc.qt.io/qt-6/build-sources.html

3. Replace the Qt `.dll` / `.so` / `.dylib` files in the DJI Studio  
   installation directory with your newly built libraries.

> ⚠️ Note: Replacing Qt libraries may cause instability.  
> DJI Studio does not provide support for installations using modified libraries.

---

## License Texts

The full text of the licenses used are available below:

- [GNU Lesser General Public License v3 (LGPLv3)](https://www.gnu.org/licenses/lgpl-3.0.html)
- [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.html)  
  *(LGPLv3 incorporates GPLv3 by reference)*

---

## Third-Party Attributions

Qt 6.5.3 is developed by The Qt Company and contributors.  
For full attribution and copyright notices, please refer to:  
https://doc.qt.io/qt-6/licenses-used-in-qt.html

---

## Contact

If you have any questions regarding our open source compliance,  
please contact us at:

📧 **opensource@dji.com**  
🌐 **https://www.dji.com**

---

*Last updated: 2026*  
*This notice applies to DJI Studio and its distributed Qt 6.5.3 libraries.*