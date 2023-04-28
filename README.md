local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "TTJY X Ruby hub Key system", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})




local Key = Window:MakeTab({
	Name = "Key",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local discord = Key:AddSection({
	Name = "Join discord server for Key https://discord.gg/YzRFEuAH"
})

_G.Key = "wjidiqwjoe3248tu8wijfw4igjwkmfjIJFWUIkaiJDIJEWGIOSOUQisojauihUHFufFHAUO"
_G.KeyInput = "string"
gayKeyforttjy = "TTJYX"



Key:AddTextbox({
	Name = "Key",
	Default = "",
	TextDisappear = true,
	Callback = function(Value)
	_G.KeyInput = Value
	end	  
})

Key:AddButton({
Name = "Check Key",
Callback = function()
if _G.KeyInput == _G.Key or gayKeyforttjy then
OrionLib:MakeNotification({
Name = "Key System",
Content = "Key Correct",
Image = "rbxassetid://4483345998",
Time = 5
})
loadstring(game:HttpGet('https://raw.githubusercontent.com/ttjy9808/ttjyXRUBYUNOBF/main/README.md'))()
task.wait(2)
OrionLib:Destroy()
else
OrionLib:MakeNotification({
Name = "Key System",
Content = "Wrong Key",
Image = "rbxassetid://4483345998",
Time = 5
})
end
end    
})
