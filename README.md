local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()
local plrhead = game.Players.LocalPlayer.Character.Head


local uimain = library:CreateWindow("Super Power Tycoon")


local web = uimain:CreateFolder("Web Tycoon")


web:Button("Get Web",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Web"].Door["ActDoor"], 0)
end)

web:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Web"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

web:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Web"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

web:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Web"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

web:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Web"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local giant = uimain:CreateFolder("Giant Tycoon")


giant:Button("Get Giant",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Giant.Door["ActDoor"], 0)
end)

giant:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons.Giant.CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

giant:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons.Giant:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

giant:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons.Giant:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

giant:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons.Giant.Spawn.CFrame * CFrame.new(0,5,0)
end)



local stone = uimain:CreateFolder("Stone Tycoon")


stone:Button("Get Stone",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Stone.Door["ActDoor"], 0)
end)

stone:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Stone"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

stone:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Stone"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

stone:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Stone"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

stone:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Stone"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local robotic = uimain:CreateFolder("Robotic Tycoon")


robotic:Button("Get Robotic",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Robotic.Door["ActDoor"], 0)
end)

robotic:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Robotic"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

robotic:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Robotic"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

robotic:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Robotic"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

robotic:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Robotic"].Spawn.CFrame * CFrame.new(0,5,0)
end)


local insanity = uimain:CreateFolder("Insanity Tycoon")

insanity:Button("Get Insanity",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Insanity"].Door["ActDoor"], 0)
end)

insanity:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Insanity"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

insanity:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Insanity"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

insanity:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Insanity"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

insanity:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Insanity"].Spawn.CFrame * CFrame.new(0,5,0)
end)


local magic = uimain:CreateFolder("Magic Tycoon")

magic:Button("Get Magic",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Magic"].Door["ActDoor"], 0)
end)

magic:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Magic"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

magic:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Magic"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

magic:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Magic"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

magic:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Magic"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local strong = uimain:CreateFolder("Strong Tycoon")

strong:Button("Get Strong",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Strong"].Door["ActDoor"], 0)
end)

strong:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Strong"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

strong:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Strong"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

strong:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Strong"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

strong:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Strong"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local storm = uimain:CreateFolder("Storm Tycoon")


storm:Button("Get Storm",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Storm.Door["ActDoor"], 0)
end)


storm:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Storm"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

storm:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Storm"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

storm:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Storm"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

storm:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Storm"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local dark = uimain:CreateFolder("Dark Tycoon")


dark:Button("Get Dark",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Dark.Door["ActDoor"], 0)
end)

dark:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Dark"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

dark:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Dark"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

dark:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Dark"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

dark:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Dark"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local spike = uimain:CreateFolder("Spike Tycoon")


spike:Button("Get Tailed",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Spike.Door["ActDoor"], 0)
end)

spike:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Spike"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

spike:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Spike"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

spike:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Spike"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

spike:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Spike"].Spawn.CFrame * CFrame.new(0,5,0)
end)

local others = uimain:CreateFolder("Others")
others:Button("Get All Tools [LOADED!]",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

others:Label("Credit to Muzan QLTN",{
    TextSize = 20; -- Self Explaining
    TextColor = Color3.fromRGB(255,255,255); -- Self Explaining
    BgColor = Color3.fromRGB(69,69,69); -- Self Explaining
    
})
others:Label("(on youtube)",{
    TextSize = 20; -- Self Explaining
    TextColor = Color3.fromRGB(255,255,255); -- Self Explaining
    BgColor = Color3.fromRGB(69,69,69); -- Self Explaining
    
})
