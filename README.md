--No example for this one, It's worth it though if you take the time to use this!
--Wolfscript without key by matz#5555

local Lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/bloodball/-back-ups-for-libs/main/modern"))()
local uis = game:GetService("UserInputService")
local rp = game:GetService("ReplicatedStorage")
local count = 0

 local ExampleTab = Lib:Tab("Animal Simulator")
ExampleTab:Button(
    "ZoneBypass",
    function()
	game:GetService("Workspace")[game.Players.LocalPlayer.Name].FreeShield:Destroy()
        game:GetService("Workspace").Baseplate:Destroy()
	game:GetService("Workspace").SafeZonePart:Destroy()
    end
)

ExampleTab:Button(
    "BreakMorph",
    function()
	game:GetService("Workspace")[game.Players.LocalPlayer.Name].LowerTorso:Destroy()
    end
)

ExampleTab:Button(
    "FightOnFarming",
    function()
	if (uis:GetFocusedTextBox()) then
            return -- make sure player's not chatting!
        end
        if input.KeyCode == Enum.KeyCode.Q then
		for i,v in pairs(game.Players:GetChildren()) do
   			for i,p in pairs(game.Workspace:GetChildren()) do
   				if p.Name == v.Name and p.Name ~= game.Players.LocalPlayer.Name then
   					game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(p.Humanoid,5)
   				end
   			end
  		end
        end
    end
)





ExampleTab:Button(
    "DisableClick",
    function()
	game:GetService("Workspace")[game.Players.LocalPlayer.Name].ClickDetector:Destroy()
    end
)


ExampleTab:Button(
    "RemoveTag",
    function()
	game:GetService("Workspace")[game.Players.LocalPlayer.Name].Head.BillboardGui:Destroy()
    end
)


ExampleTab:Button(
    "RadioGUI",
    function()
	local clone = game:GetService("Workspace")["DRadio_Script"].DRadio_Gui:Clone()
	clone.Parent = game.Players.LocalPlayer.PlayerGui
    end
)

ExampleTab:Label("ExampleLabel", "Play Radio")
ExampleTab:TextBox(
    "radio id here",
    function(text)
        print(text)
        game:GetService("Workspace")["DRadio_Script"].Event:FireServer(text)
    end
)

ExampleTab:Label("ExampleLabel", "NickName")
ExampleTab:TextBox(
    "nickname here",
    function(text)
        print(text)
        local A_1 = text
	local Event = game:GetService("Players")[game.Players.LocalPlayer.Name].PlayerGui.RolePlayName.Frame.submitBtn.nameEvent
	Event:FireServer(A_1)
    end
)

ExampleTab:Label("ExampleLabel", "RideForce")
ExampleTab:TextBox(
    "nickname here",
    function(text)
        print(text)
        for i,v in pairs(game.Players:GetChildren()) do
        	if string.find(v.Name, text) then
      			game:GetService("ReplicatedStorage").RideEvents.acceptEvent:FireServer(v.Name)
      		end
  	end
    end
)




        



ExampleTab:Label("ExampleLabel", "PackJoin")
ExampleTab:TextBox(
    "packname here",
    function(text)
        print(text)

        	local A_1 = text
		local Event = game:GetService("ReplicatedStorage").acceptedEvent
		Event:FireServer(A_1)


    end
)






ExampleTab:Toggle(
    "Autofarm-KILL",
    function(state)
        if state then
            PrintToggle = true
            while PrintToggle do
                local args = {
                    [1] = workspace.Eggs.Egg7
                }

                game:GetService("ReplicatedStorage").EggEvent:FireServer(unpack(args))
                game:GetService("ReplicatedStorage").EggEvent:FireServer(unpack(args))

                local args = {
                    [1] = workspace.Treasures.Treasure1
                }

                game:GetService("ReplicatedStorage").TreasureEvent:FireServer(unpack(args))
                game:GetService("ReplicatedStorage").TreasureEvent:FireServer(unpack(args))
                count = count + 1
                if count > 600 then
                    count = 0
                    game.Players.LocalPlayer.Character.Humanoid.Health = 0
                end

                wait(0.1)
                wait()
            end
        else
            PrintToggle = false
            count = 0
        end
    end
)




ExampleTab:Toggle(
    "Autofarm-KILLdebug",
    function(state)
        if state then
            PrintToggle55 = true
            while PrintToggle55 do



local A_1 = game:GetService("Workspace").Treasures.Treasure4

local Event = game:GetService("ReplicatedStorage").TreasureEvent

Event:FireServer(A_1)


		if game:GetService("Workspace")[game.Players.LocalPlayer.Name]:FindFirstChild("justFound") ~= nil then
			game:GetService("Workspace")[game.Players.LocalPlayer.Name].justFound:Destroy()
   		end




               local A_1 = game:GetService("Workspace").Treasures.Treasure1

local Event = game:GetService("ReplicatedStorage").TreasureEvent

Event:FireServer(A_1)


		if game:GetService("Workspace")[game.Players.LocalPlayer.Name]:FindFirstChild("justFound") ~= nil then
			game:GetService("Workspace")[game.Players.LocalPlayer.Name].justFound:Destroy()
   		end


                count = count + 1
                if count > 2400 then
                    count = 0
                    game.Players.LocalPlayer.Character.Humanoid.Health = 0
                end

                wait(0.1)
                wait()
            end
        else
            PrintToggle55 = false
            count = 0
        end
    end
)



ExampleTab:Toggle(
    "Autofarm-debug",
    function(state)
        if state then
            PrintToggle555 = true
            while PrintToggle555 do
                local A_1 = game:GetService("Workspace").Treasures.Treasure4

local Event = game:GetService("ReplicatedStorage").TreasureEvent

Event:FireServer(A_1)


		if game:GetService("Workspace")[game.Players.LocalPlayer.Name]:FindFirstChild("justFound") ~= nil then
			game:GetService("Workspace")[game.Players.LocalPlayer.Name].justFound:Destroy()
   		end




               local A_1 = game:GetService("Workspace").Treasures.Treasure1

local Event = game:GetService("ReplicatedStorage").TreasureEvent

Event:FireServer(A_1)


		if game:GetService("Workspace")[game.Players.LocalPlayer.Name]:FindFirstChild("justFound") ~= nil then
			game:GetService("Workspace")[game.Players.LocalPlayer.Name].justFound:Destroy()
   		end

                wait()
            end
        else
            PrintToggle555 = false
        end
    end
)



ExampleTab:Toggle(
    "Autofarm-for60k",
    function(state)
        if state then
            PrintToggle5555 = true
            game:GetService("Workspace")[game.Players.LocalPlayer.Name].HumanoidRootPart.CFrame = game:GetService("Workspace").OLDMAP.pleaseno["Dummy2"].HumanoidRootPart.CFrame
            playercframe = game:GetService("Workspace")[game.Players.LocalPlayer.Name].HumanoidRootPart.CFrame
            while PrintToggle5555 do

		local A_1 = game:GetService("Workspace").Treasures.Treasure1
		local Event = game:GetService("ReplicatedStorage").TreasureEvent
		Event:FireServer(A_1)


		if game:GetService("Workspace")[game.Players.LocalPlayer.Name]:FindFirstChild("justFound") ~= nil then
			game:GetService("Workspace")[game.Players.LocalPlayer.Name].justFound:Destroy()
   		end

		game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(game:GetService("Workspace").OLDMAP.pleaseno["Dummy2"].Humanoid,5)

                wait()
            end
        else
            PrintToggle5555 = false
        end
    end
)


ExampleTab:Toggle(
    "Dummy farm",
    function(state)
        if state then
            PrintToggle5555 = true
            game:GetService("Workspace")[game.Players.LocalPlayer.Name].HumanoidRootPart.CFrame = game:GetService("Workspace").OLDMAP.pleaseno["Training Dummy"].HumanoidRootPart.CFrame
            playercframe = game:GetService("Workspace")[game.Players.LocalPlayer.Name].HumanoidRootPart.CFrame
            while PrintToggle5555 do

		game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(game:GetService("Workspace").OLDMAP.pleaseno["Training Dummy"].Humanoid,5)

                wait(0.1)
            end
        else
            PrintToggle5555 = false
        end
    end
)

ExampleTab:Toggle(
    "DamageIndicator",
    function(state)
        if state then
            PrintToggle55551 = true
            while PrintToggle55551 do
		for i,v in pairs(game.Players:GetChildren()) do
   			for i,p in pairs(game.Workspace:GetChildren()) do
   				if p.Name == v.Name and p.Name ~= game.Players.LocalPlayer.Name then
					if p:FindFirstChild("HumanoidRootPart") ~= nil then
   						if p.HumanoidRootPart:FindFirstChild("DmgIndicator") ~= nil then
							p.HumanoidRootPart.DmgIndicator:Destroy()
   						end
					end
   				end
   			end
  		end
		wait(0.01)
            end
        else
            PrintToggle55551 = false
        end
    end
)


ExampleTab:Toggle(
    "Autofarm-for60k-KILL",
    function(state)
        if state then
            PrintToggle556 = true
            game:GetService("Workspace")[game.Players.LocalPlayer.Name].HumanoidRootPart.CFrame = game:GetService("Workspace").OLDMAP.pleaseno["Dummy2"].HumanoidRootPart.CFrame
            playercframe = game:GetService("Workspace")[game.Players.LocalPlayer.Name].HumanoidRootPart.CFrame
            while PrintToggle556 do



		local A_1 = game:GetService("Workspace").Treasures.Treasure1
		local Event = game:GetService("ReplicatedStorage").TreasureEvent
		Event:FireServer(A_1)


		if game:GetService("Workspace")[game.Players.LocalPlayer.Name]:FindFirstChild("justFound") ~= nil then
			game:GetService("Workspace")[game.Players.LocalPlayer.Name].justFound:Destroy()
   		end

		game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(game:GetService("Workspace").OLDMAP.pleaseno["Dummy2"].Humanoid,5)


                count = count + 1
                if count > 2400 then
                    count = 0
                    game.Players.LocalPlayer.Character.Humanoid.Health = 0
                end

                wait(0.1)
                wait()
            end
        else
            PrintToggle556 = false
            count = 0
        end
    end
)





ExampleTab:Toggle(
    "SpamHowl",
    function(state)
        if state then
            PrintToggle2 = true
            while PrintToggle2 do
                local A_1 = 2
                wait(0.3)
                game:GetService("ReplicatedStorage").WolfHowlEvent:FireServer(A_1)
                wait(0.3)
                game:GetService("Workspace")[game.Players.LocalPlayer.Name].onHowl:Destroy()
            end
        else
            PrintToggle2 = false
        end
    end
)

ExampleTab:Toggle(
    "KillSlayer",
    function(state)
        if state then
            PrintToggle3 = true
            while PrintToggle3 do
		wait(0.1)
		if game:GetService("Workspace").NPC:FindFirstChild("DragonSlayer") then
			game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(game:GetService("Workspace").NPC['DragonSlayer'].Humanoid, 5)
		end
		wait(0.1)
            end
        else
            PrintToggle3 = false
        end
    end
)

ExampleTab:Toggle(
    "KillDrake",
    function(state)
        if state then
            PrintToggle4 = true
            while PrintToggle4 do
		wait(0.1)
		if game:GetService("Workspace").NPC:FindFirstChild("Drake") then
			game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(game:GetService("Workspace").NPC['Drake'].Humanoid, 5)
		end
		wait(0.1)
            end
        else
            PrintToggle4 = false
        end
    end
)

ExampleTab:Toggle(
    "KillLavaGorilla",
    function(state)
        if state then
            PrintToggle11 = true
            while PrintToggle11 do
		wait(0.1)
		if game:GetService("Workspace").NPC:FindFirstChild("LavaGorilla") then
			game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(game:GetService("Workspace").NPC['LavaGorilla'].Humanoid, 5)
		end
		wait(0.1)
            end
        else
            PrintToggle11 = false
        end
    end
)

ExampleTab:Toggle(
    "KillTrex",
    function(state)
        if state then
            PrintToggle12 = true
            while PrintToggle12 do
		wait(0.1)
		if game:GetService("Workspace").NPC:FindFirstChild("Trex") then
			game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(game:GetService("Workspace").NPC['Trex'].Humanoid, 5)
		end
		wait(0.1)
            end
        else
            PrintToggle12 = false
        end
    end
)

ExampleTab:Toggle(
    "PlayerKill",
    function(state)
        if state then
            PrintToggle5 = true
            while PrintToggle5 do
		wait(0.1)
  		for i,v in pairs(game.Players:GetChildren()) do
   			for i,p in pairs(game.Workspace:GetChildren()) do
   				if p.Name == v.Name and p.Name ~= game.Players.LocalPlayer.Name then
   					game:GetService("ReplicatedStorage").jdskhfsIIIllliiIIIdchgdIiIIIlIlIli:FireServer(p.Humanoid,5)
   				end
   			end
  		end
		wait(0.1)
            end
        else
            PrintToggle5 = false
        end
    end
)


ExampleTab:Toggle(
    "Autofarm",
    function(state)
        if state then
            PrintToggle7 = true
            while PrintToggle7 do
                local args = {
                    [1] = workspace.Eggs.Egg7
                }

                game:GetService("ReplicatedStorage").EggEvent:FireServer(unpack(args))
                game:GetService("ReplicatedStorage").EggEvent:FireServer(unpack(args))

                local args = {
                    [1] = workspace.Treasures.Treasure1
                }

                game:GetService("ReplicatedStorage").TreasureEvent:FireServer(unpack(args))
                game:GetService("ReplicatedStorage").TreasureEvent:FireServer(unpack(args))

                wait(0.1)
                wait()
            end
        else
            PrintToggle7 = false
        end
    end
)


ExampleTab:Toggle(
    "FastDamage",
    function(state)
        if state then
            PrintToggle8 = true
            while PrintToggle8 do
		if game:GetService("Workspace")[game.Players.LocalPlayer.Name]:FindFirstChild("Deb") then
			game:GetService("Workspace")[game.Players.LocalPlayer.Name].Deb:Destroy()
		end
                wait()
            end
        else
            PrintToggle8 = false
        end
    end
)




ExampleTab:DropDown(
    "More",
    {"Fireballs", "CLICKTP", "ANTIAFK", "ANTIKICK", "DEX", "AUDIOGRABBER", "REMOTESPY", "MSGSPY", "Newbies", "ServerHop"},
    function(text)
        if text == "Fireballs" then
	    Players = game:GetService("Players")
            mouse = game.Players.LocalPlayer:GetMouse()
            tool = Instance.new("Tool")
            tool.RequiresHandle = false
            tool.Name = "FIREBALL"
            tool.Activated:connect(
                function()
                    -- Script generated by R2Sv2
                    -- R2Sv2 developed by Luckyxero

                    for i, v in pairs(game.Workspace:GetDescendants()) do
                        if v:FindFirstChild("Fireball") then
                            if v:FindFirstChild("Fireball") then
                                pos = Vector3.new(mouse.Hit.Position.X, mouse.Hit.Position.Y, mouse.Hit.Z)
                                local Event = v["Fireball"].FireballEvent
                                Event:FireServer(pos)
                            end
                        end
                    end
                end
            )
            tool.Parent = game.Players.LocalPlayer.Backpack

            tool = Instance.new("Tool")
            tool.RequiresHandle = false
            tool.Name = "LIGNINGBALL"
            tool.Activated:connect(
                function()
                    for i, v in pairs(game.Workspace:GetDescendants()) do
                        if v:FindFirstChild("Lightningball") then
                            if v:FindFirstChild("Lightningball") then
                                pos = Vector3.new(mouse.Hit.Position.X, mouse.Hit.Position.Y, mouse.Hit.Z)
                                local Event = v["Lightningball"].FireballEvent
                                Event:FireServer(pos)
                            end
                        end
                    end
                end
            )
            tool.Parent = game.Players.LocalPlayer.Backpack




            tool = Instance.new("Tool")
            tool.RequiresHandle = false
            tool.Name = "LIGNINGBALLANTI"
            tool.Activated:connect(
                function()
                    for i, v in pairs(game.Workspace:GetDescendants()) do
                        if v:FindFirstChild("Lightningball") then
                            if v:FindFirstChild("Lightningball") then
                                 pos = Vector3.new(mouse.Hit.Position.X, mouse.Hit.Position.Y, mouse.Hit.Z)
                                local Event = game.Players[v.Name].Backpack["Lightningball"].FireballEvent
                                Event:FireServer(pos)

                            end
                        end
                    end
                end
            )
            tool.Parent = game.Players.LocalPlayer.Backpack


            tool = Instance.new("Tool")
            tool.RequiresHandle = false
            tool.Name = "FireballANTI"
            tool.Activated:connect(
                function()
                    for i, v in pairs(Players:GetPlayers()) do
                        if v:FindFirstChild("Fireball") then
                            if v:FindFirstChild("Fireball") then
                                pos = Vector3.new(mouse.Hit.Position.X, mouse.Hit.Position.Y, mouse.Hit.Z)
                                local Event = game.Players[v.Name].Backpack["Fireball"].FireballEvent
                                Event:FireServer(pos)

                            end
                        end
                    end
                end
            )
            tool.Parent = game.Players.LocalPlayer.Backpack






        elseif text == "CLICKTP" then
            mouse = game.Players.LocalPlayer:GetMouse()
            tool = Instance.new("Tool")
            tool.RequiresHandle = false
            tool.Name = "Click Teleport"
            tool.Activated:connect(
                function()
                    local pos = mouse.Hit + Vector3.new(0, 2.5, 0)
                    pos = CFrame.new(pos.X, pos.Y, pos.Z)
                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = pos
                end
            )
            tool.Parent = game.Players.LocalPlayer.Backpack
        elseif text == "ANTIAFK" then
            loadstring(game:HttpGet(("https://raw.githubusercontent.com/Proxylol/OtherScripts/main/AntiAfk.lua"), true))(

            )
        elseif text == "ServerHop" then
            local PlaceID = game.PlaceId
            local AllIDs = {}
            local foundAnything = ""
            local actualHour = os.date("!*t").hour
            local Deleted = false
            local File =
                pcall(
                function()
                    AllIDs = game:GetService("HttpService"):JSONDecode(readfile("NotSameServers.json"))
                end
            )
            if not File then
                table.insert(AllIDs, actualHour)
                writefile("NotSameServers.json", game:GetService("HttpService"):JSONEncode(AllIDs))
            end
            function TPReturner()
                local Site
                if foundAnything == "" then
                    Site =
                        game.HttpService:JSONDecode(
                        game:HttpGet(
                            "https://games.roblox.com/v1/games/" .. PlaceID .. "/servers/Public?sortOrder=Asc&limit=100"
                        )
                    )
                else
                    Site =
                        game.HttpService:JSONDecode(
                        game:HttpGet(
                            "https://games.roblox.com/v1/games/" ..
                                PlaceID .. "/servers/Public?sortOrder=Asc&limit=100&cursor=" .. foundAnything
                        )
                    )
                end
                local ID = ""
                if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
                    foundAnything = Site.nextPageCursor
                end
                local num = 0
                for i, v in pairs(Site.data) do
                    local Possible = true
                    ID = tostring(v.id)
                    if tonumber(v.maxPlayers) > tonumber(v.playing) then
                        for _, Existing in pairs(AllIDs) do
                            if num ~= 0 then
                                if ID == tostring(Existing) then
                                    Possible = false
                                end
                            else
                                if tonumber(actualHour) ~= tonumber(Existing) then
                                    local delFile =
                                        pcall(
                                        function()
                                            delfile("NotSameServers.json")
                                            AllIDs = {}
                                            table.insert(AllIDs, actualHour)
                                        end
                                    )
                                end
                            end
                            num = num + 1
                        end
                        if Possible == true then
                            table.insert(AllIDs, ID)
                            wait()
                            pcall(
                                function()
                                    writefile("NotSameServers.json", game:GetService("HttpService"):JSONEncode(AllIDs))
                                    wait()
                                    game:GetService("TeleportService"):TeleportToPlaceInstance(
                                        PlaceID,
                                        ID,
                                        game.Players.LocalPlayer
                                    )
                                end
                            )
                            wait(4)
                        end
                    end
                end
            end

            function Teleport()
                while wait() do
                    pcall(
                        function()
                            TPReturner()
                            if foundAnything ~= "" then
                                TPReturner()
                            end
                        end
                    )
                end
            end

            -- If you'd like to use a script before server hopping (Like a Automatic Chest collector you can put the Teleport() after it collected everything.
            Teleport()
        elseif text == "ANTIKICK" then
            --// Variables

            local Players = game:GetService("Players")
            local OldNameCall = nil

            --// Global Variables

            getgenv().SendNotifications = true -- Set to true if you want to get notified regularly.

            --// Anti Kick Hook

            OldNameCall =
                hookmetamethod(
                game,
                "__namecall",
                function(Self, ...)
                    local NameCallMethod = getnamecallmethod()

                    if tostring(string.lower(NameCallMethod)) == "kick" then
                        if getgenv().SendNotifications == true then
                            game:GetService("StarterGui"):SetCore(
                                "SendNotification",
                                {
                                    Title = "Exunys Developer",
                                    Text = "You almost got kicked! Successfully prevented.",
                                    Icon = "rbxassetid://6238540373",
                                    Duration = 3
                                }
                            )
                        end

                        return nil
                    end

                    return OldNameCall(Self, ...)
                end
            )

            if getgenv().SendNotifications == true then
                game:GetService("StarterGui"):SetCore(
                    "SendNotification",
                    {
                        Title = "Exunys Developer",
                        Text = "Anti-Kick script loaded",
                        Icon = "rbxassetid://6238537240",
                        Duration = 5
                    }
                )
            end
	elseif text == "DEX" then
		loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/Dex%20Explorer.txt"))()

	elseif text == "REMOTESPY" then


-- FrontEnd // UI

-- Objects

local RemoteSpy = Instance.new("ScreenGui")
local BG = Instance.new("Frame")
local Ribbon = Instance.new("ImageLabel")
local Hide = Instance.new("TextButton")
local Title = Instance.new("TextLabel")
local Remotes = Instance.new("ScrollingFrame")
local Source = Instance.new("ScrollingFrame")
local ButtonsFrame = Instance.new("Frame")
local ToClipboard = Instance.new("TextButton")
local Decompile = Instance.new("TextButton")
local GetReturn = Instance.new("TextButton")
local ClearList = Instance.new("TextButton")
local CryptStrings = Instance.new("TextButton")
local EnableSpy = Instance.new("TextButton")
local Last = Instance.new("TextLabel")
local Total = Instance.new("TextLabel")
local Settings = Instance.new("TextButton")
local SetRemotes = Instance.new("ScrollingFrame")
local Storage = Instance.new("Frame")
local RBTN = Instance.new("TextButton")
local Icon = Instance.new("ImageLabel")
local RemoteName = Instance.new("TextLabel")
local ID = Instance.new("TextLabel")
local SBTN = Instance.new("TextButton")
local Icon_2 = Instance.new("ImageLabel")
local RemoteName_2 = Instance.new("TextLabel")
local ID_2 = Instance.new("TextLabel")
local ScriptLine = Instance.new("Frame")
local Line = Instance.new("TextLabel")
local SourceText = Instance.new("TextLabel")
local Tokens = Instance.new("TextLabel")
local Strings = Instance.new("TextLabel")
local Comments = Instance.new("TextLabel")
local Keywords = Instance.new("TextLabel")
local Globals = Instance.new("TextLabel")
local RemoteHighlight = Instance.new("TextLabel")
local Enabled = Instance.new("TextLabel")
local FullScreen = Instance.new("TextButton")
local SetRemotesTab = Instance.new("Frame")
local FilterF = Instance.new("TextButton")
local FilterE = Instance.new("TextButton")
local Search = Instance.new("TextBox")
local remotes_fired = 0
local encrypt_string = false
local spy_enabled = true

local lua_keywords = {"and", "break", "do", "else", "elseif", "end", "false", "for", "function", "goto", "if", "in", "local", "nil", "not", "or", "repeat", "return", "then", "true", "until", "while"}
local global_env = {"game", "workspace", "script", "math", "string", "table", "print", "wait", "BrickColor", "Color3", "next", "pairs", "ipairs", "select", "unpack", "Instance", "Vector2", "Vector3", "CFrame", "Ray", "UDim2", "Enum", "assert", "error", "warn", "tick", "loadstring", "_G", "shared", "getfenv", "setfenv", "newproxy", "setmetatable", "getmetatable", "os", "debug", "pcall", "ypcall", "xpcall", "rawequal", "rawset", "rawget", "tonumber", "tostring", "type", "typeof", "_VERSION", "coroutine", "delay", "require", "spawn", "LoadLibrary", "settings", "stats", "time", "UserSettings", "version", "Axes", "ColorSequence", "Faces", "ColorSequenceKeypoint", "NumberRange", "NumberSequence", "NumberSequenceKeypoint", "gcinfo", "elapsedTime", "collectgarbage", "PhysicalProperties", "Rect", "Region3", "Region3int16", "UDim", "Vector2int16", "Vector3int16"}

-- Properties

RemoteSpy.Name = "RemoteSpy"
RemoteSpy.Parent = game.CoreGui

BG.Name = "BG"
BG.Parent = RemoteSpy
BG.Active = true
BG.BackgroundColor3 = Color3.new(0.141176, 0.141176, 0.141176)
BG.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
BG.Draggable = true
BG.Position = UDim2.new(0.5, -700, 0.5, -400)
BG.Size = UDim2.new(1, -300, 1, -200)
BG.ClipsDescendants = true

Ribbon.Name = "Ribbon"
Ribbon.Parent = BG
Ribbon.BackgroundColor3 = Color3.new(0.760784, 0.0117647, 0.317647)
Ribbon.BorderSizePixel = 0
Ribbon.Size = UDim2.new(1, 0, 0, 20)
Ribbon.ZIndex = 2

Hide.Name = "Hide"
Hide.Parent = Ribbon
Hide.BackgroundColor3 = Color3.new(1, 0, 0)
Hide.BorderSizePixel = 0
Hide.Position = UDim2.new(1, -40, 0, 0)
Hide.Size = UDim2.new(0, 40, 0, 20)
Hide.ZIndex = 3
Hide.Font = Enum.Font.SourceSansBold
Hide.FontSize = Enum.FontSize.Size14
Hide.Text = "_"
Hide.TextColor3 = Color3.new(1, 1, 1)
Hide.TextSize = 14

Title.Name = "Title"
Title.Parent = Ribbon
Title.BackgroundColor3 = Color3.new(1, 0.0117647, 0.423529)
Title.BorderSizePixel = 0
Title.Position = UDim2.new(0.5, -100, 0, 0)
Title.Size = UDim2.new(0, 200, 0, 20)
Title.ZIndex = 3
Title.Font = Enum.Font.SourceSansBold
Title.FontSize = Enum.FontSize.Size14
Title.Text = "Remote2Script v2"
Title.TextColor3 = Color3.new(1, 1, 1)
Title.TextSize = 14

Remotes.Name = "Remotes"
Remotes.Parent = BG
Remotes.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
Remotes.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
Remotes.Position = UDim2.new(0, 10, 0, 80)
Remotes.CanvasSize = UDim2.new(0, 0, 40, 0)
Remotes.Size = UDim2.new(0, 250, 1, -90)
Remotes.ZIndex = 2
Remotes.BottomImage = "rbxassetid://148970562"
Remotes.MidImage = "rbxassetid://148970562"
Remotes.ScrollBarThickness = 5
Remotes.TopImage = "rbxassetid://148970562"

Source.Name = "Source"
Source.Parent = BG
Source.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
Source.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
Source.Position = UDim2.new(0, 270, 0, 80)
Source.Size = UDim2.new(1, -280, 1, -90)
Source.ZIndex = 2
Source.BottomImage = "rbxassetid://148970562"
Source.CanvasSize = UDim2.new(3, 0, 160, 0)
Source.MidImage = "rbxassetid://148970562"
Source.ScrollBarThickness = 5
Source.TopImage = "rbxassetid://148970562"

ButtonsFrame.Name = "ButtonsFrame"
ButtonsFrame.Parent = BG
ButtonsFrame.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
ButtonsFrame.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
ButtonsFrame.Position = UDim2.new(0, 10, 0, 30)
ButtonsFrame.Size = UDim2.new(1, -20, 0, 40)
ButtonsFrame.ZIndex = 2
ButtonsFrame.ClipsDescendants = true

ToClipboard.Name = "ToClipboard"
ToClipboard.Parent = ButtonsFrame
ToClipboard.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
ToClipboard.BorderColor3 = Color3.new(0.117647, 0.392157, 0.117647)
ToClipboard.Position = UDim2.new(0, 10, 0.5, -10)
ToClipboard.Size = UDim2.new(0, 100, 0, 20)
ToClipboard.ZIndex = 3
ToClipboard.Font = Enum.Font.SourceSansBold
ToClipboard.FontSize = Enum.FontSize.Size14
ToClipboard.Text = "COPY"
ToClipboard.TextColor3 = Color3.new(0.235294, 0.784314, 0.235294)
ToClipboard.TextSize = 14

Decompile.Name = "Decompile"
Decompile.Parent = ButtonsFrame
Decompile.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
Decompile.BorderColor3 = Color3.new(0.384314, 0.384314, 0.384314)
Decompile.Position = UDim2.new(0, 120, 0.5, -10)
Decompile.Size = UDim2.new(0, 100, 0, 20)
Decompile.ZIndex = 3
Decompile.Font = Enum.Font.SourceSansBold
Decompile.FontSize = Enum.FontSize.Size14
Decompile.Text = "DECOMPILE"
Decompile.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
Decompile.TextSize = 14

GetReturn.Name = "GetReturn"
GetReturn.Parent = ButtonsFrame
GetReturn.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
GetReturn.BorderColor3 = Color3.new(0.384314, 0.384314, 0.384314)
GetReturn.Position = UDim2.new(0, 230, 0.5, -10)
GetReturn.Size = UDim2.new(0, 100, 0, 20)
GetReturn.ZIndex = 3
GetReturn.Font = Enum.Font.SourceSansBold
GetReturn.FontSize = Enum.FontSize.Size14
GetReturn.Text = "GET RETURN"
GetReturn.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
GetReturn.TextSize = 14

ClearList.Name = "ClearList"
ClearList.Parent = ButtonsFrame
ClearList.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
ClearList.BorderColor3 = Color3.new(0.384314, 0.384314, 0.384314)
ClearList.Position = UDim2.new(0, 340, 0.5, -10)
ClearList.Size = UDim2.new(0, 100, 0, 20)
ClearList.ZIndex = 3
ClearList.Font = Enum.Font.SourceSansBold
ClearList.FontSize = Enum.FontSize.Size14
ClearList.Text = "CLEAR LOGS"
ClearList.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
ClearList.TextSize = 14

CryptStrings.Name = "CryptStrings"
CryptStrings.Parent = ButtonsFrame
CryptStrings.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
CryptStrings.BorderColor3 = Color3.new(0.392157, 0.117647, 0.117647)
CryptStrings.Position = UDim2.new(0, 450, 0.5, -10)
CryptStrings.Size = UDim2.new(0, 100, 0, 20)
CryptStrings.ZIndex = 3
CryptStrings.Font = Enum.Font.SourceSansBold
CryptStrings.FontSize = Enum.FontSize.Size14
CryptStrings.Text = "CRYPT STRINGS"
CryptStrings.TextColor3 = Color3.new(0.784314, 0.235294, 0.235294)
CryptStrings.TextSize = 14

EnableSpy.Name = "EnableSpy"
EnableSpy.Parent = ButtonsFrame
EnableSpy.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
EnableSpy.BorderColor3 = Color3.fromRGB(30, 100, 30)
EnableSpy.Position = UDim2.new(0, 560, 0.5, -10)
EnableSpy.Size = UDim2.new(0, 100, 0, 20)
EnableSpy.ZIndex = 3
EnableSpy.Font = Enum.Font.SourceSansBold
EnableSpy.FontSize = Enum.FontSize.Size14
EnableSpy.Text = "REMOTESPY"
EnableSpy.TextColor3 = Color3.fromRGB(60, 200, 60)
EnableSpy.TextSize = 14

Last.Name = "Last"
Last.Parent = ButtonsFrame
Last.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
Last.BorderColor3 = Color3.new(0.384314, 0.384314, 0.384314)
Last.Position = UDim2.new(0, 670, 0.5, -10)
Last.Size = UDim2.new(0, 200, 0, 20)
Last.ZIndex = 3
Last.Font = Enum.Font.SourceSansBold
Last.FontSize = Enum.FontSize.Size14
Last.Text = ""
Last.TextColor3 = Color3.new(1, 1, 1)
Last.TextSize = 14
Last.TextWrapped = true

Total.Name = "Total"
Total.Parent = ButtonsFrame
Total.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
Total.BorderColor3 = Color3.new(0.384314, 0.384314, 0.384314)
Total.Position = UDim2.new(0, 880, 0.5, -10)
Total.Size = UDim2.new(0, 50, 0, 20)
Total.ZIndex = 3
Total.Font = Enum.Font.SourceSansBold
Total.FontSize = Enum.FontSize.Size14
Total.Text = "0"
Total.TextColor3 = Color3.new(1, 1, 1)
Total.TextSize = 14
Total.TextWrapped = true

Settings.Name = "Settings"
Settings.Parent = ButtonsFrame
Settings.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
Settings.BorderColor3 = Color3.new(0.117647, 0.392157, 0.392157)
Settings.Position = UDim2.new(1, -110, 0.5, -10)
Settings.Size = UDim2.new(0, 100, 0, 20)
Settings.ZIndex = 3
Settings.Font = Enum.Font.SourceSansBold
Settings.FontSize = Enum.FontSize.Size14
Settings.Text = "REMOTES"
Settings.TextColor3 = Color3.new(0.235294, 0.784314, 0.784314)
Settings.TextSize = 14

SetRemotes.Name = "SetRemotes"
SetRemotes.Parent = BG
SetRemotes.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
SetRemotes.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
SetRemotes.Position = UDim2.new(0, 270, 0, 80)
SetRemotes.Size = UDim2.new(1, -280, 1, -140)
SetRemotes.Visible = false
SetRemotes.ZIndex = 2
SetRemotes.BottomImage = "rbxassetid://148970562"
SetRemotes.CanvasSize = UDim2.new(0, 0, 25, 0)
SetRemotes.MidImage = "rbxassetid://148970562"
SetRemotes.ScrollBarThickness = 5
SetRemotes.TopImage = "rbxassetid://148970562"

Storage.Name = "Storage"
Storage.Parent = RemoteSpy
Storage.BackgroundColor3 = Color3.new(1, 1, 1)
Storage.Size = UDim2.new(0, 100, 0, 100)
Storage.Visible = false

RBTN.Name = "RBTN"
RBTN.Parent = Storage
RBTN.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
RBTN.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
RBTN.Position = UDim2.new(0, 10, 0, 10)
RBTN.Size = UDim2.new(1, -20, 0, 20)
RBTN.ZIndex = 3
RBTN.Font = Enum.Font.SourceSansBold
RBTN.FontSize = Enum.FontSize.Size14
RBTN.Text = ""
RBTN.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
RBTN.TextSize = 14
RBTN.TextXAlignment = Enum.TextXAlignment.Left

Icon.Name = "Icon"
Icon.Parent = RBTN
Icon.BackgroundColor3 = Color3.new(1, 1, 1)
Icon.BackgroundTransparency = 1
Icon.Size = UDim2.new(0, 20, 0, 20)
Icon.ZIndex = 4
Icon.Image = "rbxassetid://413369506"

RemoteName.Name = "RemoteName"
RemoteName.Parent = RBTN
RemoteName.BackgroundColor3 = Color3.new(0.713726, 0.00392157, 0.298039)
RemoteName.BorderSizePixel = 0
RemoteName.Position = UDim2.new(0, 30, 0, 0)
RemoteName.Size = UDim2.new(0, 140, 0, 20)
RemoteName.ZIndex = 4
RemoteName.Font = Enum.Font.SourceSansBold
RemoteName.FontSize = Enum.FontSize.Size14
RemoteName.Text = "10"
RemoteName.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
RemoteName.TextSize = 14

ID.Name = "ID"
ID.Parent = RBTN
ID.BackgroundColor3 = Color3.new(0.458824, 0.00392157, 0.192157)
ID.BorderSizePixel = 0
ID.Position = UDim2.new(1, -50, 0, 0)
ID.Size = UDim2.new(0, 50, 0, 20)
ID.ZIndex = 4
ID.Font = Enum.Font.SourceSansBold
ID.FontSize = Enum.FontSize.Size14
ID.Text = "10"
ID.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
ID.TextSize = 14

SBTN.Name = "SBTN"
SBTN.Parent = Storage
SBTN.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
SBTN.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
SBTN.Position = UDim2.new(0, 10, 0, 10)
SBTN.Size = UDim2.new(1, -20, 0, 20)
SBTN.ZIndex = 3
SBTN.Font = Enum.Font.SourceSansBold
SBTN.FontSize = Enum.FontSize.Size14
SBTN.Text = ""
SBTN.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
SBTN.TextSize = 11
SBTN.TextXAlignment = Enum.TextXAlignment.Left

Icon_2.Name = "Icon"
Icon_2.Parent = SBTN
Icon_2.BackgroundColor3 = Color3.new(1, 1, 1)
Icon_2.BackgroundTransparency = 1
Icon_2.Size = UDim2.new(0, 20, 0, 20)
Icon_2.ZIndex = 4
Icon_2.Image = "rbxassetid://413369506"

RemoteName_2.Name = "RemoteName"
RemoteName_2.Parent = SBTN
RemoteName_2.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
RemoteName_2.BorderSizePixel = 1
RemoteName_2.BorderColor3 = Color3.fromRGB(62, 62, 62)
RemoteName_2.Position = UDim2.new(0, 30, 0, 0)
RemoteName_2.Size = UDim2.new(0, 140, 0, 20)
RemoteName_2.ZIndex = 4
RemoteName_2.Font = Enum.Font.SourceSansBold
RemoteName_2.FontSize = Enum.FontSize.Size14
RemoteName_2.Text = "SayMessageRequest"
RemoteName_2.TextColor3 = Color3.fromRGB(200, 200, 200)
RemoteName_2.TextSize = 11

ID_2.Name = "ID"
ID_2.Parent = SBTN
ID_2.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
ID_2.BorderSizePixel = 1
ID_2.BorderColor3 = Color3.fromRGB(62, 62, 62)
ID_2.Position = UDim2.new(1, -700, 0, 0)
ID_2.Size = UDim2.new(0, 700, 0, 20)
ID_2.ZIndex = 3
ID_2.Font = Enum.Font.SourceSansBold
ID_2.FontSize = Enum.FontSize.Size14
ID_2.Text = "10"
ID_2.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
ID_2.TextSize = 14

ScriptLine.Name = "ScriptLine"
ScriptLine.Parent = Storage
ScriptLine.BackgroundColor3 = Color3.new(1, 1, 1)
ScriptLine.BackgroundTransparency = 1
ScriptLine.Size = UDim2.new(1, 0, 0, 17)
ScriptLine.ZIndex = 2

Line.Name = "Line"
Line.Parent = ScriptLine
Line.BackgroundColor3 = Color3.new(0.329412, 0, 0)
Line.BackgroundTransparency = 1
Line.BorderSizePixel = 0
Line.Size = UDim2.new(0, 40, 1, 0)
Line.ZIndex = 3
Line.Font = Enum.Font.SourceSansBold
Line.FontSize = Enum.FontSize.Size18
Line.Text = ""
Line.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
Line.TextSize = 17

SourceText.Name = "SourceText"
SourceText.Parent = ScriptLine
SourceText.BackgroundColor3 = Color3.new(1, 1, 1)
SourceText.BackgroundTransparency = 1
SourceText.Position = UDim2.new(0, 40, 0, 0)
SourceText.Size = UDim2.new(1, -40, 1, 0)
SourceText.ZIndex = 3
SourceText.Font = Enum.Font.Code
SourceText.FontSize = Enum.FontSize.Size18
SourceText.Text = ""
SourceText.TextColor3 = Color3.new(1, 1, 1)
SourceText.TextSize = 17
SourceText.TextXAlignment = Enum.TextXAlignment.Left

Tokens.Name = "Tokens"
Tokens.Parent = ScriptLine
Tokens.BackgroundColor3 = Color3.new(1, 1, 1)
Tokens.BackgroundTransparency = 1
Tokens.Position = UDim2.new(0, 40, 0, 0)
Tokens.Size = UDim2.new(1, -40, 1, 0)
Tokens.ZIndex = 3
Tokens.Font = Enum.Font.Code
Tokens.FontSize = Enum.FontSize.Size18
Tokens.Text = ""
Tokens.TextColor3 = Color3.new(0.392157, 0.392157, 0.392157)
Tokens.TextSize = 17
Tokens.TextXAlignment = Enum.TextXAlignment.Left

Strings.Name = "Strings"
Strings.Parent = ScriptLine
Strings.BackgroundColor3 = Color3.new(1, 1, 1)
Strings.BackgroundTransparency = 1
Strings.Position = UDim2.new(0, 40, 0, 0)
Strings.Size = UDim2.new(1, -40, 1, 0)
Strings.ZIndex = 5
Strings.Font = Enum.Font.Code
Strings.FontSize = Enum.FontSize.Size18
Strings.Text = ""
Strings.TextColor3 = Color3.new(1, 0.615686, 0)
Strings.TextSize = 17
Strings.TextXAlignment = Enum.TextXAlignment.Left

Comments.Name = "Comments"
Comments.Parent = ScriptLine
Comments.BackgroundColor3 = Color3.new(1, 1, 1)
Comments.BackgroundTransparency = 1
Comments.Position = UDim2.new(0, 40, 0, 0)
Comments.Size = UDim2.new(1, -40, 1, 0)
Comments.ZIndex = 5
Comments.Font = Enum.Font.Code
Comments.FontSize = Enum.FontSize.Size18
Comments.Text = ""
Comments.TextColor3 = Color3.fromRGB(60, 200, 60)
Comments.TextSize = 17
Comments.TextXAlignment = Enum.TextXAlignment.Left

RemoteHighlight.Name = "RemoteHighlight"
RemoteHighlight.Parent = ScriptLine
RemoteHighlight.BackgroundColor3 = Color3.new(1, 1, 1)
RemoteHighlight.BackgroundTransparency = 1
RemoteHighlight.Position = UDim2.new(0, 40, 0, 0)
RemoteHighlight.Size = UDim2.new(1, -40, 1, 0)
RemoteHighlight.ZIndex = 3
RemoteHighlight.Font = Enum.Font.Code
RemoteHighlight.FontSize = Enum.FontSize.Size18
RemoteHighlight.Text = ""
RemoteHighlight.TextColor3 = Color3.fromRGB(0, 145, 255)
RemoteHighlight.TextSize = 17
RemoteHighlight.TextXAlignment = Enum.TextXAlignment.Left

Keywords.Name = "Keywords"
Keywords.Parent = ScriptLine
Keywords.BackgroundColor3 = Color3.new(1, 1, 1)
Keywords.BackgroundTransparency = 1
Keywords.Position = UDim2.new(0, 40, 0, 0)
Keywords.Size = UDim2.new(1, -40, 1, 0)
Keywords.ZIndex = 3
Keywords.Font = Enum.Font.Code
Keywords.FontSize = Enum.FontSize.Size18
Keywords.Text = ""
Keywords.TextColor3 = Color3.new(0.231373, 1, 0)
Keywords.TextSize = 17
Keywords.TextXAlignment = Enum.TextXAlignment.Left

Globals.Name = "Globals"
Globals.Parent = ScriptLine
Globals.BackgroundColor3 = Color3.new(1, 1, 1)
Globals.BackgroundTransparency = 1
Globals.Position = UDim2.new(0, 40, 0, 0)
Globals.Size = UDim2.new(1, -40, 1, 0)
Globals.ZIndex = 3
Globals.Font = Enum.Font.Code
Globals.FontSize = Enum.FontSize.Size18
Globals.Text = ""
Globals.TextColor3 = Color3.new(1, 0, 0)
Globals.TextSize = 17
Globals.TextXAlignment = Enum.TextXAlignment.Left

Enabled.Name = "Enabled"
Enabled.Parent = SBTN
Enabled.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Enabled.BorderSizePixel = 1
Enabled.BorderColor3 = Color3.fromRGB(30, 100, 30)
Enabled.Position = UDim2.new(0, 210, 0, 0)
Enabled.Size = UDim2.new(0, 100, 1, 0)
Enabled.ZIndex = 4
Enabled.Font = Enum.Font.SourceSansBold
Enabled.FontSize = Enum.FontSize.Size14
Enabled.Text = "Enabled"
Enabled.TextColor3 = Color3.fromRGB(60, 200, 60)
Enabled.TextSize = 14

FullScreen.Name = "FullScreen"
FullScreen.Parent = Ribbon
FullScreen.BackgroundColor3 = Color3.new(1, 0, 0)
FullScreen.BorderSizePixel = 0
FullScreen.Position = UDim2.new(1, -90, 0, 0)
FullScreen.Size = UDim2.new(0, 40, 0, 20)
FullScreen.ZIndex = 3
FullScreen.Font = Enum.Font.SourceSansBold
FullScreen.FontSize = Enum.FontSize.Size14
FullScreen.Text = "[~]"
FullScreen.TextColor3 = Color3.new(1, 1, 1)
FullScreen.TextSize = 14

SetRemotesTab.Name = "SetRemotesTab"
SetRemotesTab.Parent = BG
SetRemotesTab.Visible = false
SetRemotesTab.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
SetRemotesTab.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
SetRemotesTab.ClipsDescendants = true
SetRemotesTab.Position = UDim2.new(0, 270, 1, -50)
SetRemotesTab.Size = UDim2.new(1, -280, 0, 40)
SetRemotesTab.ZIndex = 2

FilterF.Name = "FilterF"
FilterF.Parent = SetRemotesTab
FilterF.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
FilterF.BorderColor3 = Color3.new(0.392157, 0.117647, 0.117647)
FilterF.Position = UDim2.new(0, 120, 0.5, -10)
FilterF.Size = UDim2.new(0, 120, 0, 20)
FilterF.ZIndex = 3
FilterF.Font = Enum.Font.SourceSansBold
FilterF.FontSize = Enum.FontSize.Size14
FilterF.Text = "FILTER FUNCTIONS"
FilterF.TextColor3 = Color3.new(0.784314, 0.235294, 0.235294)
FilterF.TextSize = 14

FilterE.Name = "FilterE"
FilterE.Parent = SetRemotesTab
FilterE.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
FilterE.BorderColor3 = Color3.new(0.392157, 0.117647, 0.117647)
FilterE.Position = UDim2.new(0, 10, 0.5, -10)
FilterE.Size = UDim2.new(0, 100, 0, 20)
FilterE.ZIndex = 3
FilterE.Font = Enum.Font.SourceSansBold
FilterE.FontSize = Enum.FontSize.Size14
FilterE.Text = "FILTER EVENTS"
FilterE.TextColor3 = Color3.new(0.784314, 0.235294, 0.235294)
FilterE.TextSize = 14

Search.Name = "Search"
Search.Parent = SetRemotesTab
Search.BackgroundColor3 = Color3.new(0.0784314, 0.0784314, 0.0784314)
Search.BorderColor3 = Color3.new(0.243137, 0.243137, 0.243137)
Search.Position = UDim2.new(0, 250, 0.5, -10)
Search.Selectable = true
Search.Size = UDim2.new(1, -260, 0, 20)
Search.ZIndex = 3
Search.Font = Enum.Font.SourceSansBold
Search.FontSize = Enum.FontSize.Size14
Search.Text = "[SEARCH]"
Search.TextColor3 = Color3.new(0.784314, 0.784314, 0.784314)
Search.TextSize = 14

-- FrontEnd-Backend // UI Functions

local HasSpecial = function(string)
    return (string:match("%c") or string:match("%s") or string:match("%p") or tonumber(string:sub(1,1))) ~= nil
end

local GetPath = function(Instance)
	local Obj = Instance
	local string = {}
	local temp = {}
	local error = false

	while Obj ~= game do
		if Obj == nil then
			error = true
			break
		end
		table.insert(temp, Obj.Parent == game and Obj.ClassName or tostring(Obj))
		Obj = Obj.Parent
	end

	table.insert(string, "game:GetService(\"" .. temp[#temp] .. "\")")

	for i = #temp - 1, 1, -1 do
		table.insert(string, HasSpecial(temp[i]) and "[\"" .. temp[i] .. "\"]" or "." .. temp[i])
	end

	return (error and "nil -- Path contained invalid instance" or table.concat(string, ""))
end

local GetType = function(Instance)
	local Types =
	{
		EnumItem = function()
			return "Enum." .. tostring(Instance.EnumType) .. "." .. tostring(Instance.Name)
		end,
		Instance = function()
			return GetPath(Instance)
		end,
		CFrame = function()
			return "CFrame.new(" .. tostring(Instance) .. ")"
		end,
		Vector3 = function()
			return "Vector3.new(" .. tostring(Instance) .. ")"
		end,
		BrickColor = function()
			return "BrickColor.new(\"" .. tostring(Instance) .. "\")"
		end,
		Color3 = function()
			return "Color3.new(" .. tostring(Instance) .. ")"
		end,
		string = function()
			local S = tostring(Instance)
			return "\"" .. (encrypt_string and S:gsub(".", function(c) return "\\" .. c:byte() end) or S) .. "\""
		end,
		Ray = function()
			return "Ray.new(Vector3.new(" .. tostring(Instance.Origin) .. "), Vector3.new(" .. tostring(Instance.Direction) .. "))"
		end
	}

	return Types[typeof(Instance)] ~= nil and Types[typeof(Instance)]() or tostring(Instance)
end

local size_frame = function(frame, UDim)
	frame:TweenSize(UDim, "Out", "Quint", 0.3)
end

local pos_frame = function(frame, UDim)
	frame:TweenPosition(UDim, "Out", "Quint", 0.3)
end

local size_pos_frame = function(frame, UDim, UDim2)
	frame:TweenSizeAndPosition(UDim, UDim2, "Out", "Quint", 0.3)
end

local hide = function()
	size_frame(BG, UDim2.new(0, 300, 0, 20))
	pos_frame(Title, UDim2.new(0, 0, 0, 0))
	pos_frame(Remotes, UDim2.new(0, 10, 0, 100))
	pos_frame(Source, UDim2.new(0, 270, 0, 100))
	BG.Draggable = true
	SetRemotes.Visible = false
	SetRemotesTab.Visible = false
	Source.Visible = true

	return "[]"
end

local show = function()
	size_frame(BG, UDim2.new(1, -300, 1, -200))
	pos_frame(BG, UDim2.new(0.1, 0, 0.1, 0))
	pos_frame(Title, UDim2.new(0.5, -100, 0, 0))
	pos_frame(Remotes, UDim2.new(0, 10, 0, 80))
	pos_frame(Source, UDim2.new(0, 270, 0, 80))
	BG.Draggable = false

	return "_"
end

local onclick_hide = function()
	Hide.Text = Hide.Text == "_" and hide() or show()
end

local onclick_settings = function()
	Source.Visible = not Source.Visible
	SetRemotes.Visible = not Source.Visible
	SetRemotesTab.Visible = not Source.Visible
end

local onclick_remotespy = function()
	spy_enabled = not spy_enabled
	EnableSpy.TextColor3 = EnableSpy.TextColor3 == Color3.fromRGB(60, 200, 60) and Color3.fromRGB(200, 60, 60) or Color3.fromRGB(60, 200, 60)
	EnableSpy.BorderColor3 = EnableSpy.TextColor3 == Color3.fromRGB(200, 60, 60) and Color3.fromRGB(100, 30, 30) or Color3.fromRGB(30, 100, 30)
end

local onclick_cryptstring = function()
	encrypt_string = not encrypt_string
	CryptStrings.TextColor3 = CryptStrings.TextColor3 == Color3.fromRGB(60, 200, 60) and Color3.fromRGB(200, 60, 60) or Color3.fromRGB(60, 200, 60)
	CryptStrings.BorderColor3 = CryptStrings.TextColor3 == Color3.fromRGB(200, 60, 60) and Color3.fromRGB(100, 30, 30) or Color3.fromRGB(30, 100, 30)
end

local clear_logs = function()
	Remotes:ClearAllChildren()
	remotes_fired = 0
	Total.Text = "0"
end

local filter_events = function()
	local n = 0
	for i, v in pairs(SetRemotes:GetChildren()) do
		v.Visible = not (FilterE.TextColor3 == Color3.fromRGB(60, 200, 60) and v.Icon.Image == "rbxassetid://413369623")
		if v.Visible == true then
			n = n + 1
			v.Position = UDim2.new(0, 10, 0, -20 + n * 30)
		else
			v.Position = UDim2.new(0, 10, 0, -20 + i * 30)
		end
	end
end

local filter_functions = function()
	local n = 0
	for i, v in pairs(SetRemotes:GetChildren()) do
		v.Visible = not (FilterF.TextColor3 == Color3.fromRGB(60, 200, 60) and v.Icon.Image == "rbxassetid://413369506")
		if v.Visible == true then
			n = n + 1
			v.Position = UDim2.new(0, 10, 0, -20 + n * 30)
		else
			v.Position = UDim2.new(0, 10, 0, -20 + i * 30)
		end
	end
end

local onclick_fevents = function()
	FilterE.TextColor3 = FilterE.TextColor3 == Color3.fromRGB(60, 200, 60) and Color3.fromRGB(200, 60, 60) or Color3.fromRGB(60, 200, 60)
	FilterE.BorderColor3 = FilterE.TextColor3 == Color3.fromRGB(200, 60, 60) and Color3.fromRGB(100, 30, 30) or Color3.fromRGB(30, 100, 30)
	filter_events()
end

local onclick_ffunctions = function()
	FilterF.TextColor3 = FilterF.TextColor3 == Color3.fromRGB(60, 200, 60) and Color3.fromRGB(200, 60, 60) or Color3.fromRGB(60, 200, 60)
	FilterF.BorderColor3 = FilterF.TextColor3 == Color3.fromRGB(200, 60, 60) and Color3.fromRGB(100, 30, 30) or Color3.fromRGB(30, 100, 30)
	filter_functions()
end

local Highlight = function(string, keywords)
    local K = {}
    local S = string
    local Token =
    {
        ["="] = true,
        ["."] = true,
        [","] = true,
        ["("] = true,
        [")"] = true,
        ["["] = true,
        ["]"] = true,
        ["{"] = true,
        ["}"] = true,
        [":"] = true,
        ["*"] = true,
        ["/"] = true,
        ["+"] = true,
        ["-"] = true,
        ["%"] = true,
		[";"] = true,
		["~"] = true
    }
    for i, v in pairs(keywords) do
        K[v] = true
    end
    S = S:gsub(".", function(c)
        if Token[c] ~= nil then
            return "\32"
        else
            return c
        end
    end)
    S = S:gsub("%S+", function(c)
        if K[c] ~= nil then
            return c
        else
            return (" "):rep(#c)
        end
    end)

    return S
end

local Tokens = function(string)
    local Token =
    {
        ["="] = true,
        ["."] = true,
        [","] = true,
        ["("] = true,
        [")"] = true,
        ["["] = true,
        ["]"] = true,
        ["{"] = true,
        ["}"] = true,
        [":"] = true,
        ["*"] = true,
        ["/"] = true,
        ["+"] = true,
        ["-"] = true,
        ["%"] = true,
		[";"] = true,
		["~"] = true
    }
    local A = ""
    string:gsub(".", function(c)
        if Token[c] ~= nil then
            A = A .. c
        elseif c == "\n" then
            A = A .. "\n"
		elseif c == "\t" then
			A = A .. "\t"
        else
            A = A .. "\32"
        end
    end)

    return A
end

local strings = function(string)
    local highlight = ""
    local quote = false
    string:gsub(".", function(c)
        if quote == false and c == "\"" then
            quote = true
        elseif quote == true and c == "\"" then
            quote = false
        end
        if quote == false and c == "\"" then
            highlight = highlight .. "\""
        elseif c == "\n" then
            highlight = highlight .. "\n"
	elseif c == "\t" then
	    highlight = highlight .. "\t"
        elseif quote == true then
            highlight = highlight .. c
        elseif quote == false then
            highlight = highlight .. "\32"
        end
    end)

    return highlight
end

local comments = function(string)
    local ret = ""
    string:gsub("[^\r\n]+", function(c)
        local comm = false
        local i = 0
        c:gsub(".", function(n)
            i = i + 1
            if c:sub(i, i + 1) == "--" then
                comm = true
            end
            if comm == true then
                ret = ret .. n
            else
                ret = ret .. "\32"
            end
        end)
        ret = ret
    end)

    return ret
end

local copy_source = function()
	local script = ""
	local copy
	for i, v in pairs(Source:GetChildren()) do
		script = script .. v.SourceText.Text .. "\n"
	end
	if Clipboard ~= nil then
		copy = Clipboard.set
	elseif Synapse ~= nil then
		copy = function(str)
			Synapse:Copy(str)
		end
	elseif setclipboard ~= nil then
		copy = setclipboard
	end
	copy(script)
end

local onclick_fullscreen = function()
	size_pos_frame(BG, UDim2.new(1, 0, 1, 40), UDim2.new(0, 0, 0, -40))
	BG.Draggable = false
end

local filter_remotes = function(type)
	local n = 0
	if type == "Text" then
		for i, v in pairs(SetRemotes:GetChildren()) do
			if v.Name:lower():match(Search.Text:lower()) and string ~= "" then
				v.Visible = true
				n = n + 1
			else
				v.Visible = false
			end
			if v.Visible == true then
				v.Position = UDim2.new(0, 10, 0, -20 + n * 30)
			else
				v.Position = UDim2.new(0, 10, 0, -20 + i * 30)
			end
		end
	end
end

local fix = function(string)
	if string == "/e fix" then
		show()
		wait(0.3)
		pos_frame(BG, UDim2.new(0.1, 0, 0.1, 0))
	end
end

-- FrontEnd-Connections // UI Events

Hide.MouseButton1Down:Connect(onclick_hide)
Settings.MouseButton1Down:Connect(onclick_settings)
ClearList.MouseButton1Down:Connect(clear_logs)
EnableSpy.MouseButton1Down:Connect(onclick_remotespy)
ToClipboard.MouseButton1Down:Connect(copy_source)
CryptStrings.MouseButton1Down:Connect(onclick_cryptstring)
FullScreen.MouseButton1Down:Connect(onclick_fullscreen)
FilterE.MouseButton1Down:Connect(onclick_fevents)
FilterF.MouseButton1Down:Connect(onclick_ffunctions)
Search.Changed:Connect(filter_remotes)
game:GetService("Players").LocalPlayer.Chatted:Connect(fix)

-- Recursive Remotefill // UI-Backend

Table_TS = function(T)
    local M = {}
    for i, v in pairs(T) do
        local I = "\n\t" .. (type(i) == "number" and "[" .. i .. "] = " or "[\"" .. i .. "\"] = ")
        table.insert(M, I .. (type(v) == "table" and Table_TS(v) or GetType(v)))
    end

    return "\n{" .. table.concat(M, ", ") .. "\n}"
end

function fill(base)
	for i, v in pairs(base:GetChildren()) do
		if v.ClassName:match("Remote") and v.Name ~= "CharacterSoundEvent" then
			local B = SBTN:Clone()

			B.Parent = SetRemotes
			B.Icon.Image = (v.ClassName == "RemoteEvent" and "rbxassetid://413369506" or "rbxassetid://413369623")
			B.RemoteName.Text = v.Name
			B.ID.Text = GetPath(v)
			B.Name = v.Name
			B.Position = UDim2.new(0, 10, 0, -20 + #SetRemotes:GetChildren() * 30)
			B.MouseButton1Down:Connect(function()
				B.Enabled.Text = B.Enabled.Text == "Enabled" and "Disabled" or "Enabled"
				B.Enabled.TextColor3 = B.Enabled.Text == "Enabled" and Color3.fromRGB(60, 200, 60) or Color3.fromRGB(200, 60, 60)
				B.Enabled.BorderColor3 = B.Enabled.Text == "Enabled" and Color3.fromRGB(30, 100, 30) or Color3.fromRGB(100, 30, 30)
			end)
		end
		fill(v)
	end
end

fill(game)

-- Backend // Remotespy Backend

local game_meta = getrawmetatable(game)
local game_namecall = game_meta.__namecall
local namecall_dump = {}
local current_rmt = nil
local g_caller = nil
local f_return = nil
local Step = game:GetService("RunService").Stepped

local mwr

if setreadonly ~= nil then
	mwr = function()
		setreadonly(game_meta, false)
	end
elseif make_writeable ~= nil then
	mwr = function()
		make_writeable(game_meta)
	end
end

mwr()

local namecall_script = function(object, method, ...)
	local script = "-- Script generated by R2Sv2\n-- R2Sv2 developed by Luckyxero\n\32\n"
	local args = {}
	for i, v in pairs{...} do
		script = script .. "local A_" .. i .. " = " .. (type(v) == "table" and Table_TS(v) or GetType(v)) .. "\n"
		table.insert(args, "A_" .. i)
	end
	script = script .. "local Event = " .. GetPath(object) .. "\n\n"
	script = script .. "Event:" .. method .. "(" .. table.concat(args, ", ") .. ")"

	return script
end

local dump_script = function(script)
	Source:ClearAllChildren()
	local lines = 0
	script:gsub("[^\r\n]+", function(c)
		lines = lines + 1
		local tabs = 0
		c:gsub("%\t", function() tabs = tabs + 1 end)
		local line = ScriptLine:Clone()
		line.Parent = Source
		line.SourceText.Text = c
		line.Line.Text = lines
		line.RemoteHighlight.Text = Highlight(c, {"FireServer", "InvokeServer", "invokeServer", "fireServer"})
		line.Position = UDim2.new(0, tabs * (17 * 2), 0, -17 + #Source:GetChildren() * 17)
		line.Globals.Text = Highlight(c, global_env)
		line.Line.Position = UDim2.new(0, 0 - tabs * (17 * 2), 0, 0)
		line.Strings.Text = strings(c)
		line.Keywords.Text = Highlight(c, lua_keywords)
		line.Tokens.Text = Tokens(c)
		line.Comments.Text = comments(c)
	end)
end

local log_remote = function(table)
	if SetRemotes[table.object.Name].Enabled.Text == "Disabled" then return end
	local B = RBTN:Clone()
	g_caller = table.caller
	remotes_fired = remotes_fired + 1
	Total.Text = remotes_fired

	B.Parent = Remotes
	B.Position = UDim2.new(0, 10, 0, -20 + #Remotes:GetChildren() * 30)
	B.Icon.Image = table.method == "FireServer" and "rbxassetid://413369506" or "rbxassetid://413369623"
	B.RemoteName.Text = table.object.Name
	B.ID.Text = tostring(remotes_fired)
	B.MouseButton1Down:Connect(function()
		dump_script(table.script)
		g_caller = table.caller
		f_return = table.freturn == nil and table.object.Name .. " is not RemoteFunction" or table.freturn
	end)
end


local get_namecall_dump = function(script, object, ...)
	local Ret = nil
	if object.ClassName == "RemoteFunction" then
		local freturn = {pcall(object.InvokeServer, object, ...)}
		freturn = {select(2, unpack(freturn))}

		if #freturn == 0 then
			Ret = object.Name .. " is a void type RemoteFunction."
		else
			Ret = Table_TS(freturn)
		end
	end
	namecall_dump[#namecall_dump + 1] =
	{
		script = namecall_script(object, object.ClassName == "RemoteEvent" and "FireServer" or "InvokeServer", ...),
		caller = script,
		object = object,
		method = object.ClassName == "RemoteEvent" and "FireServer" or "InvokeServer",
		freturn = Ret
	}
end

GetReturn.MouseButton1Down:Connect(function()
	dump_script(f_return)
end)

Decompile.MouseButton1Down:Connect(function()
	dump_script('Decompile currently broken with LuaU.')
end)

Step:Connect(function()
	while #namecall_dump > 0 do
		log_remote(table.remove(namecall_dump, 1))
	end
end)

local on_namecall = function(object, ...)
	local method = tostring(getnamecallmethod())
	local args = {...}
	if object.Name ~= "CharacterSoundEvent" and method:match("Server") and spy_enabled == true then get_namecall_dump(getfenv(2).script, object, unpack(args)) end

	return game_namecall(object, ...)
end

game_meta.__namecall = on_namecall
	elseif text == "MSGSPY" then




--[[
	Simple Chat Spy
	Type "spy" to enable or disable the chat spy.
	Only tested if this works executed with Synapse (should work with other exploits though)
--]]

print("-- Chat Spy Executed --")
print("Type \"spy\" to enable or disable the chat spy.")
print("Only tested if this works executed with Synapse (should work with other exploits though)")
print("https://github.com/dehoisted/Chat-Spy")

-- Config
Config = {
	enabled = true,
	spyOnMyself = true,
	public = false,
	publicItalics = true
}

-- Customizing Log Output
PrivateProperties = {
	Color = Color3.fromRGB(0,255,255);
	Font = Enum.Font.SourceSansBold;
	TextSize = 18;
}

	local StarterGui = game:GetService("StarterGui")
	local Players = game:GetService("Players")
	local player = Players.LocalPlayer
	local saymsg = game:GetService("ReplicatedStorage"):WaitForChild("DefaultChatSystemChatEvents"):WaitForChild("SayMessageRequest")
	local getmsg = game:GetService("ReplicatedStorage"):WaitForChild("DefaultChatSystemChatEvents"):WaitForChild("OnMessageDoneFiltering")
	local instance = (_G.chatSpyInstance or 0) + 1
	_G.chatSpyInstance = instance

	local function onChatted(p,msg)
		if _G.chatSpyInstance == instance then
			if p==player and msg:lower():sub(1,4)=="/spy" then
				Config.enabled = not Config.enabled
				wait(0.3)
				PrivateProperties.Text = "{SPY "..(Config.enabled and "EN" or "DIS").."ABLED}"
				StarterGui:SetCore("ChatMakeSystemMessage", PrivateProperties)
			elseif Config.enabled and (Config.spyOnMyself==true or p~=player) then
				msg = msg:gsub("[\n\r]",''):gsub("\t",' '):gsub("[ ]+",' ')
				local hidden = true
				local conn = getmsg.OnClientEvent:Connect(function(packet,channel)
					if packet.SpeakerUserId==p.UserId and packet.Message==msg:sub(#msg-#packet.Message+1) and (channel=="All" or (channel=="Team" and Config.public==false and Players[packet.FromSpeaker].Team==player.Team)) then
						hidden = false
					end
				end)
				wait(1)
				conn:Disconnect()
				if hidden and Config.enabled then
					if Config.public then
						saymsg:FireServer((Config.publicItalics and "/me " or '').."{SPY} [".. p.Name .."]: "..msg,"All")
					else
						PrivateProperties.Text = "{SPY} [".. p.Name .."]: "..msg
						StarterGui:SetCore("ChatMakeSystemMessage", PrivateProperties)
					end
				end
			end
		end
	end

	for _,p in ipairs(Players:GetPlayers()) do
		p.Chatted:Connect(function(msg) onChatted(p,msg) end)
	end

	Players.PlayerAdded:Connect(function(p)
		p.Chatted:Connect(function(msg) onChatted(p,msg) end)
	end)

	PrivateProperties.Text = "{SPY "..(Config.enabled and "EN" or "DIS").."ABLED}"
	StarterGui:SetCore("ChatMakeSystemMessage", PrivateProperties)
	local chatFrame = player.PlayerGui.Chat.Frame
	chatFrame.ChatChannelParentFrame.Visible = true
	chatFrame.ChatBarParentFrame.Position = chatFrame.ChatChannelParentFrame.Position+UDim2.new(UDim.new(),chatFrame.ChatChannelParentFrame.Size.Y)


	elseif text == "Newbies" then

local wsmode = 1
local jpmode = 1
local gothrough = false
local lotptog = false
local bodyang = nil
local cameratoggle = false
local spintoggle = false
local flytoggle = false
local scg = Instance.new('ScreenGui',game.Players.LocalPlayer.PlayerGui)
scg.ResetOnSpawn = false
local frm = Instance.new('Frame',scg)
frm.BorderSizePixel = 0
frm.BackgroundColor3 = Color3.new(255/255,122/255,122/255)
frm.Size = UDim2.new(0.3,0,0.3,0)
frm.Position = UDim2.new(0.35,0,0.35,0)
frm.Draggable = true


local topl = Instance.new('TextLabel',frm)
topl.BorderSizePixel = 0
topl.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
topl.Size = UDim2.new(0.9,1,0.2,0)
topl.Position = UDim2.new(0,0,0,0)
topl.TextScaled = true
topl.Font = "SourceSansLight"
topl.TextColor3 = Color3.new(1,1,1)
topl.Text = "Newbie's FE Gui V1.1"
topl.Draggable = true

local scrl = Instance.new('ScrollingFrame',frm)
scrl.BorderSizePixel = 0
scrl.BackgroundColor3 = Color3.new(255/255,122/255,122/255)
scrl.Size = UDim2.new(1,0,0.8,0)
scrl.Position = UDim2.new(0,0,0.2,0)
scrl.BottomImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"
scrl.TopImage = "rbxasset://textures/ui/Scroll/scroll-middle.png"






local plr = Instance.new('TextBox',scrl)
plr.BorderSizePixel = 0
plr.BackgroundColor3 = Color3.new(255/255,150/255,150/255)
plr.Size = UDim2.new(0.425,0,0.1,0)
plr.Position = UDim2.new(0.05,0,0.025,0)
plr.TextScaled = true
plr.Font = "SourceSansLight"
plr.TextColor3 = Color3.new(1,1,1)
plr.Text = "Player Name Here"


local plrsp = Instance.new('TextButton',scrl)
plrsp.BorderSizePixel = 0
plrsp.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
plrsp.Size = UDim2.new(0.425,0,0.1,0)
plrsp.Position = UDim2.new(0.5,0,0.025,0)
plrsp.TextScaled = true
plrsp.Font = "SourceSansLight"
plrsp.TextColor3 = Color3.new(1,1,1)
plrsp.Text = "Spawn Blocks"


local minim = Instance.new('TextButton',frm)
minim.BorderSizePixel = 0
minim.BackgroundColor3 = Color3.new(200/255,50/255,50/255)
minim.Size = UDim2.new(0.1,0,0.2,0)
minim.Position = UDim2.new(0.9,0,0,0)
minim.TextScaled = true
minim.Font = "SourceSansLight"
minim.TextColor3 = Color3.new(1,1,1)
minim.Text = "-"





function sblock()
for i=1,20 do
wait(1)
        for _,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
if v:IsA'Accoutrement' then
v.Parent=game.Players.LocalPlayer.Character
v.Parent = workspace.Terrain
end
end
for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
if v:IsA'Accoutrement' then
for ape,hax in pairs(v.Handle:GetChildren()) do
hax:Destroy()
end
wait'.1'
v.Parent=game.Players.LocalPlayer.StarterGear
end
end
for _,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
v:Destroy()
end
local prt=Instance.new("Model", workspace);
        Instance.new("Part", prt).Name="Torso";
        Instance.new("Part", prt).Name="Head";
        Instance.new("Humanoid", prt).Name="Humanoid";
        game.Players.LocalPlayer.Character=prt

repeat wait(1) until game.Players.LocalPlayer.Character:FindFirstChild'Head'
for lol,dad in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
if dad:IsA'Accoutrement' then
dad.Parent = game.Players.LocalPlayer.StarterGear
end
end
for _,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
v:Destroy()
end
local prt2=Instance.new("Model", workspace);
        Instance.new("Part", prt).Name="Torso";
        Instance.new("Part", prt).Name="Head";
        Instance.new("Humanoid", prt).Name="Humanoid";
        game.Players.LocalPlayer.Character=prt
end
end
plrsp.MouseButton1Click:connect(sblock)





local spin = Instance.new('TextButton',scrl)
spin.BorderSizePixel = 0
spin.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
spin.Size = UDim2.new(0.425,0,0.1,0)
spin.Position = UDim2.new(0.05,0,0.15,0)
spin.TextScaled = true
spin.Font = "SourceSansLight"
spin.TextColor3 = Color3.new(1,1,1)
spin.Text = "Crazy Spin: OFF"

local fly = Instance.new('TextButton',scrl)
fly.BorderSizePixel = 0
fly.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
fly.Size = UDim2.new(0.425,0,0.1,0)
fly.Position = UDim2.new(0.5,0,0.15,0)
fly.TextScaled = true
fly.Font = "SourceSansLight"
fly.TextColor3 = Color3.new(1,1,1)
fly.Text = "Fly: OFF"




local seethr = Instance.new('TextButton',scrl)
seethr.BorderSizePixel = 0
seethr.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
seethr.Size = UDim2.new(0.425,0,0.1,0)
seethr.Position = UDim2.new(0.05,0,0.275,0)
seethr.TextScaled = true
seethr.Font = "SourceSansLight"
seethr.TextColor3 = Color3.new(1,1,1)
seethr.Text = "See-Through: OFF"

local tpto = Instance.new('TextButton',scrl)
tpto.BorderSizePixel = 0
tpto.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
tpto.Size = UDim2.new(0.425,0,0.1,0)
tpto.Position = UDim2.new(0.5,0,0.275,0)
tpto.TextScaled = true
tpto.Font = "SourceSansLight"
tpto.TextColor3 = Color3.new(1,1,1)
tpto.Text = "Teleport To"



local ws = Instance.new('TextButton',scrl)
ws.BorderSizePixel = 0
ws.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
ws.Size = UDim2.new(0.425,0,0.1,0)
ws.Position = UDim2.new(0.05,0,0.4,0)
ws.TextScaled = true
ws.Font = "SourceSansLight"
ws.TextColor3 = Color3.new(1,1,1)
ws.Text = "WalkSpeed: Normal"

local jp = Instance.new('TextButton',scrl)
jp.BorderSizePixel = 0
jp.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
jp.Size = UDim2.new(0.425,0,0.1,0)
jp.Position = UDim2.new(0.5,0,0.4,0)
jp.TextScaled = true
jp.Font = "SourceSansLight"
jp.TextColor3 = Color3.new(1,1,1)
jp.Text = "JumpPower: Normal"





local lotp = Instance.new('TextButton',scrl)
lotp.BorderSizePixel = 0
lotp.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
lotp.Size = UDim2.new(0.425,0,0.1,0)
lotp.Position = UDim2.new(0.05,0,0.525,0)
lotp.TextScaled = true
lotp.Font = "SourceSansLight"
lotp.TextColor3 = Color3.new(1,1,1)
lotp.Text = "Loop-Teleport: OFF"

local sb = Instance.new('TextButton',scrl)
sb.BorderSizePixel = 0
sb.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
sb.Size = UDim2.new(0.425,0,0.1,0)
sb.Position = UDim2.new(0.5,0,0.525,0)
sb.TextScaled = true
sb.Font = "SourceSansLight"
sb.TextColor3 = Color3.new(1,1,1)
sb.Text = "Noclip"


local cr = Instance.new('TextLabel',scrl)
cr.BorderSizePixel = 0
cr.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
cr.Size = UDim2.new(0.875,0,0.225,0)
cr.Position = UDim2.new(0.05,0,0.65,0)
cr.TextScaled = true
cr.Font = "SourceSansLight"
cr.TextColor3 = Color3.new(1,1,1)
cr.Text = "Gui Created by Newbie15. Credit Goes to RGeeneus/Ignoramical for the Fly Script and Natural Modder for leaking the block spam script. but most importantly credits go to the users of this Gui."


local fl = Instance.new('TextLabel',scrl)
fl.BorderSizePixel = 0
fl.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
fl.Size = UDim2.new(0.875,0,0.075,0)
fl.Position = UDim2.new(0.05,0,0.9,0)
fl.TextScaled = true
fl.Font = "SourceSansLight"
fl.TextColor3 = Color3.new(1,1,1)
if game.Workspace.FilteringEnabled == true then
fl.Text = "Filtering is Enabled"
else
fl.Text = "Filtering is Disabled"
end




local gui2 = Instance.new('ScreenGui',game.Players.LocalPlayer.PlayerGui)
gui2.ResetOnSpawn = false


local oc = Instance.new('TextButton',gui2)
oc.BorderSizePixel = 0
oc.BackgroundColor3 = Color3.new(255/255,70/255,70/255)
oc.Size = UDim2.new(0,50,0,50)
oc.Position = UDim2.new(0,0,0,0)
oc.TextScaled = true
oc.Font = "SourceSansLight"
oc.TextColor3 = Color3.new(1,1,1)
oc.Text = "Close"
oc.Draggable = true













-- FLY SCRIPT BY RGEENEUS

-- The following code should be in a local script.
-- Only works on PC, not xbox or mobile. I do not have devices to test on.
-- Call the start fly function AFTER the character exists to fly. The function does not run if there is no character.

local speed = 50 -- This is the fly speed. Change it to whatever you like. The variable can be changed while running

local c
local h
local bv
local bav
local cam
local flying
local p = game.Players.LocalPlayer
local buttons = {W = false, S = false, A = false, D = false, Moving = false}

local startFly = function () -- Call this function to begin flying
    if not p.Character or not p.Character.Head or flying then return end
    c = p.Character
    h = c.Humanoid
    h.PlatformStand = true
    cam = workspace:WaitForChild('Camera')
    bv = Instance.new("BodyVelocity")
    bav = Instance.new("BodyAngularVelocity")
    bv.Velocity, bv.MaxForce, bv.P = Vector3.new(0, 0, 0), Vector3.new(10000, 10000, 10000), 1000
    bav.AngularVelocity, bav.MaxTorque, bav.P = Vector3.new(0, 0, 0), Vector3.new(10000, 10000, 10000), 1000
    bv.Parent = c.Head
    bav.Parent = c.Head
    flying = true
    h.Died:connect(function() flying = false end)
end

local endFly = function () -- Call this function to stop flying
    if not p.Character or not flying then return end
    h.PlatformStand = false
    bv:Destroy()
    bav:Destroy()
    flying = false
end

game:GetService("UserInputService").InputBegan:connect(function (input, GPE)
    if GPE then return end
    for i, e in pairs(buttons) do
        if i ~= "Moving" and input.KeyCode == Enum.KeyCode[i] then
            buttons[i] = true
            buttons.Moving = true
        end
    end
end)

game:GetService("UserInputService").InputEnded:connect(function (input, GPE)
    if GPE then return end
    local a = false
    for i, e in pairs(buttons) do
        if i ~= "Moving" then
            if input.KeyCode == Enum.KeyCode[i] then
                buttons[i] = false
            end
            if buttons[i] then a = true end
        end
    end
    buttons.Moving = a
end)

local setVec = function (vec)
    return vec * (speed / vec.Magnitude)
end

game:GetService("RunService").Heartbeat:connect(function (step) -- The actual fly function, called every frame
    if flying and c and c.PrimaryPart then
        local p = c.PrimaryPart.Position
        local cf = cam.CFrame
        local ax, ay, az = cf:toEulerAnglesXYZ()
        c:SetPrimaryPartCFrame(CFrame.new(p.x, p.y, p.z) * CFrame.Angles(ax, ay, az))
        if buttons.Moving then
            local t = Vector3.new()
            if buttons.W then t = t + (setVec(cf.lookVector)) end
            if buttons.S then t = t - (setVec(cf.lookVector)) end
            if buttons.A then t = t - (setVec(cf.rightVector)) end
            if buttons.D then t = t + (setVec(cf.rightVector)) end
            c:TranslateBy(t * step)
        end
    end
end)














function spintogl()
    if spintoggle == true then
        spintoggle = false
        spin.Text = "Crazy Spin: OFF"
    else
        spintoggle = true
        spin.Text = "Crazy Spin: ON"
        local bodyang = Instance.new('BodyAngularVelocity',game.Players.LocalPlayer.Character.PrimaryPart)
        bodyang.AngularVelocity = Vector3.new(90,999,0)
        bodyang.MaxTorque = Vector3.new(60000,100,3000)
        bodyang.P = 5000000
        repeat
            wait(0.001)
        until spintoggle == false
        bodyang:Destroy()
    end
end
spin.MouseButton1Click:connect(spintogl)


function flytogl()
    if flytoggle == true then
        flytoggle = false
        fly.Text = "Fly: OFF"
    else
        flytoggle = true
        fly.Text = "Fly: ON"
        startFly()
        repeat
            wait(0.001)
        until flytoggle == false
        endFly()
    end
end
fly.MouseButton1Click:connect(flytogl)



function opctogl()
    if scg.Enabled == true then
        scg.Enabled = false
        oc.Text = "Open"
    else
        scg.Enabled = true
        oc.Text = "Close"
    end
end
oc.MouseButton1Click:connect(opctogl)
function telep()
    game.Players.LocalPlayer.Character:MoveTo(game.Players:FindFirstChild(plr.Text).Character.PrimaryPart.Position)
end
tpto.MouseButton1Click:connect(telep)


function camtogl()
    if cameratoggle == false then
        cameratoggle = true
        game.Workspace.CurrentCamera.CameraType = "Follow"
        seethr.Text = "See-Through: ON"
    else
        cameratoggle = false
        game.Workspace.CurrentCamera.CameraType = "Custom"
        seethr.Text = "See-Through: OFF"
    end
end
seethr.MouseButton1Click:connect(camtogl)






function wsp()
    if wsmode ~= 5 then
        wsmode = wsmode + 1
    else
        wsmode = 1
    end
    if wsmode == 1 then
        ws.Text = "WalkSpeed: Normal"
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
    end
    if wsmode == 2 then
        ws.Text = "WalkSpeed: Fast"
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 32
    end
    if wsmode == 3 then
        ws.Text = "WalkSpeed: FASTER"
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 70
    end
    if wsmode == 4 then
        ws.Text = "WalkSpeed: EXTREME"
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 150
    end
    if wsmode == 5 then
        ws.Text = "WalkSpeed: The Speed of Light"
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 4357234785243
    end
end
ws.MouseButton1Click:connect(wsp)





function jpp()
    if jpmode ~= 5 then
        jpmode = jpmode + 1
    else
        jpmode = 1
    end
    if jpmode == 1 then
        jp.Text = "JumpPower: Normal"
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 50
    end
    if jpmode == 2 then
        jp.Text = "JumpPower: Trampoline"
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 100
    end
    if jpmode == 3 then
        jp.Text = "JumpPower: Big Trampoline"
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 200
    end
    if jpmode == 4 then
        jp.Text = "JumpPower: Bigger Trampoline"
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 400
    end
    if jpmode == 5 then
        jp.Text = "JumpPower:  Bounce into Heaven"
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 80000
    end
end
jp.MouseButton1Click:connect(jpp)

function spawnblock()
    if gothrough == false then
        gothrough = true
        sb.Text = "Noclip"
        local gc = game.Players.LocalPlayer.Character:GetChildren()
        for i = 1,#gc,1 do
            if (gc[i].ClassName == "Part") or (gc[i].ClassName == "MeshPart") then
            gc[i].CollisionGroupId = 29
            end
        end
        game:service("RunService").Stepped:wait()
    else
        gothrough = false
        sb.Text = "Noclip"
        local gc = game.Players.LocalPlayer.Character:GetChildren()
        for i = 1,#gc,1 do
            if (gc[i].ClassName == "Part") or (gc[i].ClassName == "MeshPart") then
            gc[i].CollisionGroupId = 1
            game:service("RunService").Stepped:wait()
            end
        end
    end
end
sb.MouseButton1Click:connect(spawnblock)
function looptelep()
    if lotptog == false then
        lotptog = true
        lotp.Text = "Loop-Teleport: ON"
        repeat
            game.Players.LocalPlayer.Character:MoveTo(game.Players:FindFirstChild(plr.Text).Character.PrimaryPart.Position)
            wait(0.001)
        until lotptog == false
    else
        lotptog = false
        lotp.Text = "Loop-Teleport: OFF"
    end
end
lotp.MouseButton1Click:connect(looptelep)


function minimi()
    scg.Enabled = false
    oc.Text = "Open"
end
minim.MouseButton1Click:connect(minimi)
	elseif text == "AUDIOGRABBER" then
		aa = game:GetObjects("rbxassetid://01997056190")[1]
aa.Parent = game.CoreGui
wait(0.2)
GUI = aa.PopupFrame.PopupFrame
pos = 0

ignore = {
	"rbxasset://sounds/action_get_up.mp3",
	"rbxasset://sounds/uuhhh.mp3",
	"rbxasset://sounds/action_falling.mp3",
	"rbxasset://sounds/action_jump.mp3",
	"rbxasset://sounds/action_jump_land.mp3",
	"rbxasset://sounds/impact_water.mp3",
	"rbxasset://sounds/action_swim.mp3",
	"rbxasset://sounds/action_footsteps_plastic.mp3"
}

GUI.Close.MouseButton1Click:connect(function()
	GUI:TweenSize(UDim2.new(0, 360, 0, 0),"Out","Quad",0.5,true) wait(0.6)
	GUI.Parent:TweenSize(UDim2.new(0, 0, 0, 20),"Out","Quad",0.5,true) wait(0.6)
	aa:Destroy()
end)

local min = false
GUI.Minimize.MouseButton1Click:connect(function()
	if min == false then
		GUI:TweenSize(UDim2.new(0, 360, 0, 20),"Out","Quad",0.5,true) min = true
	else
		GUI:TweenSize(UDim2.new(0, 360, 0, 260),"Out","Quad",0.5,true) min = false
	end
end)

function printTable(tbl)
	if type(tbl) ~= 'table' then return nil end
	local depthCount = -15

	local function run(val, inPrefix)
		depthCount = depthCount + 15
		-- if inPrefix then print(string.rep(' ', depthCount) .. '{') end
		for i,v in pairs(val) do
			if type(v) == 'table' then
				-- print(string.rep(' ', depthCount) .. ' [' .. tostring(i) .. '] = {')
				GUI.Store.Text = GUI.Store.Text..'\n'..string.rep(' ', depthCount) .. ' [' .. tostring(i) .. '] = {'
				run(v, false)
				wait()
			else
				-- print(string.rep(' ', depthCount) .. ' [' .. tostring(i) .. '] = ' .. tostring(v))
				GUI.Store.Text = GUI.Store.Text..'\n'..string.rep(' ', depthCount) .. ' [' .. tostring(i) .. '] = ' .. tostring(v)
				wait()
			end
		end
		-- print(string.rep(' ', depthCount) .. '}')
		depthCount = depthCount - 15
	end
	run(tbl, true)
end

function refreshlist()
	pos = 0
	GUI.Logs.CanvasSize = UDim2.new(0,0,0,0)
	for i,v in pairs(GUI.Logs:GetChildren()) do
		v.Position = UDim2.new(0,0,0, pos)
		GUI.Logs.CanvasSize = UDim2.new(0,0,0, pos+20)
		pos = pos+20
	end
end

function FindTable(Table, Name)
	for i,v in pairs(Table) do
		if v == Name then
			return true
		end end
	return false
end

function writefileExploit()
	if writefile then
		return true
	end
end

writeaudio = {}
running = false
GUI.SS.MouseButton1Click:connect(function()
	if writefileExploit() then
		if running == false then
			GUI.Load.Visible = true running = true
			GUI.Load:TweenSize(UDim2.new(0, 360, 0, 20),"Out","Quad",0.5,true) wait(0.3)
			for _, child in pairs(GUI.Logs:GetChildren()) do
				if child:FindFirstChild('ImageButton') then local bttn = child:FindFirstChild('ImageButton')
					if bttn.BackgroundTransparency == 0 then
						writeaudio[#writeaudio + 1] = {NAME = child.NAME.Value, ID = child.ID.Value}
					end
				end
			end
			GUI.Store.Visible = true
			printTable(writeaudio)
			wait(0.2)
			local filename = 0
			local function write()
				local file
				pcall(function() file = readfile("Audios"..filename..".txt") end)
				if file then
					filename = filename+1
					write()
				else
					local text = tostring(GUI.Store.Text)
					text = text:gsub('\n', '\r\n')
					writefile("Audios"..filename..".txt", text)
				end
			end
			write()
			for rep = 1,10 do
			GUI.Load.BackgroundTransparency = GUI.Load.BackgroundTransparency + 0.1
			wait(0.05)
			end
			GUI.Load.Visible = false
			GUI.Load.BackgroundTransparency = 0
			GUI.Load.Size = UDim2.new(0, 0, 0, 20)
			running = false
			GUI.Store.Visible = false
			GUI.Store.Text = ''
			writeaudio = {}
			game:FindService('StarterGui'):SetCore('SendNotification', {
				Title = 'Audio Logger',
				Text = 'Saved audios\n(Audios'..filename..'.txt)',
				Icon = 'http://www.roblox.com/asset/?id=176572847',
				Duration = 5,
			})
		end
	else
		game:FindService('StarterGui'):SetCore('SendNotification', {
			Title = 'Audio Logger',
			Text = 'Exploit cannot writefile :(',
			Icon = 'http://www.roblox.com/asset/?id=176572847',
			Duration = 5,
		})
	end
end)

GUI.SA.MouseButton1Click:connect(function()
	if writefileExploit() then
		if running == false then
			GUI.Load.Visible = true running = true
			GUI.Load:TweenSize(UDim2.new(0, 360, 0, 20),"Out","Quad",0.5,true) wait(0.3)
			for _, child in pairs(GUI.Logs:GetChildren()) do
				writeaudio[#writeaudio + 1] = {NAME = child.NAME.Value, ID = child.ID.Value}
			end
			GUI.Store.Visible = true
			printTable(writeaudio)
			wait(0.2)
			local filename = 0
			local function write()
				local file
				pcall(function() file = readfile("Audios"..filename..".txt") end)
				if file then
					filename = filename+1
					write()
				else
					local text = tostring(GUI.Store.Text)
					text = text:gsub('\n', '\r\n')
					writefile("Audios"..filename..".txt", text)
				end
			end
			write()
			for rep = 1,10 do
				GUI.Load.BackgroundTransparency = GUI.Load.BackgroundTransparency + 0.1
				wait(0.05)
			end
			GUI.Load.Visible = false
			GUI.Load.BackgroundTransparency = 0
			GUI.Load.Size = UDim2.new(0, 0, 0, 20)
			running = false
			GUI.Store.Visible = false
			GUI.Store.Text = ''
			writeaudio = {}
			game:FindService('StarterGui'):SetCore('SendNotification', {
				Title = 'Audio Logger',
				Text = 'Saved audios\n(Audios'..filename..'.txt)',
				Icon = 'http://www.roblox.com/asset/?id=176572847',
				Duration = 5,
			})
		end
	else
		game:FindService('StarterGui'):SetCore('SendNotification', {
			Title = 'Audio Logger',
			Text = 'Exploit cannot writefile :(',
			Icon = 'http://www.roblox.com/asset/?id=176572847',
			Duration = 5,
		})
	end
end)

selectedaudio = nil
function getaudio(place)
	if running == false then
		GUI.Load.Visible = true running = true
		GUI.Load:TweenSize(UDim2.new(0, 360, 0, 20),"Out","Quad",0.5,true) wait(0.3)
		for _, child in pairs(place:GetDescendants()) do
			spawn(function()
				if child:IsA("Sound") and not GUI.Logs:FindFirstChild(child.SoundId) and not FindTable(ignore,child.SoundId) then
					local id = string.match(child.SoundId, "rbxasset://sounds.+") or string.match(child.SoundId, "&hash=.+") or string.match(child.SoundId, "%d+")
					if id ~= nil then
						local newsound = GUI.Audio:Clone()
						if string.sub(id, 1, 6) == "&hash=" or string.sub(id, 1, 7) == "&0hash=" then
							id = string.sub(id, (string.sub(id, 1, 6) == "&hash=" and 7) or (string.sub(id, 1, 7) == "&0hash=" and 8), string.len(id))
							newsound.ImageButton.Image = 'rbxassetid://1453863294'
						end
						newsound.Parent = GUI.Logs
						newsound.Name = child.SoundId
						newsound.Visible = true
						newsound.Position = UDim2.new(0,0,0, pos)
						GUI.Logs.CanvasSize = UDim2.new(0,0,0, pos+20)
						pos = pos+20
						local function findname()
							Asset = game:GetService("MarketplaceService"):GetProductInfo(id)
						end
						local audioname = 'error'
						local success, message = pcall(findname)
						if success then
    						newsound.TextLabel.Text = Asset.Name
							audioname = Asset.Name
						else
							newsound.TextLabel.Text = child.Name
							audioname = child.Name
						end
						local data = Instance.new('StringValue') data.Parent = newsound data.Value = child.SoundId data.Name = 'ID'
						local data2 = Instance.new('StringValue') data2.Parent = newsound data2.Value = audioname data2.Name = 'NAME'
						local soundselected = false
						newsound.ImageButton.MouseButton1Click:Connect(function()
							if GUI.Info.Visible ~= true then
								if soundselected == false then soundselected = true
									newsound.ImageButton.BackgroundTransparency = 0
								else soundselected = false
									newsound.ImageButton.BackgroundTransparency = 1
								end
							end
						end)
						newsound.Click.MouseButton1Click:Connect(function()
							if GUI.Info.Visible ~= true then
								GUI.Info.TextLabel.Text = "Name: " ..audioname.. "\n\nID: " .. child.SoundId .. "\n\nWorkspace Name: " .. child.Name
								selectedaudio = child.SoundId
								GUI.Info.Visible = true
							end
						end)
					end
				end
			end)
		end
	end
	for rep = 1,10 do
		GUI.Load.BackgroundTransparency = GUI.Load.BackgroundTransparency + 0.1
		wait(0.05)
	end
	GUI.Load.Visible = false
	GUI.Load.BackgroundTransparency = 0
	GUI.Load.Size = UDim2.new(0, 0, 0, 20)
	running = false
end

GUI.All.MouseButton1Click:connect(function() getaudio(game)end)
GUI.Workspace.MouseButton1Click:connect(function() getaudio(workspace)end)
GUI.Lighting.MouseButton1Click:connect(function() getaudio(game:GetService('Lighting'))end)
GUI.SoundS.MouseButton1Click:connect(function() getaudio(game:GetService('SoundService'))end)
GUI.Clr.MouseButton1Click:connect(function()
	for _, child in pairs(GUI.Logs:GetChildren()) do
		if child:FindFirstChild('ImageButton') then local bttn = child:FindFirstChild('ImageButton')
			if bttn.BackgroundTransparency == 1 then
				bttn.Parent:Destroy()
				refreshlist()
			end
		end
	end
end)
GUI.ClrS.MouseButton1Click:connect(function()
	for _, child in pairs(GUI.Logs:GetChildren()) do
		if child:FindFirstChild('ImageButton') then local bttn = child:FindFirstChild('ImageButton')
			if bttn.BackgroundTransparency == 0 then
				bttn.Parent:Destroy()
				refreshlist()
			end
		end
	end
end)
autoscan = false
GUI.AutoScan.MouseButton1Click:connect(function()
	if autoscan == false then autoscan = true
		GUI.AutoScan.BackgroundTransparency = 0.5
		game:FindService('StarterGui'):SetCore('SendNotification', {
			Title = 'Audio Logger',
			Text = 'Auto Scan ENABLED',
			Icon = 'http://www.roblox.com/asset/?id=176572847',
			Duration = 5,
		})
	else autoscan = false
		GUI.AutoScan.BackgroundTransparency = 0
		game:FindService('StarterGui'):SetCore('SendNotification', {
			Title = 'Audio Logger',
			Text = 'Auto Scan DISABLED',
			Icon = 'http://www.roblox.com/asset/?id=176572847',
			Duration = 5,
		})
	end
end)

game.DescendantAdded:connect(function(added)
	wait()
	if autoscan == true and added:IsA('Sound') and not GUI.Logs:FindFirstChild(added.SoundId) and not FindTable(ignore,added.SoundId) then
		local id = string.match(added.SoundId, "rbxasset://sounds.+") or string.match(added.SoundId, "&hash=.+") or string.match(added.SoundId, "%d+")
		if id ~= nil then
			local newsound = GUI.Audio:Clone()
				if string.sub(id, 1, 6) == "&hash=" or string.sub(id, 1, 7) == "&0hash=" then
					id = string.sub(id, (string.sub(id, 1, 6) == "&hash=" and 7) or (string.sub(id, 1, 7) == "&0hash=" and 8), string.len(id))
					newsound.ImageButton.Image = 'rbxassetid://1453863294'
				end
				local scrolldown = false
				newsound.Parent = GUI.Logs
				newsound.Name = added.SoundId
				newsound.Visible = true
				newsound.Position = UDim2.new(0,0,0, pos)
				if GUI.Logs.CanvasPosition.Y == GUI.Logs.CanvasSize.Y.Offset - 230 then
					scrolldown = true
				end
				GUI.Logs.CanvasSize = UDim2.new(0,0,0, pos+20)
				pos = pos+20
				local function findname()
					Asset = game:GetService("MarketplaceService"):GetProductInfo(id)
				end
				local audioname = 'error'
				local success, message = pcall(findname)
				if success then
    				newsound.TextLabel.Text = Asset.Name
					audioname = Asset.Name
				else
					newsound.TextLabel.Text = added.Name
					audioname = added.Name
				end
				local data = Instance.new('StringValue') data.Parent = newsound data.Value = added.SoundId data.Name = 'ID'
				local data2 = Instance.new('StringValue') data2.Parent = newsound data2.Value = audioname data2.Name = 'NAME'
				local soundselected = false
				newsound.ImageButton.MouseButton1Click:Connect(function()
					if GUI.Info.Visible ~= true then
						if soundselected == false then soundselected = true
							newsound.ImageButton.BackgroundTransparency = 0
						else soundselected = false
							newsound.ImageButton.BackgroundTransparency = 1
						end
					end
				end)
				newsound.Click.MouseButton1Click:Connect(function()
					if GUI.Info.Visible ~= true then
						GUI.Info.TextLabel.Text = "Name: " ..audioname.. "\n\nID: " .. added.SoundId .. "\n\nWorkspace Name: " .. added.Name
						selectedaudio = added.SoundId
						GUI.Info.Visible = true
					end
				end)
				--230'
			if scrolldown == true then
				GUI.Logs.CanvasPosition = Vector2.new(0, 9999999999999999999999999999999999999999999, 0, 0)
			end
		end
	end
end)

GUI.Info.Copy.MouseButton1Click:Connect(function()
	if pcall(function() Synapse:Copy(selectedaudio) end) then
	else
		local clip = setclipboard or Clipboard.set
		clip(selectedaudio)
	end
	game:FindService('StarterGui'):SetCore('SendNotification', {
		Title = 'Audio Logger',
		Text = 'Copied to clipboard',
		Icon = 'http://www.roblox.com/asset/?id=176572847',
		Duration = 5,
	})
end)

GUI.Info.Close.MouseButton1Click:Connect(function()
	GUI.Info.Visible = false
	for _, sound in pairs(game:GetService('Players').LocalPlayer.PlayerGui:GetChildren()) do
		if sound.Name == 'SampleSound' then
			sound:Destroy()
		end
	end
	GUI.Info.Listen.Text = 'Listen'
end)

GUI.Info.Listen.MouseButton1Click:Connect(function()
	if GUI.Info.Listen.Text == 'Listen' then
		local samplesound = Instance.new('Sound') samplesound.Parent = game:GetService('Players').LocalPlayer.PlayerGui
		samplesound.Looped = true samplesound.SoundId = selectedaudio samplesound:Play() samplesound.Name = 'SampleSound'
		samplesound.Volume = 5
		GUI.Info.Listen.Text = 'Stop'
	else
		for _, sound in pairs(game:GetService('Players').LocalPlayer.PlayerGui:GetChildren()) do
			if sound.Name == 'SampleSound' then
				sound:Destroy()
			end
		end
		GUI.Info.Listen.Text = 'Listen'
	end
end)

function drag(gui)
	spawn(function()
		local UserInputService = game:GetService("UserInputService")
		local dragging
		local dragInput
		local dragStart
		local startPos
		local function update(input)
			local delta = input.Position - dragStart
			gui:TweenPosition(UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y), "InOut", "Quart", 0.04, true, nil)
		end
		gui.InputBegan:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
			dragging = true
			dragStart = input.Position
			startPos = gui.Position
		input.Changed:Connect(function()
            if input.UserInputState == Enum.UserInputState.End then
                dragging = false
            end
        end)
    end
end)
gui.InputChanged:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
        dragInput = input
    end
end)
UserInputService.InputChanged:Connect(function(input)
    if input == dragInput and dragging then
        update(input)
    end
end)
end)
end
drag(aa.PopupFrame)
        end
    end
)

uis.InputBegan:Connect(
    function(input)
        if (uis:GetFocusedTextBox()) then
            return -- make sure player's not chatting!
        end
        if input.KeyCode == Enum.KeyCode.KeypadOne then
            local poop = "9120789017" --id here
            local Event = game:GetService("Workspace")["DRadio_Script"].Event
            Event:FireServer(poop)
        end
        if input.KeyCode == Enum.KeyCode.KeypadTwo then
            local poop = "6654360741" --id here
            local Event = game:GetService("Workspace")["DRadio_Script"].Event
            Event:FireServer(poop)
        end
        if input.KeyCode == Enum.KeyCode.KeypadThree then
            local poop = "1885063716" --id here
            local Event = game:GetService("Workspace")["DRadio_Script"].Event
            Event:FireServer(poop)
        end
        if input.KeyCode == Enum.KeyCode.KeypadFour then
            local poop = "9120791512" --id here
            local Event = game:GetService("Workspace")["DRadio_Script"].Event
            Event:FireServer(poop)
        end
        if input.KeyCode == Enum.KeyCode.KeypadFive then
            local poop = "1885063716" --id here
            local Event = game:GetService("Workspace")["DRadio_Script"].Event
            Event:FireServer(poop)
        end
        if input.KeyCode == Enum.KeyCode.KeypadSix then
            local poop = "850314847" --id here
            local Event = game:GetService("Workspace")["DRadio_Script"].Event
            Event:FireServer(poop)
        end
        if input.KeyCode == Enum.KeyCode.KeypadSeven then
            local poop = "" --id here
            local Event = game:GetService("Workspace")["DRadio_Script"].Event
            Event:FireServer(poop)
        end
    end
)
