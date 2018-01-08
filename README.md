# Description

the program Photoluminescence Excitation Map (PLEM) is used to record
Excitation/Emission Maps. The technique is used for characterizing Carbon
Nanotubes. In its current version the program it is used for microscopy of
freely suspended carbon nanotube samples.

files can be loaded to IgorPro with the [igor PLEM loader](https://github.com/ukos-git/igor-swnt-plem) found in my other repository.

# Credits

* **PLEMv1** initial version by Tilman C. Hain
* **PLEMv2** improved version by Tilman C. Hain, Daniel Zuleeg, Matthias J. Kastner
* **PLEMv3** much more versatile version by Matthias J. Kastner

contents in folder other are supplied via manufacturer's DEV examples see
section installation.
Nanostage icons Designed by Freepik and distributed by Flaticon

# Standalone Versions
* https://github.com/ukos-git/labview-xenics-xeva

# Hardware Setup

* ANDOR Shamrock monochromator with attached Newton and iDus
* Physikalische Instrumente (PI) nanostage P-563.3CD controlled by E-712
* NKT SuperK Extreme lightsource with attached NKT Varia for wavelength
  control.
* Thorlabs PM100D Powermeter for measuring the lightsource excitation power
* simple custom built digital I/O board to use the external control of NKT
  SuperK. Board was manufactured by velleman.

# Installation

install the following dependencies supplied by the manufacturers' Dev Kits:

## PI nanostage 

PI SDK Version 5.3.1

folder: *other/pi*

* **DIRECTORY** E-712_GCS_LabVIEW_digital
  * E712_All_VIs.vi
  * E712_Configuration_Setup.vi
  * **DIRECTORY** Low Level
    * Analog Control.llb
    * Communication.llb
    * File handling.llb
    * GCSTranslator.dll
    * General command.llb
    * Joystick.llb
    * Limits.llb
    * Old commands.llb
    * Optical or Analog Input.llb
    * PZT voltage.llb
    * Scan support.llb
    * Special command.llb
    * Support.llb
    *  WaveGenerator.llb

## NKT lightsource

folder: *other/nkt*
* NGSerialPort.vi
* NGSerialPort_global.vi

## thorlabs powermeter

folder: *other/thorlabs*

* **DIRECTORY** PM100D Simple Example
  * PM100D Simple Example.vi
  * PM100D_Close.vi
  * PM100D_ConfMeas.vi
  * PM100D_GetSystemInfo.vi
  * PM100D_Initialize.vi
  * PM100D_Open.vi
  * PM100D_Read.vi
  * PM100D_SensIDNFlag.vi
  * PM100D_SensorFlag.vi
  * PM100D_SYST-ERR.vi
  * PM100D_Write.vi
  * Select INSTR Dialog.vi
  * visarc

## velleman board

folder: *other/velleman*
* K8055D.dll

## IgorPro IBW

[Igor Pro IBW v5 export](http://www.igorexchange.com/project/LVarray2ibw) 2010 by Andreas Wirsing

folder: *other/igor-exchange*
* igorBinV5.llb

## andor monochromator/detector

folder: *other/andor*
* atmcd32d.bas 
* atmcd32d.dll
* ATMCD32D.H
* atmcd32d.lib
* ATMCD32D.pas
* atmcd32d.vb

## xenics xeva

install via labview library manager

## flaticon icons library

Arrow Collection
by Madebyoliver
License: Flaticon Basic License 
http://file000.flaticon.com/downloads/license/license.pdf

folder: *other/flaticon*
* **DIRECTORY** 137476-arrow-collection
* **DIRECTORY** 148705-essential-collection

