# Constrained Device Application (Connected Devices)

## Lab Module 04

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-04-001 - Lab Module 04](https://github.com/orgs/programming-the-iot/projects/1#column-10488379).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
measuring and modeling the data generate as part of a simple sensor and actuator simulation environment build for the CDA. The generated data will represent a small environmental sensors, and process simple threshold crossings to trigger simulated actuation events

How does your implementation work?
 It will create an object of ConstrainedDeviceApp which has objecct of DeviceDataManager. DeviceDataManager will get data metrics from SensorAdapterManager, emPerformanceManager, and AtuatorAdapterManager. 
Then it will start app.Then DeviceDataManager call SystemPerformanceManager ,SystemPerformanceManager, AtuatorAdapterManager`  which will eventurally get metrics from SystemCpuUtilTask and SystemMemUtilTask.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/NU-CSYE6530/cda-lab-modules-alasundkar/tree/labmodule04

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![Image of CDA-LAB04](cda.png)
### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- src/test/python/programmingtheiot/part02/unit/sim/HumiditySensorSimTaskTest.p 
- src/test/python/programmingtheiot/part02/unit/sim/HvacActuatorSimTaskTest.py
- src/test/python/programmingtheiot/part02/unit/sim/HumidifierActuatorSimTaskTest.py
- src/test/python/programmingtheiot/part02/unit/sim/PressureSensorSimTaskTest.py- src/test/python/programmingtheiot/part02/unit/sim/TemperatureSensorSimTaskTest.py
- src/test/python/programmingtheiot/part02/unit/data/ActuatorDataTest.py
- src/test/python/programmingtheiot/part02/unit/data/SensorDataTest.py
- src/test/python/programmingtheiot/part02/unit/data/BaseIotDataTest.py
- src/test/python/programmingtheiot/part02/unit/data/SystemPerformanceDataTest.py

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)


- src/test/python/programmingtheiot/part02/integration/system/ActuatorAdapterManagerTest.py
- src/test/python/programmingtheiot/part02/integration/system/SensorAdapterManagerTest.py 
- src/test/python/programmingtheiot/part02/integration/emulated/ActuatorEmulatorManagerTest.py
- src/test/python/programmingtheiot/part02/integration/emulated/HumidifierEmulatorTaskTest.py
- src/test/python/programmingtheiot/part02/integration/emulated/HvacEmulatorManagerTest.py
- src/test/python/programmingtheiot/part02/integration/emulated/SenseHatEmulatorManagerTest.py
- src/test/python/programmingtheiot/part02/integration/emulated/LedDiaplayEmulatorManagerTest.py
- src/test/python/programmingtheiot/part02/integration/emulated/SensorEmulatorManagerTest.py


EOF.
