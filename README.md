# MakoMermaids-V.1
This Script

local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

local Window = Library.CreateLib("Mako Mermaids OP SCRIPT", "Ocean")


local Characters = Window:NewTab("Mermaids")

local Coins = Characters:NewSection("Coins Character")

Coins:NewButton("Sirena", "pick", function()
   local args = {
    [1] = "Outfit1",
    [2] = "Sirena"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))

end)

Coins:NewButton("Aquata", "pick", function()
   local args = {
    [1] = "Outfit1",
    [2] = "Aquata"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))

end)


local Weilan = Characters:NewSection("Weilan / GAMEPASS ONLY")

Weilan:NewButton("Outfit1", "WARNING IF YOU PRESS YOU WILL KICK", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Weilan"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

Weilan:NewButton("Outfit2", "WARNING IF YOU PRESS YOU WILL KICK", function()
    local args = {
    [1] = "Outfit2",
    [2] = "Weilan"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

local Mimi = Characters:NewSection("Mimi / GAMEPASS ONLY")

Mimi:NewButton("Outfit1", "WARNING IF YOU PRESS YOU WILL KICK", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Mimi"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

Mimi:NewButton("Outfit2", "WARNING IF YOU PRESS YOU WILL KICK", function()
    local args = {
    [1] = "Outfit2",
    [2] = "Mimi"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

local Ondina = Characters:NewSection("Ondina / GAMEPASS ONLY")

Ondina:NewButton("Outfit1", "WARNING IF YOU PRESS YOU WILL KICK", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Ondina"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

Ondina:NewButton("Outfit2", "WARNING IF YOU PRESS YOU WILL KICK", function()
    local args = {
    [1] = "Outfit2",
    [2] = "Ondina"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

local SirenSirena = Characters:NewSection("Siren Sirena / GAMEPASS ONLY")

SirenSirena:NewButton("Outfit1", "WARNING IF YOU PRESS YOU WILL KICK", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Siren Sirena"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

local FreeChar = Characters:NewSection("Free Chars")

FreeChar:NewButton("Nixie", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Nixie"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

FreeChar:NewButton("Lyla", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Lyla"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)


----- MERMANS

local Characters = Window:NewTab("Mermans")

local Merman = Characters:NewSection("Mermans")

Merman:NewButton("Zac", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Zac"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

Merman:NewButton("Erik", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Erik"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)


---- HUMANS

local Characters = Window:NewTab("Humans")

local Humans = Characters:NewSection("Mermans")

Humans:NewButton("Cam", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Cam"
}

Humans:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

Humans:NewButton("Evie", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Evie"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

Humans:NewButton("Carly", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Carly"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)

Humans:NewButton("Will", "Pick", function()
    local args = {
    [1] = "Outfit1",
    [2] = "Will"
}

game:GetService("ReplicatedStorage").System_Remotes.CharacterChoose:FireServer(unpack(args))
end)


local Characters = Window:NewTab("Characters Unlocker")

local item = Characters:NewSection("Unlock")

item:NewButton("Aquata","Unlocking Char", function()
local args = {
    [1] = "Aquata",
    [2] = game:GetService("Players").LocalPlayer.Cash
}

game:GetService("ReplicatedStorage").System_Remotes.CharPurchase:FireServer(unpack(args))

end)

item:NewButton("Sirena","Unlocking Char", function()
local args = {
    [1] = "Sirena",
    [2] = game:GetService("Players").LocalPlayer.Cash
}

game:GetService("ReplicatedStorage").System_Remotes.CharPurchase:FireServer(unpack(args))

end)


local Powers = Window:NewTab("Abilities")

local item = Powers:NewSection("COMING SOON!")

local Ui = Window:NewTab("ToggleUi")

local Toggle = Ui:NewSection("Settings")

Toggle:NewKeybind("KeybindText", "KeybindInfo", Enum.KeyCode.Zero, function()
	Library:ToggleUI()
end)


if game.PlaceId == 12596301000 then
    Script()
end
