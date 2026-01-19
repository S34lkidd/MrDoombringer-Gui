-- Gui to Lua

-- Version: 3.2



-- Instances:



local ScreenGui = Instance.new("ScreenGui")

local TextLabel = Instance.new("TextLabel")

local Frame = Instance.new("Frame")

local TextButton = Instance.new("TextButton")

local TextButton_2 = Instance.new("TextButton")

local TextButton_3 = Instance.new("TextButton")

local TextButton_4 = Instance.new("TextButton")

local TextLabel_2 = Instance.new("TextLabel")



--Properties:



ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling



TextLabel.Parent = ScreenGui

TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)

TextLabel.Position = UDim2.new(0.177758202, 0, 0.245322242, 0)

TextLabel.Size = UDim2.new(0, 167, 0, 22)

TextLabel.Font = Enum.Font.SourceSans

TextLabel.Text = "MrDoombringer Simple Gui"

TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)

TextLabel.TextSize = 14.000



Frame.Parent = TextLabel

Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

Frame.BorderColor3 = Color3.fromRGB(0, 0, 0)

Frame.Position = UDim2.new(0, 0, 1, 0)

Frame.Size = UDim2.new(0, 167, 0, 264)



TextButton.Parent = Frame

TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextButton.BorderColor3 = Color3.fromRGB(0, 0, 0)

TextButton.Position = UDim2.new(0.0898203626, 0, 0.0456852801, 0)

TextButton.Size = UDim2.new(0, 136, 0, 40)

TextButton.Font = Enum.Font.SourceSans

TextButton.Text = "Shedletsy"

TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)

TextButton.TextSize = 14.000



TextButton_2.Parent = Frame

TextButton_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextButton_2.BorderColor3 = Color3.fromRGB(0, 0, 0)

TextButton_2.Position = UDim2.new(0.0838323385, 0, 0.226157561, 0)

TextButton_2.Size = UDim2.new(0, 136, 0, 40)

TextButton_2.Font = Enum.Font.SourceSans

TextButton_2.Text = "Skybox"

TextButton_2.TextColor3 = Color3.fromRGB(0, 0, 0)

TextButton_2.TextSize = 14.000



TextButton_3.Parent = Frame

TextButton_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextButton_3.BorderColor3 = Color3.fromRGB(0, 0, 0)

TextButton_3.Position = UDim2.new(0.0838323385, 0, 0.423069566, 0)

TextButton_3.Size = UDim2.new(0, 136, 0, 40)

TextButton_3.Font = Enum.Font.SourceSans

TextButton_3.Text = "Decal"

TextButton_3.TextColor3 = Color3.fromRGB(0, 0, 0)

TextButton_3.TextSize = 14.000



TextButton_4.Parent = Frame

TextButton_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextButton_4.BorderColor3 = Color3.fromRGB(0, 0, 0)

TextButton_4.Position = UDim2.new(0.0780239478, 0, 0.608563066, 0)

TextButton_4.Size = UDim2.new(0, 136, 0, 40)

TextButton_4.Font = Enum.Font.SourceSans

TextButton_4.Text = "Theme"

TextButton_4.TextColor3 = Color3.fromRGB(0, 0, 0)

TextButton_4.TextSize = 14.000



TextLabel_2.Parent = Frame

TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextLabel_2.BorderColor3 = Color3.fromRGB(0, 0, 0)

TextLabel_2.Position = UDim2.new(0, 0, 0.810606062, 0)

TextLabel_2.Size = UDim2.new(0, 167, 0, 50)

TextLabel_2.Font = Enum.Font.SourceSans

TextLabel_2.Text = "Gui by GoldFishMaster687"

TextLabel_2.TextColor3 = Color3.fromRGB(0, 0, 0)

TextLabel_2.TextSize = 14.000



-- Scripts:



local function NKYXQC_fake_script() -- TextLabel.LocalScript 

	local script = Instance.new('LocalScript', TextLabel)



	script.Parent.Selectable = true

	script.Parent.Active = true

	script.Parent.Draggable = true

	

end

coroutine.wrap(NKYXQC_fake_script)()

local function XBYJJW_fake_script() -- TextButton.Script 

	local script = Instance.new('Script', TextButton)



	script.Parent.MouseButton1Down:Connect(function()

		for _, obj in pairs(workspace:GetDescendants()) do

			if obj:IsA("BasePart") then

				local particle = Instance.new("ParticleEmitter")

				particle.Texture = "rbxassetid://14793262780" -- your id is here

				particle.Rate = 20

				particle.Lifetime = NumberRange.new(2, 5)

				particle.Speed = NumberRange.new(3, 7)

				particle.Parent = obj

				particle.SpreadAngle = Vector2.new(360, 360)

			end

		end

	end)

end

coroutine.wrap(XBYJJW_fake_script)()

local function RFWER_fake_script() -- TextButton_2.Script 

	local script = Instance.new('Script', TextButton_2)



	function click()

		s = Instance.new("Sky")

		s.Name = "Sky"

		s.Parent = game.Lighting

		s.SkyboxBk = "rbxassetid://172423468"--the id is here 

		s.SkyboxDn = "rbxassetid://172423468"--the id is here 

		s.SkyboxFt = "rbxassetid://172423468"--the id is here

		s.SkyboxLf = "rbxassetid://172423468"--the id is here 

		s.SkyboxRt = "rbxassetid://172423468"--the id is here 

		s.SkyboxUp = "rbxassetid://172423468"--the id is here 

		game.Lighting.TimeOfDay = 12

	end

	

	script.Parent.MouseButton1Down:connect(click)

	

end

coroutine.wrap(RFWER_fake_script)()

local function JTFA_fake_script() -- TextButton_3.Script 

	local script = Instance.new('Script', TextButton_3)



	function click()

		function exPro(root)

			for _, v in pairs(root:GetChildren()) do

				if v:IsA("Decal") and v.Texture ~= "rbxassetid://95923731769358" then

					v.Parent = nil

				elseif v:IsA("BasePart") then

					v.Material = "Plastic"

					v.Transparency = 0

					local One = Instance.new("Decal", v)

					local Two = Instance.new("Decal", v)

					local Three = Instance.new("Decal", v)

					local Four = Instance.new("Decal", v)

					local Five = Instance.new("Decal", v)

					local Six = Instance.new("Decal", v)

					One.Texture = "rbxassetid://95923731769358"

					Two.Texture = "rbxassetid://95923731769358"

					Three.Texture = "rbxassetid://95923731769358"

					Four.Texture = "rbxassetid://95923731769358"

					Five.Texture = "rbxassetid://95923731769358"

					Six.Texture = "rbxassetid://95923731769358"--put id in here i will put it in description

					One.Face = "Front"

					Two.Face = "Back"

					Three.Face = "Right"

					Four.Face = "Left"

					Five.Face = "Top"

					Six.Face = "Bottom"

				end

				exPro(v)

			end

		end

		function asdf(root)

			for _, v in pairs(root:GetChildren()) do

				asdf(v)

			end

		end

		exPro(game.Workspace)

		asdf(game.Workspace)

	end

	

	script.Parent.MouseButton1Down:connect(click)

	

end

coroutine.wrap(JTFA_fake_script)()

local function FOQYN_fake_script() -- TextButton_4.Script 

	local script = Instance.new('Script', TextButton_4)



	function click()

		Spooky = Instance.new("Sound", workspace)

		Spooky.Name = "Spooky"

		Spooky.SoundId = "rbxassetid://6070263388"

		Spooky.Volume = 1500

		Spooky.PlaybackSpeed = 1

		Spooky.Looped = true

		Spooky:Play()

	end

	

	script.Parent.MouseButton1Down:connect(click)

end

coroutine.wrap(FOQYN_fake_script)()

