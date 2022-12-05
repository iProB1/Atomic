# ImGui Documentation for Growtopia Executor
* **[Example](#Example)**
* **[Functions](#functions)**

## functions
* **[Tab](#Tab)**
* **[RemoveTabs](#RemoveTabs)**
* **[GetItemsCount](#GetItemsCount)**
* **[Button](#Button)**
* **[Checkbox](#Checkbox)**
* **[Spacing](#Spacing)**
* **[SameLine](#SameLine)**
* **[Text](#Text)**
* **[InputText](#InputText)**
* **[Clear](#Clear)**

### Tab
```lua
Tab("TabName")
```

### RemoveTabs
```lua
RemoveTabs()
```

### GetItemsCount
```lua
tab = Tab("TabName")
log(tab:GetItemsCount())
```

### Button
```lua
tab = Tab("TabName")
tab:Button("its button" function() log("Hello") end)
```

### Checkbox
```lua
tab = Tab("TabName")
smthng = false
tab:Checkbox("Test", smthng)
```

### Spacing
```lua
tab = Tab("TabName")
smthng = false
tab:Button("its button" function() log("Hello") end)
tab:Spacing()
tab:Checkbox("Test", smthng)
```

### SameLine
```lua
tab = Tab("TabName")
smthng = false
tab:Button("its button" function() log("Hello") end)
tab:SameLine()
tab:Checkbox("Test", smthng)
```

### Text
```lua
tab = Tab("TabName")
tab:Text("Hi This is a text")
```

### InputText
```lua
tab = Tab("TabName")
test = 10
tab:Spacing()
tab:InputText("Hi This is a text", test)
```

### Clear
```lua
tab = Tab("TabName")
tab:Button("Clear Tab" tab:Clear())
```
