-- Configurações
local invulnerabilityEnabled = false -- Ativar ou desativar invulnerabilidade
local damageBoostEnabled = false -- Ativar ou desativar aumento de dano
local rapidHitsEnabled = false -- Ativar ou desativar ataques rápidos

-- Função para ativar/desativar invulnerabilidade
function toggleInvulnerability()
    invulnerabilityEnabled = not invulnerabilityEnabled
    print("Invulnerabilidade " .. (invulnerabilityEnabled and "ativada" or "desativada"))
end

-- Função para ativar/desativar aumento de dano
function toggleDamageBoost()
    damageBoostEnabled = not damageBoostEnabled
    print("Aumento de dano " .. (damageBoostEnabled and "ativado" or "desativado"))
end

-- Função para ativar/desativar ataques rápidos
function toggleRapidHits()
    rapidHitsEnabled = not rapidHitsEnabled
    print("Ataques rápidos " .. (rapidHitsEnabled and "ativados" or "desativados"))
end

-- Função principal
function main()
    while true do
        if invulnerabilityEnabled then
            -- Lógica para evitar dano
            -- Implemente aqui a lógica específica para evitar dano
        end

        if damageBoostEnabled then
            -- Lógica para aumentar o dano
            -- Implemente aqui a lógica específica para aumentar o dano
        end

        if rapidHitsEnabled then
            -- Lógica para ataques rápidos
            -- Implemente aqui a lógica específica para ataques rápidos
        end

        wait(0.5) -- Aguarda 0.5 segundos antes de verificar novamente
    end
end

-- Chamada da função principal
main()
