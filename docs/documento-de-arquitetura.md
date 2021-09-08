# Documento de Arquitetura

## Histórico de revisão
  |Data|Versão|Alteração|Autor|  
  |----|------|---------|-----|  
  |10/08/2021|0.1|Abertura do documento de Arquitetura|Érico Maximiano Bandeira|
  |07/09/2021|0.2|Adição da introdução e Representação da arquitetura|Max Henrique Barbosa|


## 1. Introdução
### 1.1 Finalidade

Este documento apresenta uma visão geral abrangente da arquitetura do projeto Oráculo, utilizando de uma série de visões arquiteturais diferentes para ilustrar os diversos aspectos do sistema. Este projeto fora realizado na disciplina Métodos de Densenvolvimento de Software em conjunto com a disciplina Engenharia de Produto de Software, e possui como principal cliente a Polícia Civil do Estado de Goiás.

### 1.2 Escopo

Neste documento serão descritos os componentes de software, padrões arquiteturais adotados e *frameworks* escolhidos para o desenvolvimento do projeto que tem por objetivo a criação de um sistema que permita acesso e gerenciamento de metadados acerca de procesos que envolvam vários setores internos da Polícia Civil. O documento explora a fundo as características da arquitetura e como estas se relacionam com o projeto.


### 1.3 Definições, acrônimos e abreviações
|Abreviação|Significado|
|----------|-----------|
|FGA|Faculdade do Gama|
|MDS|Métodos de Desenvolvimento de Software|
|UNB|Universidade de Brasília|
|PC-GO|Polícia Civil do Estado de Goiás|
|Backend|Parte do sistema responsável por prover e organizar recursos para a interfáce do sistema|
|Frontend|Parte do sistema responsável por ser a interfáce entre o sistema e o usuário|
|API|Application Programming Interface|

### 1.4 Visão Geral

O presente documento faz o detalhamento e descrição de características da arquitetura escolhidas pela equipe de desenvolvimento para a solução no software do projeto Oráculo. Nele estará presente:

| |Tópico|Descrição|
|-|------|---------|
|1|Introdução| - |
|2|Representação Arquitetural| - |
|3|Metas e Restrições da Arquitetura| - |
|4|Visão dos Casos de Uso| - |
|5|Visão Lógica| - |
|6|Tamanho e Desempenho| - |
|7|Qualidade| - |

## 2. Representação da Arquitetura

A arquitetura utilizada contém dois ambientes diferentes para a nossa aplicação, o ambiente de controle de dados que é conhecido como API e um ambiente web para os usuarios, onde poderam registrar, iniciar e acompanhar o andamento de processos internos.

Com relação a API, o projeto **Oráculo** será desenvolvido utilizando uma arquitetura orientada a microserviços, que é utilizada para desenvolver uma aplicação como um conjunto de pequenos serviços, que funcionam com seu próprio processo. Cada serviço é desenvolvido em torno de um conjunto de regras de negócio específicas, e é implementado de forma independente.

 - Usuário, serviço responsável por conter as lógicas de autenticação e armazenar as informações dos usuários.
 - Processos, serviço responsável por manter as lógicas de armazenamento dos metadados e do histórico de alterações dos processos.

<!-- Adicionar imagem de representação -->

### 2.1 Tecnologias

#### NodeJs

O Node.js pode ser definido como um ambiente de execução Javascript server-side.

Isso significa que com o Node.js é possível criar aplicações Javascript para rodar como uma aplicação standalone em uma máquina, não dependendo de um browser para a execução, como estamos acostumados.
O principal motivo de sua adoção é a sua alta capacidade de escala. Além disso, sua arquitetura, flexibilidade e baixo custo, o tornam uma boa escolha para implementação de Microsserviços e componentes da arquitetura Serverless.

#### NextJs

O front-end será desenvolvido utilizando o framework NextJs. é uma estrutura da web de desenvolvimento front-end React de código aberto criada por Vercel que permite funcionalidades como renderização do lado do servidor e geração de sites estáticos para aplicativos da web baseados em React. É uma estrutura pronta para produção que permite que os desenvolvedores criem rapidamente sites JAMstack estáticos e dinâmicos

#### PostgreSQL

O PostgreSQL tem o papel de gerenciar os dados desses bancos de maneira organizada e eficaz, rodando e gravando todas as informações que ficam registradas nesses compartimentos de maneira relacional.


## 3. Metas e restrições de Arquitetura 

### 3.1 Metas
 - Compatibilidade com os principais browsers da atualidade: Mozilla Firefox, Google Chrome e Internet Explorer
 - Modularidade: o código deve ter baixo acoplamento e alta modularidade, para facilitar a manutenabilidade


### 3.2 Restrições
 - Banco de dados relacional PostgreSQL, pois o sistema deverá ser executado em produção
 - React: 

### 3.3 Requisitos não funcionais
-

## 4. Visão dos Casos de Uso
  
### 4.1 Diagrama de Casos de Uso

### 4.2 Atores de Casos de Uso
|Ator|Descrição|
|----|---------|
| - | - |

### 4.3 Descrições de Casos de Uso
|Épico|Caso de uso|Descrição|
|-----|-----------|---------|
|E1| - | - |
|E2| - | - |
|E3| - | - |
## 5. Visão Lógica
### 5.1 Diagrama de Pacotes

## 6. Tamanho e desempenho

## 7. Qualidade
  
## 8. Referências
 
 - Documentação do Postgre - https://www.postgresql.org/docs/
 - Documentação do NodeJs - https://nodejs.org/en/docs/
 - Documentação do NextJs - https://nextjs.org/