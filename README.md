# 📌 PAC - 6ª Fase  **DRAFT**

## 📖 Sobre a Disciplina  
O **PAC da 6ª fase** é uma disciplina prática onde os alunos desenvolvem um projeto de software aplicando conceitos de:  
- **Análise, Projeto e Construção Ágil**  
- **Algoritmos Avançados**  
- **Inteligência Artificial**  
- **Manutenção e Melhoria de Software**  

Neste semestre, o desafio é criar uma **ferramenta CLI** que auxilie no ciclo de manutenção e qualidade de código.  

## 🎯 Objetivo do Projeto  
Os alunos deverão, em duplas, desenvolver uma **ferramenta de análise de código**. 

As analise que a ferramenta deve suportar, não sendo uma lista exaustiva, contempla:  


## 🔹 Ordem de Implementação  

| **#** |**Funcionalidade** | **Justificativa** | 
|------|----------------------|------------------|
|  1.1 | **Contagem de Linhas de Código (LOC)** | Simples pois apenas lê o arquivo e conta linhas de código e comentários. Não exige análise sintática profunda. |  
|  1.2 | **Contagem de Funções e Classes** | Exige parsing básico do código para detectar padrões como `def`, `class` ou `{}`. Pode ser feito com expressões regulares. | 
|  1.3 | **Linhas de Comentário** |  Número de linhas de documentação/comentário.|
|  2.1 | **Níveis de Indentação** | Pode ser feito contando tabulações/espaços por linha. Exige pouca lógica, mas requer atenção para diferentes estilos de código. |
|  2.2 | **Número de Dependências Externas** | Exige leitura e análise dos imports no código, podendo variar conforme a linguagem. Simples, mas requer um parser para `import` e `require()`. |
|  2.3 | **Proporção Comentário/Código** | Percentual de código comentado com relação ao total de linhas do codigo. Deve ser gerado por Unidade de código |
|  2.4 | **Número de Métodos Privados/Públicos**  | Mede a quantidade de métodos privados e públicos em uma classe. Ajuda a avaliar o nível de encapsulamento e modularidade do código. |
|  3.1 | **Tamanho Médio das Funções** | Extensão da contagem de funções, somando as linhas de cada uma e dividindo pelo total. Ainda simples, pois usa análise estrutural básica. |
|  3.2 | **Identificação de Código Duplicado** | Moderado, pois exige análise de trechos de código para encontrar padrões repetidos. Pode ser implementado comparando hashes de blocos de código. |
|  3.3 | **Predição de Bugs com IA** | Submter trechos de código para uma API de LLM solicitando sugestões de melhoria, indicações de problemas e etc. |
|  3.4 | **Análise Assintotica das Funções** | técnica usada para estudar o comportamento da complexidade de um algoritmo conforme o tamanho da entrada cresce. |
|  A.1 | **Identificação de Código Morto** | Complexo, pois requer análise de fluxo de execução para detectar funções e classes não utilizadas. Pode exigir análise do Abstract Syntax Tree (AST). |
|  A.2 | **Análise Ciclomática do Código** | Extremamente complexa, pois exige a construção de um grafo de fluxo de controle e cálculo da quantidade mínima de caminhos independentes, demandando análise profunda do código. |


# 📌 Perspectiva de Avaliação

A avaliação do trabalho será baseada na **entrega progressiva das funcionalidades** e na **demonstração prática** do CLI.  
 
- Cada dupla deve selecionar uma linguagem para o qual o CLI será focado. 
- **Para N1 e N2**, os alunos devem apresentar **exemplos de uso do CLI**, demonstrando suas funcionalidades.  
- **Para N3**, o projeto deve estar **integrado a um pipeline de CI/CD** (sugestão: utilizar **GitHub Actions**).


---

## 📌 Critérios de Avaliação  

Cada nível da avaliação segue a seguinte estrutura:  

### 🟢 N1 (Primeira Entrega)  
- **Nota 6.0:** Implementar **1 funcionalidade**.  
- **Nota 8.0:** Implementar **2 funcionalidades**.  
- **Nota 10.0:** Implementar **todas as funcionalidades** previstas para N1.  

### 🟡 N2 (Segunda Entrega)  
- **Nota 6.0:** Implementar **2 funcionalidades**.  
- **Nota 7.0:** Implementar **3 funcionalidades**.  
- **Nota 8.0:** Implementar **4 funcionalidades**.  
- **Nota 9.0:** Implementar **5 funcionalidades**.  
- **Nota 10.0:** Implementar **6 funcionalidades**. 

### 🔴 N3 (Terceira Entrega)  
- **Nota 6.0:** Ter pelo menos **5 funcionalidades concluídas** (somando N1, N2 e N3).  
- **Nota 7.0:** Ter pelo menos **6 funcionalidades concluídas** (somando N1, N2 e N3).  
- **Nota 8.0:** Ter pelo menos **7 funcionalidades concluídas** (somando N1, N2 e N3).  
- **Nota 9.0:** Ter pelo menos **8 funcionalidades concluídas** (somando N1, N2 e N3).  
- **Nota 10.0:** Ter pelo menos **8 funcionalidades concluídas + 1 funcionalidade avançada**.  

---

## 📌 Observações Finais  

- Funcionalidades avançadas incluem **predição de bugs com IA, análise ciclomatica ou qualquer outra métrica de alto nível**.  
- A documentação e a qualidade do código também serão consideradas na avaliação.  
- Projetos com **baixa qualidade de código ou sem funcionamento adequado podem perder pontuação**, mesmo que tenham o número mínimo de funcionalidades entregues.  

📌 *Recomenda-se que as equipes adotem boas práticas desde o início e realizem testes para validar suas implementações.* 🚀  




## 🏗️ Tecnologias Sugeridas  
- **Linguagem:** Python, Java, JavaScript, Go ou .Net  
- **Bibliotecas:** AST, Pylint, ESLint, SonarQube API  
- **IA/ML:** TensorFlow, PyTorch, Hugging Face  
- **Pipelines:** GitHub Actions, GitLab CI/CD, Azure DevOps  


## 📅 Cronograma de Entregas  
| Entrega | Descrição | Data |
|---------|------------|------|
| **N1** | CLI básico para análise de código | 20/03/2025 |
| **N2** | Cli avançado para analise de código | 15/05/2025 |
| **N3** | Integração com IA para suporte a análise e pipelines de CI/CD | 26/06/2025 |

