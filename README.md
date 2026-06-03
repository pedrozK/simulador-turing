# Simulador de Máquina de Turing de Fita Dupla

Este é um simulador web moderno de uma **Máquina de Turing com duas fitas infinitas independentes**. O projeto foi desenvolvido utilizando **React**, **TypeScript** e **Vite**, garantindo um ambiente de execução rápido, fortemente tipado e com alto desempenho.

---

## Objetivo e Inspiração

O projeto nasceu da admiração pelo clássico simulador de Máquina de Turing do Instituto de Informática da UFRGS (disponível em: [inf.ufrgs.br/~rma/simuladores/turing.html](https://www.inf.ufrgs.br/~rma/simuladores/turing.html)). 

Aliando o respeito por essa ferramenta acadêmica ao desejo do grupo de compreender a arquitetura de aplicações web baseadas em renderização e atualização dinâmica de estados, decidimos propor e implementar uma versão expandida: uma máquina síncrona de **fita dupla**.

---

## Principais Obstáculos Superados

* **Curva de Aprendizado:** Período de adaptação rápida com o ecossistema do React e a rigidez do TypeScript por parte dos membros do grupo.
* **Crescimento Exponencial da Matriz:** O maior desafio de usabilidade do projeto. A duplicação da fita gera uma explosão combinatória de colunas na tabela de transição ($N \times N$ combinações para um alfabeto de tamanho $N$).
* **Arquitetura de Software:** Separação estrita entre a interface do usuário (Frontend) e o motor de inferência matemática (Lógica), evitando acoplamento e conflitos no repositório.

---

## Divisão de Responsabilidades

* **Pietro (Frontend):** Responsável pela interface visual, gerenciamento de estados do HTML, comportamento reativo dos componentes e a implementação do mecanismo de contração/expansão de colunas no arquivo `src/App.tsx`.
* **Leonel (Lógica Matemática):** Responsável pela modelagem da máquina abstrata, controle dos cabeçotes de leitura/escrita e processamento das regras de transição na memória do sistema no arquivo `src/logicaTuring.ts`.
* **Pedro (Full-Stack & DevOps):** Responsável pela criação, conteinerização e gerência do ambiente de desenvolvimento. Atuou como facilitador entre as duas frentes, desenvolvendo a estilização visual dos elementos no Frontend, auxiliando na lógica matemática e implementando de ponta a ponta o sistema de persistência (salvamento e carregamento de arquivos de configuração da máquina).

---
