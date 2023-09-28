# Azure_Kinect_practice
# 1. Installation on ubuntu20.04

    $ curl -sSL https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
    $ sudo apt-add-repository https://packages.microsoft.com/ubuntu/18.04/prod
    $ curl -sSL https://packages.microsoft.com/config/ubuntu/18.04/prod.list | sudo tee /etc/apt/sources.list.d/microsoft-prod.list
    $ curl -sSL https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
    $ sudo apt-get update
    $ sudo apt install libk4a1.3-dev
    $ sudo apt install libk4abt1.0-dev
    $ sudo apt install k4a-tools=1.3.0

## Run without sudo
Copy 'scripts/99-k4a.rules' into '/etc/udev/rules.d/'. refer to [here](https://github.com/microsoft/Azure-Kinect-Sensor-SDK/blob/develop/docs/usage.md#linux-device-setup).
    
# 2. Some Links
### Python API
https://unanancyowen.github.io/k4asdk_python_apireference/

### ROS API
https://github.com/microsoft/Azure_Kinect_ROS_Driver

### Azure Kinect example
https://github.com/microsoft/Azure-Kinect-Samples
