-- Configurações
local acertarGolpes = true
local ganharXP = true
local causarDano = true
local sofrerDanoZero = true

-- Função para acertar 10 golpes em 1 segundo
function AcertarGolpes()
    while acertarGolpes do
        -- Coloque aqui o código para acertar golpes
        wait(0.1) -- Aguarde 0.1 segundo entre os golpes
    end
end

-- Função para ganhar 10000+ pontos de XP a cada inimigo eliminado
function GanharXP()
    game.Players.PlayerAdded:Connect(function(player)
        player.CharacterAdded:Connect(function(character)
            if ganharXP then
                -- Coloque aqui o código para conceder XP ao eliminar inimigos
            end
        end)
    end)
end

-- Função para dar 975+ de dano em qualquer coisa
function CausarDano()
    if causarDano then
        -- Coloque aqui o código para causar dano
    end
end

-- Função para sofrer 0 de dano de qualquer coisa
function SofrerDanoZero()
    if sofrerDanoZero then
        -- Coloque aqui o código para evitar sofrer dano
    end
end

-- Ativar ou desativar o script
game:GetService("UserInputService").InputBegan:Connect(function(input)
    if input.KeyCode == Enum.KeyCode.P then
        acertarGolpes = not acertarGolpes
        ganharXP = not ganharXP
        causarDano = not causarDano
        sofrerDanoZero = not sofrerDanoZero
    end
end)
