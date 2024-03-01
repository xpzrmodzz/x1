-- create By FRITE
while true do
    wait()
    
    local args1 = {
        [1] = {
            ["multiply"] = 1,
            ["action"] = "hit",
            ["enemyHum"] = workspace.dummies.TrainingDummy1.Humanoid
        }
    }

    game:GetService("ReplicatedStorage").DamageEvent:FireServer(unpack(args1))

    local args2 = {
        [1] = {
            ["multiply"] = 1,
            ["action"] = "damage",
            ["enemyChar"] = workspace.dummies.TrainingDummy1
        }
    }

    game:GetService("ReplicatedStorage").Events.WaterbeamEvent:FireServer(unpack(args2))
end
