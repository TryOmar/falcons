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
local ped = createPed(0, 1530, -1530, 13)
~~~

---

## L0- 4. fixPickupType

### Question

~~~lua
local pickup = createPickup(0, 0, 3, "invalidType") -- The developer used an invalid pickup type. Use a valid pickup type which is 3.
~~~

### Answer

~~~lua
local pickup = createPickup(0, 0, 3, 3)
~~~

---

## L0- 5. fixMarkerShape

### Question

~~~lua
local marker = createMarker(10, 10, 3, "unknownShape") -- The developer used an unknown shape. Use a valid shape which is "cylinder".
~~~

### Answer

~~~lua
local marker = createMarker(10, 10, 3, "cylinder")
~~~

---

## L0- 6. fixColShapeRadius

### Question

~~~lua
local colShape = createColCircle(10, 10, "invalidRadius") -- The developer set an invalid radius. Use a valid radius which is 5.
~~~

### Answer

~~~lua
local colShape = createColCircle(10, 10, 5)
~~~

---

## L1- 7. fixTimerFunction

### Question

~~~lua
setTimer("invalidFunction", 1000, 1) -- A developer tried to use a string instead of a valid function. Use an embedded function that output to chatbox "Timer completed!" once in a second.
~~~

### Answer

~~~lua
setTimer(function() outputChatBox("Timer completed!") end, 1000, 1)
~~~

---

## L1- 8. fixRenderHandler

### Question

~~~lua
addEventHandler("onClientRender", root, "nonexistentFunction") -- A developer attached a non-existent function. The correct function name is "renderHandling".
~~~

### Answer

~~~lua
addEventHandler("onClientRender", root, renderHandling)
~~~

---

## L1- 9. fixCustomEvent

### Question

~~~lua
addEvent("invalidEvent", false) -- The developer used an invalid event name. Change it to "validEvent". Also the event needs to be triggerable remotely so arg 2 should be true.
~~~

### Answer

~~~lua
addEvent("validEvent", true)
~~~

---

## L1- 10. fixShaderFile

### Question

~~~lua
local shader = dxCreateShader("invalid.fx") -- The developer used a missing shader file. Use "valid.fx".
~~~

### Answer

~~~lua
local shader = dxCreateShader("valid.fx")
~~~

---

## L1- 11. fixTextPosition

### Question

~~~lua
dxDrawText("Hello", "invalidX", 500) -- The developer used an invalid X coordinate. Replace it with 300.
~~~

### Answer

~~~lua
dxDrawText("Hello", 300, 500)
~~~

---

## L1- 12. fixSoundFile

### Question

~~~lua
local sound = playSound("invalid.mp3") -- The developer referenced a missing sound file. Use "valid.mp3".
~~~

### Answer

~~~lua
local sound = playSound("valid.mp3")
~~~

---

## L2- 13. FixGUIWindowPosition

### Question

~~~lua
local window = guiCreateWindow(500, "invalidY", 300, 400, "My Window", false) -- The developer used an invalid Y coordinate. Use 200.
~~~

### Answer

~~~lua
local window = guiCreateWindow(500, 200, 300, 400, "My Window", false)
~~~

---

## L2- 14. fixButtonPosition

### Question

~~~lua
local button = guiCreateButton("invalidX", 200, 100, 50, "Click Me", false) -- The developer used an invalid X coordinate. Use 150.
~~~

### Answer

~~~lua
local button = guiCreateButton(150, 200, 100, 50, "Click Me", false)
~~~

---

## L2- 15. fixMemoWidth

### Question

~~~lua
local memo = guiCreateMemo(300, 200, "invalidWidth", 100, "Enter text...", false) -- The developer used an invalid width. Use 250.
~~~

### Answer

~~~lua
local memo = guiCreateMemo(300, 200, 250, 100, "Enter text...", false)
~~~

---

## L2- 16. fixImageHeight

### Question

~~~lua
local image = guiCreateStaticImage(400, 300, 100, "invalidHeight", "image.png", false) -- The developer used an invalid height. Use 80.
~~~

### Answer

~~~lua
local image = guiCreateStaticImage(400, 300, 100, 80, "image.png", false)
~~~

---

## L2- 17. fixLabelHeight

### Question

~~~lua
local label = guiCreateLabel(10, 20, 200, "invalidHeight", "Hello World", false) -- The developer used an invalid height. Use 30.
~~~

### Answer

~~~lua
local label = guiCreateLabel(10, 20, 200, 30, "Hello World", false)
~~~

---

## L2- 18. fixProgressBarParent

### Question

~~~lua
local progressBar = guiCreateProgressBar(50, 100, 200, 30, "invalidParent") -- The developer set an invalid parent. Use nil for no parent.
~~~

### Answer

~~~lua
local progressBar = guiCreateProgressBar(50, 100, 200, 30, nil)
~~~

---

## L3- 19. fixEditBoxWidth 

### Question

~~~lua
local editBox = guiCreateEdit(100, 200, "invalidWidth", 30, "Text", false) -- The developer used an invalid width. Use 150.
~~~

### Answer

~~~lua
local editBox = guiCreateEdit(100, 200, 150, 30, "Text", false)
~~~

---

## L3- 20. fixGridListHeight

### Question

~~~lua
local gridList = guiCreateGridList(300, 400, 250, "invalidHeight", false) -- The developer used an invalid height. Use 300.
~~~

### Answer

~~~lua
local gridList = guiCreateGridList(300, 400, 250, 300, false)
~~~

---

## L3- 21. fixCheckBoxY

### Question

~~~lua
local checkBox = guiCreateCheckBox(50, "invalidY", 150, 20, "Check Me", false, false) -- The developer used an invalid Y coordinate. Use 100.
~~~

### Answer

~~~lua
local checkBox = guiCreateCheckBox(50, 100, 150, 20, "Check Me", false, false)
~~~

---

## L3- 22. fixRadioButtonX

### Question

~~~lua
local radioButton = guiCreateRadioButton("invalidX", 200, 120, 20, "Option", false) -- The developer used an invalid X coordinate. Use 75.
~~~

### Answer

~~~lua
local radioButton = guiCreateRadioButton(75, 200, 120, 20, "Option", false)
~~~

---

## L3- 23. fixTabPanelHeight 

### Question

~~~lua
local tabPanel = guiCreateTabPanel(10, 10, 400, "invalidHeight", false) -- The developer used an invalid height. Use 250.
~~~

### Answer

~~~lua
local tabPanel = guiCreateTabPanel(10, 10, 400, 250, false)
~~~

---

## L3- 24. fixTabParent

### Question

~~~lua
local tab = guiCreateTab("My Tab", "invalidParent") -- The developer used an invalid parent. The valid tab panel parent name is 'tabPanel'.
~~~

### Answer

~~~lua
local tab = guiCreateTab("My Tab", tabPanel)
~~~

---

## L4- 25. fixAdditionFunction

### Question

~~~lua
function addNumbers(a, b)
    return a + b -- The developer forgot to convert a and b to numbers. Ensure they are numbers before adding. (keep the function this way, but with ensuring a and b are numbers
end
~~~

### Answer

~~~lua
function addNumbers(a, b)
    return tonumber(a) + tonumber(b)
end
~~~

---
