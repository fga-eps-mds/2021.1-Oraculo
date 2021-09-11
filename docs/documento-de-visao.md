# Documento de Visão

## 1. Introdução

Este documento tem o propósito de apresentar de forma geral e clara, o objetivo do projeto, algumas definições e formas de resolver os problemas propostos.

### 1.1. Propósito

O projeto tem o intuito de auxiliar no trabalho de alguns setores da GIPC-GO. Demandas que chegam para estes setores são todas processadas de várias origens diferentes, e são acompanhadas usando planilhas ou outros meios que facilitam o erro humano, como o re-trabalho de algumas demandas, podendo atrasar o trabalho. Por isso o intuito é facilitar e agilizar esse processo de trabalho da GIPC-GO.

### 1.2. Escopo

O escopo do projeto está associado a necessidade da GIPC-GO em armazenar dados sobre a tramitação de processos, sabendo de onde é a sua origem, quais as seçoes que já passou, e onde se encontra atualmente, sem a necessidade de vasculhar planilhas ou pastas todos os dias para dar sequência a uma demanda que chegue até a GIPC-GO.

### 1.3. Definições, acrônimos e abreviações
- Oráculo - Sistema de Gerenciamento de Tramitação de Documentos. 
- FGA - Faculdade do Gama.
- UnB - Universidade de Brasília.
- MDS - Métodos de Desenvolvimento de Software.
- EPS - Engenharia de Projeto de Software.
- GIPC-GO - Gerência de Identificação da Polícia Civil do Estado de Goiás
- Processos - Formas a qual se solicita um serviço oferecido pela GIPC-GO, sendo um serviço administrativo.
- Plataforma - Referência para o produto que está sendo desenvolvido.
- Front-end - É a camada do software no qual o cliente tem contato, no caso é o website que será utilizado pelo usuário final
- Back-end - É a camada do software no qual o usuário não terá acesso diretamente, esta camada é onde será guardado os dados, e é consumida pelo Front-end
- framework - O framework é um conjunto de códigos genéricos e básicos usados como um pacote por desenvolvedores.
- ReactJs - framework utilizado para o desenvolvimento do Front-end
- NodeJs - framework utilizado para o desenvolvimento do Back-end
- PO's - Donos do produto (Product Owners) são os usuários que estão em contato direto com o grupo de gestão e de desenvolvimento


### 1.4. Visão geral
Esse documento é dividido em 7 seções. A introdução compõem o escopo e o propósito do projeto dado a situação da GIPC-GO.

A seções do posicionamento revela as oportunidades de negócio por trás do produto e explica o problema a ser solucionado.

O terceiro tópico, visa passar pelas necessidades dos usuários e elaborar a definição de requisitos.

A visão geral do produto fornece uma visão em alto nível das capacidades do produto, mostrando uma perspectiva do produto e suas funções.

Na quinta seção, o recursos do produto lista os recursos do produto. Cada subtópico dessa seção  inclui uma descrição e o problema que deve solucionar.

A sexta seção, observam-se as restrições de design e as retrições externas, como requisitos operacionais ou regulamentares.

O último e o sétimo tópico, aprensenta nossas referências que ajudaram no processo de elaboração do documento.

## 2. Posicionamento

### 2.1. Oportunidade de negócio
O Oráculo tem como principal objetivo diminuir as chances de erro causados pelos servidores da atual GIPC-GO, agregando no rendimento e na organização dos funcionários centralizando as informações a cerca de seus processos em um único sistema. Além disso, conseguir manter os metadados dos processos garente uma rastreabilidade impedindo o re-trabalho, e possíveis perdas de dados em documentos importantes. Assim provendo uma melhora de agilidade e facilidade para acompanhamentos de processos.


### 2.2. Instrução do problema
Os servidores da GIPC-GO, no presente momento, sofrem com a questão de organização dos processos e o compartilhamento intuitivo e adequado dos mesmo. Atualmente o compartilhamento e a rastreabilidade destes processos ainda são feitos a partir de planilhas em excel ou mensagens por email, faltando padronização e mecanismo de busca para aquisição de dados.

Visto que o problema está ligado principalmente ao acesso e a perda de dados. O Oráculo gerência e padroniza a forma que o serviço é feito. Assim, nosso produto simplifica e acelera o trabalho dos agentes.

### 2.3. Instrução de Posição do produto

Atualmente os servidores que trabalham na GIPC-GO possui várias planilhas e pastas distintas para organizar seus documentos, geralmente cada repositório é individual ao setor para onde é destinado. Dessa forma fazendo com que a organização, acesso e acompanhamento daquele processo por outro setor seja prejudicado, provocando uma certa demora paradar continuidade, causando algumas vezes re-trabalho com um mesmo processo (duplicidade).

O produto proposto tem como objetivo de centralizar as demandas, e facilitar o acesso a esses dados por qualquer setor que tenha alguma relação com o processo.

## 3. Descrições da Parte Interessada e do Usuário

### 3.1 Resumo da Parte Interessada:

Grupo     | Descrição   | Responsabilidade 
:-------: | :------: | :------:
Equipe de Gestão do Projeto | Alunos da disciplina de EPS, FGA-UnB | Gerenciar e direcionar a equipe de desenvolvimento e documentar o projeto.
Equipe de Desenvolvimento   | Alunos da disciplina de MDS, FGA-UnB | Desenvolver, testar e documentar um produto final que supra as necessidades do cliente.
Professor | Professor das disciplinas EPS e MDS FGA-UnB | Avaliar e orientar os trabalhos desenvolvidos pela Equipe de MDS e EPS.
GIPC-GO   | Servidores que trabalham na GIPC-GO | Orientar e dar a visão sobre o produto.


### 3.2 Resumo do Usuário:
Grupo     | Descrição   | Responsabilidade 
:-------: | :------: | :------:
Funcionário GIPC-GO | Servidores da GIPC-GO | Acompanhar e atender as demandas de processos.
Admin | Representa o administrador de um setor | Administra e tem acesso a todas as demandas em andamento e históricos daquele setor. 


## 4. Visão Geral do Produto

### 4.1 Perspectiva do Produto:
Os funcionários da GIPC-GO não possuem um software de uso próprio para auxiliá-los em todas suas necessidades e para este fim o Oráculo foi criado. Ele é um website que auxilia os funcionários da GIPC-GO a realizar o acompanhamento e gerenciamento, rastreabilidade, e centralização da tramitação de processos recebidos pela GIPC-GO a fim de agilizar a realização de tarefas.

### 4.2 Resumo das capacidades:

**Benefícios para o Usuário**     | **Recursos de Suporte**
----------------------------------|--------------------
Padronizar o forma de trabalho    | Aplicação com várias funcionalidades que cobrem suas necessidades
Evitar perda de dados             | Banco de dados para armazenar documentos
Agilizar a análise de dados       | Mecanismo de busca no site

&nbsp;

**Benefícios para o Cliente**     | **Recursos de Suporte**
----------------------------------|--------------------
Maior satisfação do Cliente       | Centralização dos dados
Impede que haja a criação de um mesmo processo que já havia siado aberto       | Identificadores garantem isso nos processos


## 5. Recursos do Produto

### 5.1. Adicionar processo
É uma das principais funções da aplicação, o usuário pode cadastrar o processo no site e acessar os dados cadastrados do mesmo. 

### 5.2. Histórico de Processos
Essa funcionalidade permite ao usuário um controle mais amplo dos processos para visualizar seu estado atual e confirmar eventos posteriores.

### 5.3. Filtragem de processos
A filtragem de processos é um mecanismo de busca para facilitar o acesso de informações feitas pelo usuário.

### 5.4. Criar tag
A criacação de uma tag para facilitar o acompanhamento e organização interna de um setor.

### 5.5. Adicionar tag
É uma das principais funções da aplicação, o usuário pode cadastrar uma tag como marcador em um processo no site e acessar os dados a partir da tag. 

### 5.6. Filtragem de tag
A filtragem de tag é um mecanismo de busca para facilitar o acesso de informações feitas pelo usuário.

### 5.7. Admin
Usuário de um respectivo setor que possui permissão para criação de um usuário vinculado ao seu setor.

## 6. Restrições

Para o design a equipe de gestão do projeto em conjunto com a equipe de desenvolvimento deverão seguir a paleta de cores e o protótipo, que foram validados pelo PO e pelos clientes do projeto.
Para restrição de segurança, e até de uso, a plataforma permite que usuários sejam cadastrados por administradores, os usuários que serão cadastrados como funcionários da GIPC-GO que irão poder editar, apenas, de processos vinculados ou enviados para o seu setor. Apenas o admin pode criar campos para processos. Restrição para implementação, o grupo em conjunto decidiu centralizar as plataformas usando Javascript, com os frameworks Reactjs para o Front-end e Nodejs para o Back-end.

## 7. Referências
IBM Knowledge Center - Documento de Visão: Estruturas de um Documento de Visão.

Disponível em: https://www.ibm.com/docs/pt-br/elm/7.0.1?topic=requirements-vision-document

Acesso em: 11 de Setembro de 2021.