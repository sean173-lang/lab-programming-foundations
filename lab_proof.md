HomeGuard – Lab Proof

1. Program File

homeguard_system.py

2. How to Run

Open the terminal in the project folder and run:

python3 homeguard_system.py

3. Project Description

HomeGuard is a simple smart-home security simulator written in Python.

The program uses a Sensor class to monitor four sensors:

Temperature

Smoke

Motion

Door

It supports three modes: HOME, AWAY, and SLEEP.

The program uses functions, dictionaries, lists, loops, and if/else statements to detect problems and display alerts. It also records events with timestamps.

4. Deterministic Tests

The simulator runs three scans with fixed readings.

Scan

Mode

Temperature

Smoke

Motion

Door

1

HOME

68°F

False

False

False

2

AWAY

30°F

True

True

True

3

SLEEP

100°F

False

False

True

Expected Results

Scan 1: No alerts.

Scan 2:

Frozen pipe risk

Smoke detected

Motion detected while away

Door opened while away

Motion and door triggered together

Scan 3:

Equipment failure risk

Door open longer than 5 minutes

Actual Output

Paste the actual terminal output here after running the program:

[INSERT ACTUAL OUTPUT]

5. Edge Case Test

The temperature sensor is reset using reset().

Expected result:

The sensor value becomes None.

isAbnormal() returns False.

The program does not crash.

Actual result:

[INSERT ACTUAL RESULT]

6. Random Readings

The program also demonstrates randomly generated sensor readings using Python's random module.

The fixed test cases are used separately to make the tests reproducible.

7. What I Learned

During this project, I learned how to use Python variables, dictionaries, lists, conditions, loops, and functions.

I also learned how to create a class, use self, and define methods such as read(), isAbnormal(), and reset().

The most challenging part was connecting the different parts of the program and understanding indentation.
