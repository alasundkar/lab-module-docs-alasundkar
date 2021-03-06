# Constrained Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-05-001 - Lab Module 05](https://github.com/orgs/programming-the-iot/projects/1#column-10488421).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
use a DeviceDataManager to orchestrate the information flow within the application, and a new component is added – DataUtil – to provide a centralized data translation utility for converting the CDA’s data container objects into a format that other systems can readily consume

How does your implementation work?
We wll create RedisPersistenceAdapter and integrate with DeviceDataManager. Configure redis with CDA.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/NU-CSYE6530/cda-lab-modules-alasundkar/tree/labmodule05 

### UML Design Diagram(s)

![Image of CDA-LAB05](cda.png)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- /src/test/python/programmingtheiot/part02/integration/DataUtilTest
 

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- src/test/python/programmingtheiot/part02/integration/data/DataIntegrationTest.py

EOF.
