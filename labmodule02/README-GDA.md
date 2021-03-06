# Gateway Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-02-001 - Lab Module 02](https://github.com/orgs/programming-the-iot/projects/1#column-9974938).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
This implementation will add system performance monitoring to the application

How does your implementation work?
It will create an object of GatewayDeviceAppTest and then it will start app.Then it will call SystemPerformanceManager , which will eventurally get metrics from SystemCpuUtilTask and SystemMemUtilTask.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/NU-CSYE6530/gda-lab-modules-alasundkar/tree/labmodule02

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![Image of GDA-LAB02](labmodule02GDA.png)

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- src/test/java/programmingtheiot/part01/unit/common/ConfigUtilTest.java
- src/test/java/programmingtheiot/part01/unit/system/SystemCpuUtilTaskTest.java
- src/test/java/programmingtheiot/part01/unit/system/SystemMemUtilTaskTest.java

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- src/test/java/programmingtheiot/part01/integration/system/SystemPerformanceManagerTest.java
- src/test/java/programmingtheiot/part01/integration/app/GatewayDeviceAppTest.java
- 

EOF.
