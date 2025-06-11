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
## L0- 3. fixPedModel

### Question

~~~lua
local ped = createPed(999, 1530, -1530, 13) -- A developer used an invalid ped model ID. The correct model ID is 0.
~~~

### Answer

~~~lua
answer
~~~

---
---
## L0- 4. fixPickupType

### Question

~~~lua
local pickup = createPickup(0, 0, 3, "invalidType") -- The developer used an invalid pickup type. Use a valid pickup type which is 3.
~~~

### Answer

~~~lua
answer
~~~

---

---
## L0- 5. fixMarkerShape

### Question

~~~lua
local marker = createMarker(10, 10, 3, "unknownShape") -- The developer used an unknown shape. Use a valid shape which is "cylinder".
~~~

### Answer

~~~lua
answer
~~~

---
## L0- 6. fixColShapeRadius

### Question

~~~lua
local colShape = createColCircle(10, 10, "invalidRadius") -- The developer set an invalid radius. Use a valid radius which is 5.
~~~

### Answer

~~~lua
answer
~~~

---

## L1- 7. fixTimerFunction

### Question

~~~lua
setTimer("invalidFunction", 1000, 1) -- A developer tried to use a string instead of a valid function. Use an embedded function that output to chatbox "Timer completed!" once in a second.
~~~

### Answer

~~~lua
ans
~~~

---## L1- 8.fixRenderHandler

### Question

~~~lua
addEventHandler("onClientRender", root, "nonexistentFunction") -- A developer attached a non-existent function. The correct function name is "renderHandling".
~~~

### Answer

~~~lua
ans
~~~

---
## L1- 9.fixCustomEvent

### Question

~~~lua
addEvent("invalidEvent", false) -- The developer used an invalid event name. Change it to "validEvent". Also the event needs to be triggerable remotely so arg 2 should be true.
~~~

### Answer

~~~lua
ans
~~~

---
## L1- 10. fixShaderFile

### Question

~~~lua
local shader = dxCreateShader("invalid.fx") -- The developer used a missing shader file. Use "valid.fx".
~~~

### Answer

~~~lua
ans
~~~

---
## L1- 11.fixTextPosition

### Question

~~~lua
dxDrawText("Hello", "invalidX", 500) -- The developer used an invalid X coordinate. Replace it with 300.
~~~

### Answer

~~~lua
ans
~~~

---
## L1- 12. fixSoundFile

### Question

~~~lua
local sound = playSound("invalid.mp3") -- The developer referenced a missing sound file. Use "valid.mp3".
~~~

### Answer

~~~lua
ans
~~~

---
## L2- 13.FixGUIWindowPosition

### Question

~~~lua
local window = guiCreateWindow(500, "invalidY", 300, 400, "My Window", false) -- The developer used an invalid Y coordinate. Use 200.
~~~

### Answer

~~~lua
ans
~~~

---
## L2- 14. fixButtonPosition

### Question

~~~lua
local button = guiCreateButton("invalidX", 200, 100, 50, "Click Me", false) -- The developer used an invalid X coordinate. Use 150.
~~~

### Answer

~~~lua
ans
~~~

---
