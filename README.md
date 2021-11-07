-- Objects

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Credits = Instance.new("TextLabel")
local insaneall = Instance.new("TextButton")
local daball = Instance.new("TextButton")
local dabothers = Instance.new("TextButton")
local insaneothers = Instance.new("TextButton")

-- Properties

ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.Active = true
Frame.BackgroundColor3 = Color3.new(0, 0, 0)
Frame.BackgroundTransparency = 0.5
Frame.Draggable = true
Frame.Position = UDim2.new(0, 341, 0, 41)
Frame.Size = UDim2.new(0, 358, 0, 423)

Credits.Name = "Credits"
Credits.Parent = Frame
Credits.BackgroundColor3 = Color3.new(0, 0, 0)
Credits.BackgroundTransparency = 0.5
Credits.Position = UDim2.new(0, 79, 0, 0)
Credits.Size = UDim2.new(0, 200, 0, 50)
Credits.Font = Enum.Font.SciFi
Credits.FontSize = Enum.FontSize.Size24
Credits.Text = "By 0abidik"
Credits.TextColor3 = Color3.new(0, 1, 1)
Credits.TextSize = 24

insaneall.Name = "insaneall"
insaneall.Parent = Frame
insaneall.BackgroundColor3 = Color3.new(0, 0, 0)
insaneall.BackgroundTransparency = 0.5
insaneall.Position = UDim2.new(0, 0, 0, 106)
insaneall.Size = UDim2.new(0, 155, 0, 50)
insaneall.Font = Enum.Font.SciFi
insaneall.FontSize = Enum.FontSize.Size18
insaneall.Text = "Anti-Afk GUI"
insaneall.TextColor3 = Color3.new(0, 1, 1)
insaneall.TextSize = 18

daball.Name = "daball"
daball.Parent = Frame
daball.BackgroundColor3 = Color3.new(0, 0, 0)
daball.BackgroundTransparency = 0.5
daball.Position = UDim2.new(0, 0, 0, 228)
daball.Size = UDim2.new(0, 155, 0, 50)
daball.Font = Enum.Font.SciFi
daball.FontSize = Enum.FontSize.Size18
daball.Text = "Toggle E to Fly"
daball.TextColor3 = Color3.new(0, 1, 1)
daball.TextSize = 18



dabothers.Name = "dabothers"
dabothers.Parent = Frame
dabothers.BackgroundColor3 = Color3.new(0, 0, 0)
dabothers.BackgroundTransparency = 0.5
dabothers.Position = UDim2.new(0, 203, 0, 230)
dabothers.Size = UDim2.new(0, 155, 0, 50)
dabothers.Font = Enum.Font.SciFi
dabothers.FontSize = Enum.FontSize.Size18
dabothers.Text = "Speed = 100"
dabothers.TextColor3 = Color3.new(0, 1, 1)
dabothers.TextSize = 18

insaneothers.Name = "insaneothers"
insaneothers.Parent = Frame
insaneothers.BackgroundColor3 = Color3.new(0, 0, 0)
insaneothers.BackgroundTransparency = 0.5
insaneothers.Position = UDim2.new(0, 203, 0, 105)
insaneothers.Size = UDim2.new(0, 155, 0, 50)
insaneothers.Font = Enum.Font.SciFi
insaneothers.FontSize = Enum.FontSize.Size18
insaneothers.Text = "JumpPower = 100"
insaneothers.TextColor3 = Color3.new(0, 1, 1)
insaneothers.TextSize = 18

insaneall.MouseButton1Click:connect(function()
local vu = game:GetService("VirtualUser")
game.StarterGui:SetCore("SendNotification", {
		Title = "Anti Afk GUI";
		Text = "Anti Afk GUI Loaded. Tnx For Using Anti Afk GUI Made By:0abidik";
		Icon = "";
		Duration = 10;
	})

local ScreenGui = Instance.new("ScreenGui")
local main = Instance.new("Frame")
local AntiAfk = Instance.new("TextButton")
local Test = Instance.new("TextButton")



ScreenGui.Parent = game.CoreGui

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
main.BorderColor3 = Color3.fromRGB(45, 45, 45)
main.Position = UDim2.new(0.0616438352, 0, 0.686906993, 0)
main.Size = UDim2.new(0, 85, 0, 33)
main.Active = true
main.Draggable = true

AntiAfk.Name = "AntiAfk"
AntiAfk.Parent = main
AntiAfk.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
AntiAfk.Position = UDim2.new(0.137681156, 0, 0.136363626, 0)
AntiAfk.Size = UDim2.new(0, 62, 0, 24)
AntiAfk.Font = Enum.Font.Ubuntu
AntiAfk.Text = "AntiAfk"
AntiAfk.TextColor3 = Color3.fromRGB(0, 0, 0)
AntiAfk.TextSize = 14.000
AntiAfk.MouseButton1Down:connect(function()
	local vu = game:GetService("VirtualUser")
	game:GetService("Players").LocalPlayer.Idled:connect(function()
		vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
		wait(1)
		vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
        
	end)
end)
local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
   vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
   wait(1)
   vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)
AntiAfk.MouseButton1Down:connect(function()
	local vu = game:GetService("VirtualUser")
	game:GetService("Players").LocalPlayer.Idled:connect(function()
		vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
		wait(1)
		vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
        
	end)
end)
AntiAfk.MouseButton1Down:connect(function()
local vu = game:GetService("VirtualUser")
game.StarterGui:SetCore("SendNotification", {
		Title = "Anti Afk Gui";
		Text = "Anti Afk Loaded";
		Icon = "";
		Duration = 10;
	})

end)

end)
daball.MouseButton1Click:connect(function()
loadstring(game:HttpGet("https://pastebinp.com/raw/7rXZ9VNc", true))()

end)

insaneothers.MouseButton1Click:connect(function()
while true do
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 100
wait()
end

    

end)
dabothers.MouseButton1Click:connect(function()
while true do
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 100
wait()
end
end)
