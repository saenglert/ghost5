# FlyingBear Ghost 5
This repo contains my personal information and configurations about the FlyingBear Ghost 5 3D Printer.

## Firmware

The firmware the printer ships with contains multiple errorous values as is explained in the [video by drucktipps3D](https://www.youtube.com/watch?v=z7eNHElRNNM). The `robin-nano35+cfg.txt` file in this repository contains the fixes mentioned in the video. 

#### Attention

The `robin-nano35+cfg.txt` also containes changes to the direction of the z-axis and extruders which are only needed when using TMC2208 stepper motor drivers for the Z axis and the extruder motor (see below).

## Silent Stepper Driver Upgrade
My Ghost 5 came equipped with a TMC2208 driver for the X and Y axis respectively. Z and the extruder were using a basic A4988 driver which means the stepper motors are quite noisy.

Upgrading the Z axis and the extruder drivers to TMC2208s can solve this problem. However, this requires some hardware tweaking as can be seen in [this guide](https://flyingbearghost.com/en/tmc2209).

## Filament Cooling

By default, the 5020 fan the printhead comes equipped is wholy inadequat to cool the filament while extruding. Because the airflow is not directed at the nozzle, prints are prone to stringing and failing bridges.

An easy improvement is a [simple fan duct](https://www.thingiverse.com/thing:4597917) which can be clipped on the fan and improves the quality noticeably. However, this is still not enough to successfully print with [certain filaments](https://www.dasfilament.de/filament-refill/pla-1-75-mm/270/pla-filament-1-75-mm-weiss-refill-800-g). Next [a completly new printhead](https://www.thingiverse.com/thing:4615328) was tryed which still does not provide enough cooling.

## Links
* [drucktipps3D Youtube Video](https://www.youtube.com/watch?v=z7eNHElRNNM)
* [FlyingBear Firmware on Google Drive](https://drive.google.com/drive/folders/1ZUuk_V8Bdn0Vt0OC19J2wQ0Nd3v5MbL4)
* [Guide to upgrading to TMC2208 drivers](https://flyingbearghost.com/en/tmc2209)
* [Simple fan duct on Thingiverse](https://www.thingiverse.com/thing:4597917)
* [Universal Printhead v2 on Thingiverse](https://www.thingiverse.com/thing:4615328)