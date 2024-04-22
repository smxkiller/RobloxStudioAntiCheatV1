--------------------------------------------- ~Put In StarterCharchterScripts~
--           --//AniteCheatV1\\--        //||
--                  \_____               //||
--         _________/                    //||
--        /         \____________        //||
--       |  credits To BlazingCore\       //||
--        \_________/____________/       //||
--                  \_____               //||
--             _____/                    //||
--------------------------------------------- ~#BlazigCore On Discord~
Make Sure To Remove Credits--

How  Fly Works. it check for material that player standing on If Materail is Air Player Get Kicked -- You can make it ban
q: If Player fell from hight part He get banned?
--No He dont get Banned

-- Script Here --


--//Virablas\\---
local RunService = game:GetService("RunService")
local Player = game.Players.LocalPlayer
local LastGround = tick()
local hum = script.Parent:WaitForChild("Humanoid")
--//MainCode\\--
local function CheckFly()
	local humanoid = Player.Character:FindFirstChild("Humanoid")
	if humanoid then
		if humanoid.floorMaterial == Enum.Material.Air then
			if tick() - LastGround > 1 then
				Player:Kick("Deceted By AntiCheat If you Feel Its A Glitch Make A Ticket And Apeal!")
		    print("Kicked")
      else
            print("Error")
		 end
	  else
			LastGround = tick()
	  end
   end
end
--//Run!\\--
RunService.RenderStepped:Connect(CheckFly)
--//EndOfCode1\\--



--//Speed,Jump\\--anitecheat
while true do
	wait(1)
	if hum.WalkSpeed ~= 16 then
		game.Players.LocalPlayer:Kick("Deceted By AntiCheat If you Feel Its A Glitch Make A Ticket And Apeal!")
		print("Kicked")
	else
		print("Error")
	end
	end
if hum.jumpPower ~= 50 then
		game.Players.LocalPlayer:Kick("Deceted By AntiCheat If you Feel Its A Glitch Make A Ticket And Apeal!")
	print("kicked")
	else
	print("Error")	
	if hum.MaxHealth ~= 100 then
		game.Players.LocalPlayer:Kick("Deceted By AntiCheat If you Feel Its A Glitch Make A Ticket And Apeal!")
end
end
--//EndOfCode2\\--
