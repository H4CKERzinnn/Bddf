-- Carregar a biblioteca Kavo UI
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/KavoHub/KavoUI/main/source.lua"))()
local Window = Library.CreateLib("Hzin Vendas", "DarkTheme")

-- Aba Aimbot
local AimbotTab = Window:NewTab("Aimbot")
local AimbotSection = AimbotTab:NewSection("Memory Features")

AimbotSection:NewToggle("Aimbot Legit", "Aimbot mais suave e legit", function(state)
    print("Aimbot Legit:", state)
end)

AimbotSection:NewToggle("Aimbot Rage (TESTE)", "Aimbot forte e rápido", function(state)
    print("Aimbot Rage:", state)
end)

AimbotSection:NewButton("Camera Direita (F2)", "Ativa a câmera à direita", function()
    print("Câmera Direita ativada")
end)

AimbotSection:NewButton("Wall Hack (F3)", "Ativa Wall Hack", function()
    print("Wall Hack ativado")
end)

local AimbotConfigSection = AimbotTab:NewSection("Aimbot Configs")
AimbotConfigSection:NewSlider("Distância", "Alcance do Aimbot", 500, 50, function(value)
    print("Distância do Aimbot:", value)
end)

-- Aba Visuals
local VisualsTab = Window:NewTab("Visuals")
local VisualsSection = VisualsTab:NewSection("Em breve...")
VisualsSection:NewLabel("Ainda sem configurações visuais.")

-- Aba Configs
local ConfigsTab = Window:NewTab("Configs")
local ConfigsSection = ConfigsTab:NewSection("Ajustes Gerais")
ConfigsSection:NewLabel("Você pode colocar configs salvas aqui.")
