# System Design

## Contexto

O exercício é projetar um sistema que permita aos usuários acompanharem os resultados de jogos de futebol (ou outro esporte à escolha).

## Requisitos

- **Autenticação**: Login não é uma necessidade primária.
- **Fontes de Dados**: Os resultados podem ser obtidos de diversas fontes, como FIFA, CBF, NFL, entre outras.
- **Retenção de Dados**: Os dados não precisam ser mantidos para além da duração da partida.
- **Consulta de Resultados**: Usuários podem visualizar os resultados mais recentes dos jogos. Deve ser possível filtrar os jogos por liga e time.
- **Escopo dos Dados**: Apenas o placar corrente deve ser exibido – outros eventos do jogo não serão considerados.
- **Tempo de Atualização**: O atraso máximo permitido para exibição dos resultados é de 60 segundos. No percentil P95, o tempo de espera máximo deve ser de 30 segundos.
- **Interface Web e Mobile**: O sistema deve oferecer um site responsivo e um aplicativo mobile para Android e iOS.
- **Alta Disponibilidade**: O sistema deve ser resiliente para lidar com picos de tráfego, especialmente em dias de jogos importantes.
- **Baixa Latência**: Os resultados devem ser atualizados em tempo real, sem necessidade de recarregar a página.
- **Escalabilidade**: A solução deve suportar o crescimento da base de usuários sem comprometer o desempenho.
