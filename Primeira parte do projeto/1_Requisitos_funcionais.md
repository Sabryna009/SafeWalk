# Tabela de Requisitos Funcionais

## ✅ Funcionalidades do Projeto

| Funcionalidade                                        | Como o usuário vai usar                           | O que ela faz                                                                 | Tem algo que precise ser feito antes?                                  |
|-------------------------------------------------------|---------------------------------------------------|------------------------------------------------------------------------------|------------------------------------------------------------------------|
| [RF001] Ligar/Desligar o sistema                      | Através de um botão ou chave física               | Liga ou desliga o funcionamento do sistema                                   | Implementar botão e lógica de inicialização                            |
| [RF002] Detectar obstáculos                           | O usuário apenas utiliza a bengala normalmente    | O sensor ultrassônico mede a distância à frente do usuário                   | Calibrar o sensor e garantir alimentação da ESP32                      |
| [RF003] Emitir sinal de alerta com vibração           | O usuário sentirá a vibração automaticamente      | As vibrações são ativadas ao detectar obstáculos próximos                    | Programar a lógica de detecção e conectar os motores vibratórios       |
| [RF004] Aumento de frequência com proximidade         | O usuário perceberá aumento na vibração           | Quanto menor a distância, maior a frequência da vibração                     | Definir escalas de distância e intensidade na programação              |
| [RF005] Indicação de ausência de obstáculos           | Usando normalmente                                | Quando não há obstáculos, o sistema permanece silencioso ou sem vibração     | Definir zona de segurança no código                                    |
