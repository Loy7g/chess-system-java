
# ♟️ Chess System Java

Uma aplicação Java de console que implementa um jogo de xadrez completo para dois jogadores. Regras clássicas estão presentes, como **en passant**, **promoção de peão**, **roque**, validação de xeque e xeque-mate, além de exibir o tabuleiro e capturas.

---

## 🛠️ Tecnologias usadas

- Java 17+
- Programação Orientada a Objetos
- Manipulação de terminal/texto

---

## 📁 Estrutura do Projeto

```text
src/
└── application/
    └── Program.java           # Classe principal com loop de jogo e interação no console
└── chess/
    ├── board/                 # Tabuleiro, posições (Bloco), lógica de movimentação
    ├── pieces/                # Classes por peça: King, Queen, Rook, Bishop, Knight, Pawn
    ├── exceptions/            # Tratamentos de erros (xeque ilegal, etc.)
    └── util/                  # Classes auxiliares para entrada e saída no console
```

---

## ▶️ Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Loy7g/chess-system-java.git
   cd chess-system-java
   ```

2. Compile o projeto:
   ```bash
   javac -d bin src/application/Program.java
   ```

3. Execute o jogo:
   ```bash
   java -cp bin application.Program
   ```

---

## 🎮 Como jogar

- O jogo apresenta o estado atual do tabuleiro no console.

  ![Screenshot 2025-06-09 010911](https://github.com/user-attachments/assets/97aae1b0-e890-4a24-aa54-0b605d803f8c)

- Informe o **ponto de origem** (ex: `e2`) e o **destino** (`e4`) para mover uma peça.

  ![Screenshot 2025-06-09 010614](https://github.com/user-attachments/assets/cd593d3f-c51d-4a1a-9fb9-4da28af69099)

- O sistema valida movimentos válidos, impede derrube ou movimento que deixa o rei em xeque.
- O jogo termina quando ocorre xeque-mate ou empate por falta de jogadas válidas.

---

## 📌 Regras implementadas

- Roque (pequeno e grande)
- Promoção de peão

  ![Screenshot 2025-06-09 010900](https://github.com/user-attachments/assets/7ebf03df-3d6e-48df-b461-180bc72608b8)

- En passant
- Checagem de xeque e xeque-mate
- Registro de peças capturadas

---
