# Iris-Exploit-Bundle
Created by [Michael48](https://github.com/Michael-48), bundled by [me](https://github.com/x0581) for exploit usage

I am releasing this bundled version of Iris for Exploit Usage.
I am not the creator, I simply bundled it into a single file, and removed LuaU operators for compatibility.

Scripts I made with it:
* [Mike Explorer (Instance Viewer)](https://github.com/x0581/MikeExplorer)

Example Usage:
```lua
local Iris = loadstring(game:HttpGet("https://raw.githubusercontent.com/x0581/Iris-Exploit-Bundle/main/bundle.lua"))().Init(game.CoreGui)
Iris:Connect(Iris.ShowDemoWindow)
Iris:Connect(function()
    Iris.Window({"My First Window!"}) do
        Iris.Text({"Hello, World"})
        if Iris.Button({"Save"}).clicked then
            print("Clicked!")
        end
        Iris.InputNum({"Input"})
        Iris.End()
    end
end)
```
