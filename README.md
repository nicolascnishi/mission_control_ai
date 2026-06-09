🚀 Mission Control AI
Sistema Inteligente de Monitoramento de Missão Espacial
Desenvolvido para a GS2026.1 - Pensamento Computacional e Automação com Python
📋 Sobre o Projeto
O Mission Control AI é um sistema computacional desenvolvido em Python que simula o monitoramento inteligente de uma missão espacial experimental. O sistema analisa dados de diferentes ciclos de operação, identifica riscos, emite alertas automáticos e gera um relatório completo com a situação da missão.
Missão Simulada: Orion Test Alpha
A missão simula o acompanhamento da cápsula espacial Órion em uma operação de teste experimental, monitorando parâmetros críticos para a segurança da tripulação e dos sistemas.
🛰️ Áreas Monitoradas
| # | Área                     | Parâmetro    | Unidade |
| - | ------------------------ | ------------ | ------- |
| 0 | Temperatura interna      | Temperatura  | °C      |
| 1 | Comunicação com a base   | Comunicação  | %       |
| 2 | Sistema de energia       | Bateria      | %       |
| 3 | Suporte de oxigênio      | Oxigênio     | %       |
| 4 | Estabilidade operacional | Estabilidade | %       |

⚠️ Regras de Alerta
Temperatura
| Condição        | Classificação |
| --------------- | ------------- |
| < 18 °C         | ATENÇÃO       |
| 18 °C a 30 °C   | NORMAL        |
| > 30 °C a 35 °C | ATENÇÃO       |
| > 35 °C         | CRÍTICO       |

Comunicação
| Condição  | Classificação |
| --------- | ------------- |
| < 30%     | CRÍTICO       |
| 30% a 59% | ATENÇÃO       |
| ≥ 60%     | NORMAL        |

Bateria
| Condição  | Classificação |
| --------- | ------------- |
| < 20%     | CRÍTICO       |
| 20% a 49% | ATENÇÃO       |
| ≥ 50%     | NORMAL        |

Oxigênio
| Condição  | Classificação |
| --------- | ------------- |
| < 80%     | CRÍTICO       |
| 80% a 89% | ATENÇÃO       |
| ≥ 90%     | NORMAL        |

Estabilidade
| Condição  | Classificação |
| --------- | ------------- |
| < 40%     | CRÍTICO       |
| 40% a 69% | ATENÇÃO       |
| ≥ 70%     | NORMAL        |

📊 Sistema de Pontuação de Risco
| Classificação | Pontuação |
| ------------- | --------- |
| NORMAL        | 0 ponto   |
| ATENÇÃO       | 1 ponto   |
| CRÍTICO       | 2 pontos  |

Classificação do Ciclo:
0 a 2 pontos → MISSÃO ESTÁVEL
3 a 5 pontos → MISSÃO EM ATENÇÃO
6 a 10 pontos → MISSÃO CRÍTICA
🔄 Ciclos de Monitoramento
A missão foi simulada com 6 ciclos de monitoramento:
| Ciclo | Descrição                    |
| ----- | ---------------------------- |
| 1     | Início da missão             |
| 2     | Estabilização dos sistemas   |
| 3     | Queda parcial de comunicação |
| 4     | Alerta de energia            |
| 5     | Risco operacional            |
| 6     | Tentativa de recuperação     |

Dados Simulados
dados_missao = [
    [24, 92, 88, 96, 90],   # Ciclo 1
    [27, 80, 72, 94, 85],   # Ciclo 2
    [31, 65, 58, 91, 70],   # Ciclo 3
    [36, 42, 38, 87, 55],   # Ciclo 4
    [39, 28, 19, 78, 35],   # Ciclo 5
    [34, 55, 32, 82, 50]    # Ciclo 6
]
🧠 Funções do Sistema
O sistema possui mais de 10 funções organizadas em módulos:
Funções de Análise Individual
analisar_temperatura() - Analisa temperatura interna
analisar_comunicacao() - Analisa qualidade da comunicação
analisar_bateria() - Analisa nível de bateria
analisar_oxigenio() - Analisa nível de oxigênio
analisar_estabilidade() - Analisa estabilidade operacional
Funções de Classificação e Decisão
classificar_ciclo() - Classifica o ciclo com base na pontuação
gerar_recomendacao() - Gera recomendações automáticas
analisar_tendencia() - Analisa tendência da missão
identificar_area_mais_afetada() - Identifica área com maior risco
gerar_relatorio_final() - Gera relatório completo
Função Principal
executar_sistema() - Executa o fluxo completo do sistema

🚀 Como Executar
Pré-requisitos
Python 3.x instalado
Execução
python mission_control.py

📈 Exemplo de Saída
O sistema exibe no terminal:
Análise detalhada de cada ciclo
Pontuação de risco por ciclo
Classificação do ciclo
Recomendações automáticas
Relatório final com:
Médias de todos os parâmetros
Ciclo mais crítico
Risco médio
Tendência da missão
Pontuação acumulada por área
Área mais afetada
Classificação final
Conclusão

👥 Equipe
Equipe: Equipe Apollo
Missão: Orion Test Alpha

📝 Tecnologias Utilizadas
Python 3 - Linguagem de programação
Estruturas de dados: Listas e Matrizes
Estruturas de controle: Repetição (for) e Condicionais (if/elif/else)
Funções: Organização modular do código
Lógica de decisão: Regras baseadas em limites predefinidos

📚 Requisitos Atendidos
✅ Nome da missão e equipe
✅ Matriz dados_missao com 6+ ciclos
✅ 5 informações por ciclo na ordem correta
✅ Lista de áreas monitoradas
✅ 10+ funções bem definidas
✅ Estrutura de repetição para percorrer ciclos
✅ Estruturas condicionais para alertas
✅ Cálculo de risco por ciclo
✅ Classificação de cada ciclo
✅ Análise de tendência da missão
✅ Identificação da área mais afetada
✅ Relatório final no terminal
✅ README.md completo
📄 Licença
Projeto desenvolvido para fins acadêmicos na FIAP.
