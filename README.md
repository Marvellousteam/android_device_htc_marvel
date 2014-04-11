Device configuration for the HTC Wildfire S A510e (marvel).

  - Copyright (C) 2013 The OmniROM Project
  - Copyright (C) 2011 Andreas Schneider <asn@cryptomilk.org>
  - Copyright (C) 2013 OWL Project
  - Copyright (C) 2014 MarvelMod

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

------------------------------------------------------------------

* Description

  This repository is for OmniROM 4.3 on the HTC Wildfire S (marvel).
  It is still a work in progress.


* Boardinfo

  - Touchscreen
    Cypress CY8C_TMA

  - Sensors
    Gsensor: BOSCH_BMA150
    Compass: AKM8975
    Battery: TPS65200
    Light:   CM3602


* How To Build Omni for HTC Marvel

  - Make a workspace

  $ mkdir -p ~/omnirom/system;cd ~/omnirom/system


  - Do repo init & sync

  
  $ repo init -u git://github.com/cm-10-2-marvel/android.git -b omni-4.3;repo sync


  - Setup vendor

  $ ./vendor/cm/get-prebuilts


  - Setup environment

  $ source build/envsetup.sh;lunch omni_marvel-eng


  - Build OmniROM

  $ export USE_CCACHE=1;make -j4 bacon


* Thanks

  - Andreas Schneider
  - OWL Project
  - OmniROM
  - alquez
  - Droste
  - pabloPL
