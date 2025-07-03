local Players = game:GetService("Players")
local TweenService = game:GetService("TweenService")
local RunService = game:GetService("RunService")
local player = Players.LocalPlayer

local screenGui = Instance.new("ScreenGui", player:WaitForChild("PlayerGui"))
screenGui.Name = "TeleportUI"
screenGui.ResetOnSpawn = false

local mainFrame = Instance.new("Frame", screenGui)
mainFrame.Name = "MainUI"
mainFrame.Size = UDim2.new(0, 250, 0, 150)
mainFrame.Position = UDim2.new(0.05, 0, 0.05, 0)
mainFrame.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
mainFrame.BorderSizePixel = 0
mainFrame.Active = true
mainFrame.Draggable = true

local uiCorner = Instance.new("UICorner", mainFrame)
uiCorner.CornerRadius = UDim.new(0, 10)

local title = Instance.new("TextLabel", mainFrame)
title.Text = "Teleportador de Base"
title.Size = UDim2.new(1, 0, 0, 30)
title.Position = UDim2.new(0, 0, 0, 0)
title.BackgroundTransparency = 1
title.TextColor3 = Color3.new(1, 1, 1)
title.Font = Enum.Font.GothamBold
title.TextScaled = true

local toggle = Instance.new("TextButton", mainFrame)
toggle.Text = "Ativar"
toggle.Size = UDim2.new(0.4, 0, 0.2, 0)
toggle.Position = UDim2.new(0.05, 0, 0.5, 0)
toggle.BackgroundColor3 = Color3.fromRGB(60, 200, 60)
toggle.Font = Enum.Font.Gotham
toggle.TextScaled = true
toggle.TextColor3 = Color3.new(1, 1, 1)

local goButton = Instance.new("TextButton", mainFrame)
goButton.Text = "Ir para Base"
goButton.Size = UDim2.new(0.5, 0, 0.2, 0)
goButton.Position = UDim2.new(0.45, 0, 0.5, 0)
goButton.BackgroundColor3 = Color3.fromRGB(60, 120, 200)
goButton.Font = Enum.Font.Gotham
goButton.TextScaled = true
goButton.TextColor3 = Color3.new(1, 1, 1)

local ativo = true
toggle.MouseButton1Click:Connect(function()
	ativo = not ativo
	toggle.Text = ativo and "Ativar" or "Desativado"
	toggle.BackgroundColor3 = ativo and Color3.fromRGB(60, 200, 60) or Color3.fromRGB(200, 60, 60)
end)

local function moverSuavementeAteBase()
	if not ativo then return end

	local char = player.Character or player.CharacterAdded:Wait()
	local hrp = char:WaitForChild("HumanoidRootPart")

	local bases = workspace:FindFirstChild("Bases")
	if not bases then return end

	local base = bases:FindFirstChild(player.Name)
	if not base or not base:IsA("BasePart") then return end

	local destino = base.Position + Vector3.new(0, 5, 0)
	local tweenInfo = TweenInfo.new(2, Enum.EasingStyle.Quad, Enum.EasingDirection.Out)
	local objetivo = {Position = destino}
	local tween = TweenService:Create(hrp, tweenInfo, objetivo)
	tween:Play()
end

goButton.MouseButton1Click:Connect(moverSuavementeAteBase)

local function aplicarESPNoCorpo(jogador)
	if jogador == player then return end

	jogador.CharacterAdded:Connect(function(char)
		task.wait(1)
		for _, parte in pairs(char:GetChildren()) do
			if parte:IsA("BasePart") and parte.Name ~= "HumanoidRootPart" then
				local overlay = Instance.new("BoxHandleAdornment")
				overlay.Adornee = parte
				overlay.AlwaysOnTop = true
				overlay.ZIndex = 5
				overlay.Size = parte.Size
				overlay.Transparency = 0.7
				overlay.Color3 = Color3.fromRGB(255, 80, 80)
				overlay.Parent = parte
			end
		end
	end)
end

for _, p in pairs(Players:GetPlayers()) do
	aplicarESPNoCorpo(p)
end

Players.PlayerAdded:Connect(aplicarESPNoCorpo)
