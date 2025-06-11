# Software Developer – Lua Questions & Answers

Each question is labeled (e.g., `L4 - 27`) and includes both the original code (possibly with mistakes) and the corrected version.

---

## L0- 1. fixBlipID

### Question

~~~lua
local blip = createBlip(1500, -1500, '3') -- A developer incorrectly used a string instead of a number for the blip ID. Fix it by using a numeric ID.
~~~

### Answer

~~~lua
local blip = createBlip(1500, -1500, 3)
~~~

---

## L0- 2. fixVehicleModel

### Question

~~~lua
local vehicle = createVehicle("InvalidModel", 1520, -1520, 13) -- A developer used an invalid model name instead of a model ID. The correct model ID should be 411.
~~~

### Answer

~~~lua
local vehicle = createVehicle(411, 1520, -1520, 13)
~~~

---
