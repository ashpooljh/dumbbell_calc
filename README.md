# dumbbell\_calc
A library and a cli tool to help assemble a modular dumbbell inventory

## Requirements

Python 3.5+

## Usage

```
$ python -i dumbbell.py
>>> d = Dumbbell(grip=1.5, disks=[0.75, 1, 2.5, 5])
```
`grip` represents the weight of the dumbbell's grip.  
`disks` is a list of disk weights, it's assumed that 2 disks are available of each of them.
```
>>> d.configurations()
[3.0, 3.5, 5.0, 6.5, 8.0, 8.5, 10.0, 11.5, 13.0, 13.5, 15.0, 16.5, 18.0, 18.5, 20.0]
```
This returns a sorted list of all possible weight configurations for this dumbbell.
```
>>> d.maxdelta()
1.5
```
This returns a maximum weight difference between any two configurations adjacent in the list.

More features are going to be implemented real soon...
