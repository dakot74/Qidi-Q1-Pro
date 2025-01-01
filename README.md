# Qidi-Q1-Pro
Upgrades and Tunning for Qidi Q1 Pro

_I apologize in advance for my English_

My upgades applied to the printer

Most of them find on internet (Printables.com, GitHub...), some my remixes of them...

**1. TPU seals for electronic bay**
  - https://www.printables.com/model/878779-qidi-q1-pro-heat-loss-plugs
  - https://www.printables.com/model/886627-qidi-q1-pro-rear-tpu-seal

**2. Better cooling for Motherboard with 80mm fan _(rework)_**
  - original https://www.printables.com/model/861709-qidi-q1-pro-motherboard-fan-plate
  - my rework https://www.printables.com/model/1017902-qidi-q1-pro-mothreboard-fan-80mm-holder
  - 
**3. External carbon filtration box**
 - original https://www.printables.com/model/895646-qidi-q1-pro-filter-scrubber-hepa-and-carbon-extern
 - my remix (not published yet)

**4. Internal exhaust duct _(rework)_**
 - originals [Printables.com](https://www.printables.com/model/904764-qidi-q1-pro-internal-exhaust-duct), [Makerworld.com](https://makerworld.com/en/models/411229?fbclid=IwZXh0bgNhZW0CMTEAAR3f0M9DgXlkferK0tAFzDghmkW5zvwlpZ_0zBMjcjAj5kIBMrbzlP3vYic_aem_Yo-cguwd-8sszccZO92pzQ#profileId-313181)
 - my rework (not published yet)

**5. Klipper tweaks (heated chamber)**
 - starting to print ASA, I have problems with temperature in heated chamber; all my prints fails due to an error ("Heater chamber not heating at expected rate"). Heater worked properly, side panels was realy hot (not measured), but temperature measured by chmaber temperature sensor can't reach required temperature. With long preheat time (and very hot side panels) I can be able to reach required temperature and start print, but after some time print failed to an mentioned error; after print start temp on temp chamber sensor goes down, chamber heater work on 100%, but not able to catch up required temp.
 - Googling, I find solution on [GitHub](https://github.com/qidi-community/Plus4-Wiki/tree/main/content/chamber-heater-investigation) _(qidi-community)_ wich solved my problem; the trick was to average the temperatures in the chamber from different sensors....
 - After editting Printer.cfg, Macros.cfg and adding some necessary files to Klipper compilation _(yes, Klipper version on Qidi Q1 Pro is old and does'nt know required syntax for "temperature_combined")_ I was able to print ASA with active heated chamber without problems ;-)
