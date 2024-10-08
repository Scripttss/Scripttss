-- Script para Mini City RP no Roblox
-- Certifique-se de estar usando o executor Delta

-- Função para teleportar o jogador para uma localização específica
function teleportar(x, y, z)
    local player = game.Players.LocalPlayer
    if player and player.Character then
        player.Character.HumanoidRootPart.CFrame = CFrame.new(x, y, z)
    end
end

-- Exemplo de uso: Teleportar para as coordenadas (100, 50, 100)
teleportar(100, 50, 100)

-- Função para dar dinheiro ao jogador
function darDinheiro(quantidade)
    local player = game.Players.LocalPlayer
    if player then
        player.leaderstats.Money.Value = player.leaderstats.Money.Value + quantidade
    end
end

-- Exemplo de uso: Dar 1000 de dinheiro ao jogador
darDinheiro(1000)
