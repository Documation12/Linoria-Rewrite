# Linoria Documantion
## Libary Startup
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Documation12/Linoria-Rewrite/main/Libary.lua",true))()
local ThemeManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/Documation12/Linoria-Rewrite/main/Addons/Thememanager.lua",true))()
local SaveManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/Documation12/Linoria-Rewrite/main/Addons/SaveManager.lua",true))()
```
## Window Creation
```lua
local Window = Library:CreateWindow({
  Title = 'Example menu',
	Center = true,
	AutoShow = true,
	Resizable = true,
	ShowCustomCursor = false, 
	TabPadding = 8,
	MenuFadeTime = 0.2
})
```
## Creating Tabs
```lua
local Tabs = {
    Main = Window:AddTab('Example'), 
    ['UI Settings'] = Window:AddTab('Settings'), 
}
-- Or local Main = Window:AddTab('Example')
```
## Group box
#### Left Groupbox
```lua
local LGroupBox = Tabs.Main:AddLeftGroupbox('Example') -- Main to the tab name
```
#### Right Group Box
```lua
local RGroupBox = Tabs.Main:AddRightGroupbox('Example') -- Main to the tab name
```
## Buttons
```lua
local MyButton = Main:AddButton('Name', function()
    print('You clicked a button!')
end)
```
```lua
local MySubButton = Mybutton:AddButton('NameSub', function()
    print('You clicked a Sub button!')
end)
```
## Toggle
```lua

```
