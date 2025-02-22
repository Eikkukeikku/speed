local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local speedBoost = 50 -- The amount to increase speed by
local normalSpeed = 16 -- Default walk speed

-- Function to toggle speed
local function toggleSpeed()
    if character.Humanoid.WalkSpeed == normalSpeed then
        character.Humanoid.WalkSpeed = normalSpeed + speedBoost
    else
        character.Humanoid.WalkSpeed = normalSpeed
    end
end

-- Bind the function to a key (e.g., "E")
local UserInputService = game:GetService("UserInputService")
UserInputService.InputBegan:Connect(function(input, gameProcessed)
    if input.KeyCode == Enum.KeyCode.E and not gameProcessed then
        toggleSpeed()
    end
end)
