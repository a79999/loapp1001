-- Criação da interface de administração

local Players = game:GetService("Players")
local StarterGui = game:GetService("StarterGui")
local player = Players.LocalPlayer

-- Criação do Frame principal
local screenGui = Instance.new("ScreenGui")
screenGui.Name = "AdminGUI"
screenGui.Parent = StarterGui

local mainFrame = Instance.new("Frame")
mainFrame.Size = UDim2.new(0.3, 0, 0.5, 0)
mainFrame.Position = UDim2.new(0.35, 0, 0.25, 0)
mainFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
mainFrame.Parent = screenGui

-- Título
local title = Instance.new("TextLabel")
title.Size = UDim2.new(1, 0, 0.2, 0)
title.Text = "Admin Options"
title.BackgroundColor3 = Color3.fromRGB(100, 100, 100)
title.TextColor3 = Color3.fromRGB(255, 255, 255)
title.Parent = mainFrame

-- Botão 1
local button1 = Instance.new("TextButton")
button1.Size = UDim2.new(0.8, 0, 0.2, 0)
button1.Position = UDim2.new(0.1, 0, 0.3, 0)
button1.Text = "Option 1"
button1.BackgroundColor3 = Color3.fromRGB(100, 100, 100)
button1.TextColor3 = Color3.fromRGB(255, 255, 255)
button1.Parent = mainFrame
button1.MouseButton1Click:Connect(function()
    print("Option 1 selected")
end)

-- Botão 2
local button2 = Instance.new("TextButton")
button2.Size = UDim2.new(0.8, 0, 0.2, 0)
button2.Position = UDim2.new(0.1, 0, 0.6, 0)
button2.Text = "Option 2"
button2.BackgroundColor3 = Color3.fromRGB(100, 100, 100)
button2.TextColor3 = Color3.fromRGB(255, 255, 255)
button2.Parent = mainFrame
button2.MouseButton1Click:Connect(function()
    print("Option 2 selected")
end)
