# Notes

## references

- paper looking at different voltage sensors:
  - https://www.mdpi.com/1424-8220/22/20/7769
  - had noise issues with ZMPT, could be due to overtuning gain from the oversized input resistor sizing
- issues with 820k resistor value and component footprint/package
  - https://forum.arduino.cc/t/warning-about-zmpt101b-voltage-sensor-modules-with-active-output/693258
  - line: https://www.digikey.ca/en/products/detail/vishay-dale/CRCW2512127KFKEG/1173717
  - burden: https://www.digikey.ca/en/products/detail/vishay-beyschlag-draloric-bc-components/MCA1206MD1000DP500/3883970
- OpenEnergyMonitor (EMON)
  - links
    - https://github.com/openenergymonitor/emonVs
    - https://github.com/openenergymonitor/emonpi2
    - https://github.com/openenergymonitor/emontx4
  - Engineering report on SCT-013-000 by EMON
    - https://docs.openenergymonitor.org/electricity-monitoring/ct-sensors/yhdc-sct-013-000-ct-sensor-report.html
  - Interfacing CT sensors by EMON
    - https://docs.openenergymonitor.org/electricity-monitoring/ct-sensors/interface-with-arduino.html
  - Also uses ZMPT103B (x3) but part of power supply that sends 3 phase transformed voltage along with 5V and GND for power over an RJ45-8

## parts dump

- ZMCT/ZMPT source
  - https://a.co/d/7U0w1WT
- SCT-013-xxx source
  - https://a.co/d/iOVg5ov
- current sensor used by EMON
  - https://dgechun.en.made-in-china.com/product/YEmpWMfyOscU/China-Echun-UL-Certification-Split-Core-Current-Transformer-Ecs12-12mm-Hole-AC-100A-333mv-with-3-5mm-Audio-Jack.html
    - default comes 333mV output but can be ordered for diff current or voltage
  - https://shop.openenergymonitor.com/100a-split-core-current-transformer/
- barrel jack for current sensor
  - https://www.digikey.ca/en/products/detail/same-sky-formerly-cui-devices/SJ-3524-SMT-TR/281298
- big 0R resistor
  - https://www.digikey.ca/en/products/detail/vishay-dale/RCL06120000Z0EA/2587612
- digital potentiometer 100k non-volatile
  - https://www.digikey.ca/en/products/detail/microchip-technology/MCP4161-104E-SN/1874204
