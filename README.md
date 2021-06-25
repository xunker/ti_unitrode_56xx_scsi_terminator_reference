# Compatibility Information for TI/Unitrode UC[C]56xx series SCSI terminator ICs

Information about cross-compatibility between various TI/Unitrode SCSI terminator ICs of the UC[C]56xx family, such as UC5605, UCC5606, etc.

A collection the IC datasheets can be found in the [datasheets](datasheets/) directory.

https://github.com/xunker/ti_unitrode_56xx_scsi_terminator_reference

## Cross-compatibility

All ICs are *pin-compatible* with any other IC with the same number of signal lines, but do not always share the same DISCNCT logic levels, termination resistance or feature set.

Examples:
* UCC5614 can be substituted for UCC5606 if you reverse the logic level to the DISCNCT pin
* UC5604 can replace UC5603 if you don't need negative clamping on the signal lines

## 9-Line SE
### Termination enabled by driving DISCNCT pin to ground

* [UC5603](datasheets/uc5603.pdf)
* [UC5604](datasheets/uc5604.pdf)
* [UC5612](datasheets/uc5612.pdf)
* [UC5613](datasheets/uc5613.pdf)
* [UCC5614](datasheets/ucc5614.pdf)
  * Also has a 2.5K-ohm mode by driving DISCNCT low via a 80K-150K ohm resistor
* [UCC5616](datasheets/ucc5616.pdf)

### Termination enabled by driving DISCNCT pin to Vcc

* [UC5605](datasheets/uc5605.pdf)
* [UCC5606](datasheets/ucc5606.pdf)
  * Also has a 2.5K-ohm mode by driving DISCNCT high via a 80K-150K ohm resistor
* [UCC5615](datasheets/ucc5615.pdf)
  * Features reverse-disconnect

## 9-Line LVD

All ICs disable termination by driving DISCNCT High.

* [UCC5630](datasheets/ucc5630.pdf)
  * Supports SE and LVD
* [UCC5632](datasheets/ucc5632.pdf)
  * Supports SE and LVD
* [UCC5640](datasheets/ucc5640.pdf)
  * Supports LVD Only

## 18-Line

### Termination enabled by driving DISCNCT pin to ground

* [UC5601](datasheets/uc5601.pdf)
* [UC5602](datasheets/uc5602.pdf)
* [UC5608](datasheets/uc5608.pdf)
* [UCC5610](datasheets/ucc5610.pdf)
* [UCC5618](datasheets/ucc5618.pdf)

### Termination enabled by driving DISCNCT pin to Vcc

* [UC5607](datasheets/uc5607.pdf)
* [UC5609](datasheets/uc5609.pdf)
* [UCC5611](datasheets/ucc5611.pdf)
  * Also has a 2.5K-ohm mode by driving DISCNCT high via a 80K-150K ohm resistor
* [UCC5617](datasheets/ucc5617.pdf)
## 27-Line

### Termination enabled by driving DISCNCT pin to ground

* [UCC5620](datasheets/ucc5620.pdf)
* [UCC5622](datasheets/ucc5622.pdf)

### Termination enabled by driving DISCNCT pin to Vcc

* [UCC5619](datasheets/ucc5619.pdf)
* [UCC5621](datasheets/ucc5621.pdf)
