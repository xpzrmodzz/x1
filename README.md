--create By FRITE--
while true do wait()
local args = {
    [1] = {
        ["multiply"] = 1,
        ["action"] = "hit",
        ["enemyHum"] = workspace.dummies.TrainingDummy1.Humanoid
    }
}

game:GetService("ReplicatedStorage").DamageEvent:FireServer(unpack(args))
end
