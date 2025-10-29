                    end
            elseif not game:GetService("Workspace").Map:FindFirstChild("MysticIsland") or not game:GetService("Workspace").Map:FindFirstChild("MysticIsland") then
                Hop()
                end
            end
        end
    end)

    spawn(function()
        while wait() do
            if _G.Hopfindmoon then
            if game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709149052" or game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709149431" then
                wait(2.0)
                OrionLib:MakeNotification({
                    Name = "Sla Hub",
                    Content = "Turn Off Hop Find Moon Please",
                    Image = "rbxassetid://119980140458596",
                    Time = 5
                })
            elseif game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709143733" then
                Hop()
                OrionLib:MakeNotification({
                    Name = "Sla Hub",
                    Content = "Hop Server",
                    Image = "rbxassetid://119980140458596",
                    Time = 5
                })
            elseif game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709150401" then
                Hop()
                OrionLib:MakeNotification({
                    Name = "Sla Hub",
                    Content = "Hop Server",
                    Image = "rbxassetid://119980140458596",
                    Time = 5
                })
            elseif game:GetService("Lighting").Sky.MoonTextureId=="http://www.roblox.com/asset/?id=9709149680" then
                Hop()
                OrionLib:MakeNotification({
                    Name = "Sla Hub",
                    Content = "Hop Server",
                    Image = "rbxassetid://119980140458596",
                    Time = 5
                })
            else
                Hop()
                end
            end
        end
    end)

OrionLib:MakeNotification({
        Name = "Sla Hub",
        Content = "Loading script complete!, You can now enable the function!",
        Image = "rbxassetid://119980140458596",
        Time = 5
    })

_G.Remove_Effect = true

spawn(function()
    while wait() do
    for i,v in pairs(game.Players:GetPlayers()) do
        if v.Name == "red_game43" or v.Name == "rip_indra" or v.Name == "Axiore" or v.Name == "Polkster" or v.Name == "wenlocktoad" or v.Name == "Daigrock" or v.Name == "toilamvidamme" or v.Name == "oofficialnoobie" or v.Name == "Uzoth" or v.Name == "Azarth" or v.Name == "arlthmetic" or v.Name == "Death_King" or v.Name == "Lunoven" or v.Name == "TheGreateAced" or v.Name == "rip_fud" or v.Name == "drip_mama" or v.Name == "layandikit12" or v.Name == "Hingoi" then
            Hop()
            end
        end
    end
end)

spawn(function()
    game:GetService('RunService').Stepped:Connect(function()
        if _G.Remove_Effect then
            for i, v in pairs(game:GetService("ReplicatedStorage").Effect.Container:GetChildren()) do
                if v.Name == "Death" then
                    v:Destroy() 
                end
            end
        end
    end)
end)

spawn(function()
    while wait() do
        for i,v in pairs(game.Players.LocalPlayer:GetChildren()) do
            if v.Name == "DataLoaded" or v.Name == "DataPreloaded" then
                v:Destroy()
            end
        end
    end
end)

OrionLib:Init()

OrionLib:MakeNotification({
    Name = "Sla Hub",
    Content = "Loading Config Complete!!",
    Image = "rbxassetid://119980140458596",
    Time = 5
})
