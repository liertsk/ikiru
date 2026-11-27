# Ikiru

Projeto acadêmico de desenvolvimento de um jogo de sobrevivência com perspectiva top-down, desenvolvido em Godot como atividade da disciplina: Fundamentos de Sistema de Informação. O projeto utiliza *Eu Sou a Lenda*, de Richard Matheson, como obra de referência.

## Conceito

*Ikiru* é um jogo de sobrevivência top-down centrado na relação entre permanência, vontade e necessidade de sobreviver.

A experiência é estruturada em ciclos nos quais o jogador precisa administrar suas ações, explorar ambientes, obter recursos, lidar com ameaças e retornar à própria casa. A sobrevivência não depende apenas da capacidade de enfrentar perigos, mas também das decisões tomadas sobre quando agir, quanto tempo permanecer em determinado lugar e quais riscos aceitar.

A proposta busca explorar a tensão entre a preservação das condições necessárias para continuar vivo e os custos que essa própria preservação impõe ao personagem.

## Estrutura da experiência

O jogo combina três formas principais de interação:

- **Exploração local:** movimentação em espaços organizados em grids implícitos, com deslocamento por células e interação com elementos do ambiente.
- **Planejamento e deslocamento:** escolha de destinos e atividades por meio de um mapa geral e de opções contextuais.
- **Encontros e ameaças:** situações de perigo que podem exigir fuga, posicionamento ou combate.

A exploração local é baseada em movimentação discreta. Em ambientes sem ameaças, o jogador pode investigar e interagir com o espaço. Quando há inimigos, os deslocamentos passam a provocar respostas dos adversários, criando uma dinâmica de perseguição e posicionamento.

## Ciclo de jogo

O ciclo de jogo é organizado em torno da relação entre disponibilidade de ações, tempo de permanência e consequências das decisões.

A casa funciona como ponto de partida e retorno. A partir dela, o jogador pode selecionar destinos, realizar atividades e buscar recursos.

As expedições possuem custos de deslocamento e limites de permanência. O tempo gasto em um ambiente influencia as condições do retorno, enquanto determinadas ações podem consumir ou comprometer o tempo disponível.

Ao retornar, o jogador pode administrar recursos, tratar ferimentos e preparar a casa para o próximo período.

## Sistemas previstos para o MVP

O MVP pretende apresentar uma versão simplificada de todas as camadas fundamentais da experiência:

- **Movimentação por grid:** deslocamento discreto em quatro direções, com ocupação de células e obstáculos.
- **Interações contextuais:** pontos de interesse que apresentam opções de ações disponíveis.
- **Navegação entre ambientes:** casa, ambiente externo e mapa geral para seleção de destinos.
- **Gerenciamento de tempo:** disponibilidade diária de ações e temporizador de permanência nos ambientes.
- **Recursos:** coleta, utilização e administração de itens necessários à sobrevivência.
- **Inimigos:** comportamento básico de detecção, aproximação e perseguição.
- **Combate:** encontros em turnos com ações de ataque e defesa, acompanhadas de uma mecânica simples de timing.
- **Ferimentos:** consequências físicas específicas que afetam as capacidades do personagem e podem persistir entre os ciclos.
- **Tratamento:** utilização de recursos para lidar com ferimentos.
- **Preparação e defesa da casa:** administração simplificada de pontos vulneráveis e resposta a ameaças durante a noite.
- **Persistência:** manutenção de alterações relevantes nos ambientes, recursos, ferimentos e estado da casa entre os ciclos.

## Limites do MVP

O objetivo é demonstrar a integração entre os sistemas, não desenvolver uma simulação extensa de sobrevivência.

Por isso, o escopo inicial prioriza:

- Poucos ambientes, com funções bem definidas.
- Quantidade reduzida de recursos e interações.
- Comportamento limitado de inimigos.
- Combate com poucas ações e regras claras.
- Conjunto restrito de ferimentos e consequências.
- Defesa da casa baseada em poucas possibilidades de preparação.
- Um ciclo jogável que permita observar as consequências das decisões e a continuidade da experiência.

Sistemas complexos de geração procedural, grandes mapas, árvores extensas de habilidades, inventários elaborados e múltiplas categorias de inimigos não fazem parte das prioridades do MVP.

## Tecnologias

- **Engine:** Godot
- **Linguagem:** GDScript
- **Versionamento:** Git e GitHub

## Estrutura do projeto

```text
projeto/
├── addons/       # Extensões e plugins
├── assets/       # Recursos visuais, sonoros e fontes
├── docs/         # Documentação do projeto
├── resources/    # Recursos e configurações reutilizáveis
├── scenes/       # Cenas do jogo
└── scripts/      # Scripts e lógica do jogo
```

## Organização do desenvolvimento

O desenvolvimento é organizado por meio de GitHub Issues e GitHub Projects.

- `main`: versão estável do projeto.
- `dev`: branch de desenvolvimento.

As tarefas são divididas em etapas de planejamento, implementação do MVP, refinamento e entrega.

## Referência

*Eu Sou a Lenda*, de Richard Matheson.

O livro constitui a referência literária para o desenvolvimento conceitual do projeto.
