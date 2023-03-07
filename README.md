while true do
	wait(0.01)
	local args = {
    [1] = 2,
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 15
    }
}

game:GetService("ReplicatedStorage"):WaitForChild("Project"):WaitForChild("RemoteEvent"):WaitForChild("ControlMessageEvent"):FireServer(unpack(args))

end
