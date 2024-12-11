# CuraEngineLE_Plugin_Infill_Generate

This Engine plugin extends the current infill patterns in CURA with:

- Continuous Honeycomb
- Normal Honey Comb
- Cura
- Honeycomb Fill
- ... You can create your own infill tills by adding `*.wtk` files in the `CuraEngineTiledInfill/tiles/` folder even when you already installed it in CuraLE...

NOTE: Please note that this plugin is Experimental and adding custom infills is not possible at the moment.

## Licenses

### Front End CuraLE Plugin

[![Badge LGPL]][LGPL]

------------------------------

### C++ Business logic headers for the CuraEngine plugin logic

[![Badge BSD-4]][BSD]

------------------------------

### C++ Infill Generation Header

[![Badge AGPL]][AGPL]

## Installation

1. Configure Conan

   Before you start, if you use conan for other (big) projects as well, it's a good idea to either switch conan-home and/or backup your existing conan configuration(s).

   That said, installing our config goes as follows:

   ```bash
   pip install conan==2.7.0
   conan config install https://github.com/lulzbot3d/Conan_LulzBot_Config.git
   conan profile new default --detect --force
   ```

2. Clone CuraEngineLE_Plugin_Infill_Generate

   ```bash
   git clone https://github.com/lulzbot3d/CuraEngineLE_Plugin_Infill_Generate.git
   cd CuraEngineLE_Plugin_Infill_Generate
   ```

3. Install & Build CuraEngine (Release OR Debug)

   ```bash
   conan install . --build=missing --update -s build_type=Debug/Release
   ```

[For more info](https://github.com/lulzbot3d/CuraEngineLE/wiki/Building-CuraEngine-From-Source)

<!------------------------------------------------------------------>

[Badge LGPL]: https://img.shields.io/badge/License-LGPL--3.0-orange?style=for-the-badge&logoColor=white&logo=GNU
[Badge BSD-4]: https://img.shields.io/github/license/lulzbot3d/CuraEngineLE_Plugin_Infill_Generate?style=for-the-badge&logoColor=white&logo=BSD
[Badge AGPL]: https://img.shields.io/badge/License-AGPL--3.0-orange?style=for-the-badge&logoColor=white&logo=GNU

[LGPL]: CuraEngineTiledInfill/LICENSE
[BSD]: LICENSE
[AGPL]: LICENSE-AGPL-3.0
