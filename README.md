local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Drag, Qura W Phyt", "DarkTheme")
    -- MAIN
    local Main = Window:NewTab("Main")
    local MainSection = Main:NewSection("Main")

local AnimationCurveLoop

MainSection:NewToggle("DRAG", "drag atabilmeni saglar", function(arg)
if arg then
game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.WoodenFloor.Tick.Visible = true
    game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.WoodenFloor.WoodenFloor.Style = "RobloxRoundButton"

local Humanoid = game.Players.LocalPlayer.Character.Humanoid

AnimationCurveLoop = Humanoid.AnimationPlayed:Connect(function(AnimationTrack)
    if AnimationTrack.Name == "OldMKickL" or AnimationTrack.Name == "OldMKick" or AnimationTrack.Name == "OldLKickL" or AnimationTrack.Name == "OldLKick" or AnimationTrack.Name == "MKickL" or AnimationTrack.Name == "MKick" or AnimationTrack.Name == "LKickL" or AnimationTrack.Name == "LKick" or AnimationTrack.Name == "OldDribbleL" or AnimationTrack.Name == "OldDribble" or AnimationTrack.Name == "DribbleL" or AnimationTrack.Name == "Dribble" then
    if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - game.Workspace.TPSSystem.TPS.Position).Magnitude < 300.4500 then
        if game.Players.LocalPlayer.Backpack.Curving.Value == 2 then
        wait(0.1)
                local A_1T = game:GetService("Workspace").TPSSystem.TPS
local A_2T = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
local EventT = game:GetService("Workspace").FE.Actions.KickC1
EventT:FireServer(A_1T, A_2T)
wait(0.2)
EventT:FireServer(A_1T, A_2T)

elseif game.Players.LocalPlayer.Backpack.Curving.Value == 1 then
wait(0.1)
local A_1 = game:GetService("Workspace").TPSSystem.TPS
local A_2 = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
local Event = game:GetService("Workspace").FE.Actions.KickC2
Event:FireServer(A_1, A_2)
wait(0.2)
Event:FireServer(A_1, A_2)

            end
        end
    end
end)
    else
        AnimationCurveLoop:Disconnect()
        game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.WoodenFloor.Tick.Visible = false
    game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.WoodenFloor.WoodenFloor.Style = "RobloxRoundDefaultButton"
    end
end)
