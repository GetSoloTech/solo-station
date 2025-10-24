# [Robot Name] - Solo Station Module

## Overview

Brief description of the robot platform and its capabilities.

**Robot Type:** [Manipulator/Mobile/Humanoid/Hand/Gripper/Quadruped]
**Manufacturer/Project:** [Name]
**DOF:** [Number of degrees of freedom]
**Open Source:** [Yes/No]

## Compatibility

- Solo Station Version: 1.0+
- Required Components:
  - [ ] Base station platform
  - [ ] Mounting adapter (custom)
  - [ ] Sensor brackets
  - [ ] Calibration markers

## Hardware Requirements

### 3D Printed Components
- Mounting plate (see `models/mounting_plate.stl`)
- Sensor brackets (see `models/sensor_bracket.stl`)
- [Any additional custom parts]

### Additional Hardware
- M4 bolts (quantity: X)
- [Other hardware needed]

## Setup Instructions

### 1. Print Components
Print all STL files from the `models/` directory using:
- Material: PETG or PLA
- Layer height: 0.2mm
- Infill: 20%+

### 2. Assembly
1. Attach mounting plate to robot base
2. Install sensor brackets
3. Connect calibration markers
4. Verify stability and clearances

### 3. Calibration
```bash
python calibration/calibrate.py --robot [robot-name]
```

### 4. Testing
```bash
python examples/test_setup.py
```

## Configuration

Edit `config.yaml` to customize:
- Workspace dimensions
- Sensor positions
- Safety limits
- Data collection parameters

## Example Usage

### Data Collection
```python
from solo_station import RobotModule

robot = RobotModule.load('[robot-name]')
robot.calibrate()
robot.collect_data(task='pick_place', episodes=100)
```

### Inference
```python
robot.load_model('policy.pth')
robot.run_inference()
```

## Known Issues

- [List any known limitations or issues]

## Resources

- Robot documentation: [Link]
- Community examples: [Link]
- Support forum: [Link]

## Contributing

Improvements welcome! Please test thoroughly and document any changes.
