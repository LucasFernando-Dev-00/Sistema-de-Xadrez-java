# ♟️ Sistema de Xadrez (Chess System)

> Aplicação interativa em formato de console desenvolvida em Java, que implementa um motor de jogo de xadrez completo. O projeto utiliza de forma profunda os pilares da Programação Orientada a Objetos (POO) para gerenciar o tabuleiro, validar movimentos complexos em matrizes e aplicar todas as regras oficiais do jogo.

---

## 🚀 Sobre o Projeto

Este projeto foi desenvolvido com o objetivo de encarar um dos maiores desafios de lógica de programação: a construção de um jogo de estratégia por turnos estruturado em camadas. A aplicação abstrai o comportamento de um tabuleiro genérico de jogos de mesa (`boardgame`) e o especializa para as regras estritas e refinadas do xadrez internacional (`chess`).

### 🔑 Diferenciais Técnicos e Regras Implementadas

* **Lógica de Xeque e Xeque-Mate:** Monitoramento contínuo da posição do Rei em relação às peças adversárias, calculando automaticamente se há movimentos de fuga ou bloqueio válidos antes de declarar o fim da partida.
* **Jogadas Especiais Oficiais:**
  * **Roque (*Castling*):** Movimento duplo envolvendo o Rei e uma das Torres (tanto o Roque Pequeno quanto o Roque Grande), validando se as peças já se moveram ou se há ameaças no caminho.
  * **En Passant:** Captura especial de peão que avança duas casas na sua primeira jogada por um peão adversário na quinta fileira.
  * **Promoção de Peão:** Mecanismo que transforma o peão que atinge a oitava fileira em uma peça de maior poder (como a Rainha, Bispo, Cavalo ou Torre).
* **Sistema de Cores e Capturas:** Interface de console customizada com códigos de cores ANSI para diferenciar as peças brancas das amarelas/pretas, além de um painel de controle que exibe o turno atual, o jogador ativo e a lista de peças capturadas.

---

## 🛠️ Tecnologias e Ferramentas

* **Java SE (JDK):** Linguagem core utilizada para toda a modelagem matemática e lógica do motor do jogo.
* **Matrizes (Arrays Bidimensionais):** Estrutura de dados central utilizada para representar as posições 8x8 do tabuleiro.
* **IntelliJ IDEA:** IDE utilizada para o desenvolvimento e gerenciamento do projeto.

---

### Detalhes dos Pacotes:
* **`application`:** Controla a execução do programa e a interface de usuário direta via terminal (`UI.java`), garantindo que o motor do jogo e a tela fiquem independentes.
* **`boardgame`:** Um motor genérico de tabuleiro. Não conhece regras de xadrez, apenas sabe o que é uma matriz, uma posição genérica e se uma peça existe ou não no espaço.
* **`chess`:** Especialização do sistema. É aqui que as regras oficiais entram, herdando a estrutura do `boardgame` e injetando o comportamento, as peças e as exceções próprias do xadrez.

---

## 📌 Como Jogar e Executar

### Pré-requisitos
* Java JDK instalado (versão 11 ou superior).
* Um terminal com suporte a códigos de cores ANSI (como o Git Bash no Windows, ou o terminal nativo do Linux/Mac) para visualizar o tabuleiro colorido corretamente.















