# 🎬 Sistema de Gestão do **CineMack**

Projeto – Algoritmos e Programação I (2º Bimestre)

Este repositório contém um sistema completo desenvolvido para o projeto do 2º bimestre da disciplina de **Algoritmos e Programação I**, cujo objetivo é simular a operação diária de um cinema fictício chamado **CineMack**.

O sistema foi criado utilizando apenas os conteúdos abordados em aula:
✔ variáveis
✔ listas
✔ funções
✔ estruturas condicionais
✔ laços de repetição (`for` e `while`)

Nenhum recurso avançado, dicionários ou bibliotecas externas foi utilizado.

---

## 📌 Funcionalidades Principais

### 🎟️ Venda de ingressos

O sistema permite a compra de três tipos de ingressos:

* **Meia**
* **Inteira**
* **VIP**

Os preços variam conforme o filme (R$ 20, R$ 15 e R$ 10).
Cada filme possui duas sessões e capacidades diferentes (50, 40 e 30 lugares).
A compra é feita de forma sequencial, ocupando as primeiras poltronas disponíveis.

### 🪑 Controle de poltronas

Para cada sessão, o programa:

* Exibe a quantidade de assentos disponíveis
* Registra poltronas ocupadas via lista (0 = livre, 1 = ocupada)
* Impede vendas acima da capacidade

### ⭐ Avaliação dos filmes

Após assistir ao filme, o usuário pode avaliá-lo com notas de **0 a 5 estrelas**.
O sistema armazena as avaliações e calcula a média final de cada filme.

### 📊 Relatório Final

Ao encerrar o dia, é exibido um relatório contendo:

* Número de ingressos vendidos por tipo e por sessão
* Receita total por categoria de ingresso
* Receita total de cada filme e do dia
* Média de avaliações
* Total de ingressos vendidos

Tudo calculado manualmente com listas e operações básicas.

---

## 🆕 Funcionalidade Extra Implementada: **Cancelamento de Ingressos**

Como funcionalidade adicional obrigatória, o sistema inclui um módulo totalmente funcional para **cancelamento de ingressos**.

### 🔄 Como funciona o cancelamento no sistema

* O usuário escolhe **filme**, **sessão** e **tipo de ingresso** (meia, inteira ou VIP)
* O sistema verifica se há ingressos daquele tipo registrados
* Cancela a quantidade solicitada
* Libera as poltronas correspondentes, substituindo `1 → 0`
* Atualiza o contador de ingressos vendidos
* Garante que nenhum valor negativo seja registrado

A lógica foi implementada apenas com listas e estruturas básicas, respeitando as regras do projeto.

---

## 🧩 Estrutura do Código

O programa é totalmente modularizado, contando com funções como:

* `menu()` – menu principal
* `assentos_disponiveis()` – retorna quantas poltronas estão livres
* `menu_compra_ingresso()` – controla o processo de compra
* `comprar_ingresso()` – registra a compra nas listas
* `menu_cancelar_ingressos()` – interface do cancelamento
* `cancelar_ingressos()` – remove assentos ocupados e atualiza contadores
* `avaliar()` – registra avaliações
* `relatorio()` – gera o relatório final completo

---

## 🛠️ Tecnologias

* **Python 3**
* Programação estruturada

---

## 🎯 Objetivo Educacional

Este projeto foi construído para praticar:

* Manipulação de listas
* Modularização do código
* Construção de menus interativos
* Controle de fluxo
* Simulação de sistemas reais usando apenas bases da programação
