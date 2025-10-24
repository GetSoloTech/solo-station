# Solo Station Robot Modules

This directory contains integration modules for different robot platforms compatible with Solo Station. Each module provides the necessary configuration, mounting adapters, and setup instructions for specific robots.

## Module Categories

### Manipulators
Robot arms and manipulation platforms
- Standard mounting interfaces
- Workspace calibration files
- Gripper/end-effector configurations

### Mobile Robots
Mobile bases and ground robots
- Platform mounting adapters
- Sensor positioning guides
- Navigation integration

### Humanoids
Humanoid robot platforms
- Full-body mounting solutions
- Multi-sensor calibration
- Bimanual task configurations

### Hands
Robotic hands and dexterous manipulators
- Wrist mounting options
- Tactile sensor integration
- Grasp dataset configurations

### Grippers
Various gripper mechanisms
- Quick-change mounting plates
- Force/torque sensor integration
- Object manipulation setups

### Quadrupeds
Four-legged robotic platforms
- Body mounting solutions
- Dynamic task configurations
- Outdoor/terrain setups

## Module Structure

Each robot module should contain:

```
robot-name/
├── README.md              # Robot-specific documentation
├── config.yaml            # Configuration parameters
├── models/                # 3D printable mounting adapters
│   ├── mounting_plate.stl
│   └── sensor_bracket.stl
├── calibration/           # Calibration files
│   └── workspace.json
└── examples/              # Usage examples
    └── data_collection.py
```

## Adding a New Robot

1. Create a new directory under the appropriate category
2. Copy the module template from `_template/`
3. Customize the configuration and 3D models
4. Document any special requirements
5. Submit a pull request

## Supported Robots

Browse robots at [robotsthatexist.com](https://robotsthatexist.com) and check the specific category folders for available modules.

### Coming Soon
- Open-source robot integrations
- Community-contributed modules
- Automated calibration tools
