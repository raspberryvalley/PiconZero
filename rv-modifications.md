# Raspberry Valley Modifications

Please find a list of our modifications in this document

## Picon Zero for Python 3

We have slightly modified the **piconzero.py** (basically only print statements) to be compatible with our Python 3 code. The resulting file - **piconzero3.py** is added to the Python folder.

## Previous states added (speed)

Previous motor states were added to allow for new functionality

```python
CURRENTSPEED0 = 0  # current speed of motor 0
CURRENTSPEED1 = 0  # current speed of motor 1
OLDSPEED0 = 0  # old (previous) speed setting of motor 0
OLDSPEED1 = 0  # old (previous) speed setting of motor 1
```

These led to extensions to the **setMotor (motor, value)** function

## New functions added

```python
# increase speed: increases speed by delta
increaseSpeed(delta)
# set previous speed values
previousSpeed()
```