

##  Análise do Código
O código é uma implementação sólida do "Guessing Game" em Rust. Pontos principais:
1. **Gerenciamento de Dependências:** O uso de `rand::Rng` exige a configuração do `Cargo.toml`.
2. **Robustez:** O uso de `match` com `parse().Ok/Err` evita que o programa pare caso o usuário digite algo inválido (letras, símbolos).
3. **Idiomatismo:** O uso de `Ordering` é a forma mais eficiente e "limpa" de realizar comparações em Rust.
4. **UX:** O loop é bem estruturado, com uma saída clara (`break`) no acerto.

---

# Jogo: Adivinhe o Número (Guess the Number)

Este é um jogo simples de linha de comando onde o objetivo é adivinhar um número secreto gerado aleatoriamente pelo computador.

##  Pré-requisitos
Certifique-se de ter o **Rust** e o **Cargo** instalados.

##  Configuração Inicial
1. Crie o projeto:
   `cargo new adivinhe_numero`
   `cd adivinhe_numero`

2. Adicione a dependência no arquivo `Cargo.toml`:
   [dependencies]
   rand = "0.3.23"

3. Substitua o conteúdo de `src/main.rs` pelo código fornecido.

##  Execução
Para rodar o jogo, use o comando:
`cargo run`

##  Como Jogar
- O computador escolhe um número entre 1 e 100.
- Você digita seu palpite.
- O jogo informa se o chute foi "Too low!" (Muito baixo) ou "Too high!" (Muito alto).
- O jogo termina quando você acertar o número exato!

---
## Referência e Créditos
Este projeto foi desenvolvido seguindo o tutorial oficial do livro de Rust, traduzido pela comunidade **Rust-BR**:
* [Tutorial do Jogo de Adivinhação - Rust Book (PT-BR)](https://rust-br.github.io/rust-book-pt-br/ch02-00-guessing-game-tutorial.html)
*Projeto criado para fins de estudo da linguagem Rust.*

