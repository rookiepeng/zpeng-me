<h2><a href="https://github.com/rookiepeng/Multi-Device-XBee" rel="noopener" target="_blank"><i class="fa fa-github" aria-hidden="true"></i> View Source Code on GitHub</a></h2>

------

Use MSP430 to sample analog signals (from motion radars in my application), and transfer data to a computer through XBee (ZigBee) modules.

## Environments

### Hardware

- MSP430 (M430F261X)
- XBee module

### Software

- IAR Embedded Workbench for MSP430
- National Instruments (NI) LabVIEW 2015 or newer

## Configuration

### Connections

![Connections](https://rookiepeng.github.io/Multi-Device-XBee/connection.png)

### XBee modules

#### Coordinator

Connect with the computer

![Coordinator](https://rookiepeng.github.io/Multi-Device-XBee/coordinator.png)

#### End device

Connect with the sensors

![end-device](https://rookiepeng.github.io/Multi-Device-XBee/end-device.png)

## Running

### Query Mode

LabVIEW code: ```LabVIEW/XBee_Query.vi```

- Support 3 devices at the same time
- Sampling: 20 Hz x 12 bits x 2 channels each device
- Update every 10 s

### Continuous Mode

LabVIEW code: ```LabVIEW/XBee_Continuous.vi```

- 1 device
- Sampling: 80 Hz x 12 bits x 2 channels
- Update every 0.0125 s

## Screenshots

### Query Mode

![Query mode](https://rookiepeng.github.io/Multi-Device-XBee/queryMode.png)

### Continuous Mode

![Continuous mode](https://rookiepeng.github.io/Multi-Device-XBee/continuousMode.png)
