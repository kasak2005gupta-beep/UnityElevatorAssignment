# UnityElevatorAssignment
Unity 2D Elevator Simulation (Multiple Lifts)
An internship assignment developed for Underpin Technology, featuring a smart multi-elevator dispatch system built in Unity 6.

Project developed by: Kasak Gupta

Engine: Unity 6 (6000.0.47f1)

Environment: 2D Simulation

Scope: 3 Elevators, 5 Floors (Ground, 1st, 2nd, 3rd, 4th)

Duration: 2-day development window

Modular Architecture: Organized into 3 clean scripts: ElevatorController, ElevatorManager, and FloorButton.

Synchronized Physics: All elevators feature identical speeds and smooth Vector3 transitions to ensure zero "teleportation" between floors.

Organized groups: 3 folders (scripts, prefabs, scenes)

Submitted as: .unitypackage with dependencies included

Issue i faced: the standard 'nearest lift' logic caused lift1 to get stuck working on floor 3 and 4 ONLY, lift2 to get stuck working on floor 1 and 2 ONLY and lift3 to not move cause it was on ground floor from the start.

Solution i implemented: i have added a second logic as well, a sort of second/ third click feature to the buttons. If a floor button is pressed while a lift is already there, the system treats that lift as occupied and dispatches the next nearest elevator.

Result: each button can be pressed 2-3 times and the lifts will respond 1 at a time considering the nearest logic but also being able to move to all the floors through this, hence all lifts stay active throughout the floors.
