# Rubrica

A rubrica deste projeto é dividida por grupos apresentados abaixo. 

## Setup do projeto

| Grupo | Requisito | Data de entrega | Conceito | 
|-------|-----------|-----------------|----------|
| Estrutura da Equipe | [Definição da estrutura da equipe](./requisitos.md#estrutura-da-equipe) | 18/11 | D |
| Compreensão do problema | [Entrega do documento de compreensão do problema em markdown no repositório do projeto](./requisitos.md#compreensão-do-problema) | 22/11 | D |
| Modelagem | [Entregar o documento com perguntas sobre CNN em markdown no repositório do projeto](./requisitos.md#modelagem) | 22/11 | D |
| Análise exploratória de dados | [Entrega do relatório de análise exploratória de dados](./requisitos.md#análise-exploratória-de-dados) | 22/11 | D |
| Estrutura dos repositórios | [Cada equipe deve ter dois repositórios: um para o desenvolvimento do modelo e outro para o desenvolvimento das aplicações](./requisitos.md#estrutura-dos-repositórios) | 18/11 | D |

## Aquisição e pré-processamento dos dados

| Grupo | Requisito | Data de entrega | Conceito | 
|-------|-----------|-----------------|----------|
| Pré-processamento e armazenamento dos dados | [Garantir que os dados estejam disponíveis e acessíveis para a equipe de MLEng](./requisitos.md#pré-processamento-e-armazenamento-dos-dados) | 22/11 | C |
| Pré-processamento e armazenamento dos dados | [Automatizar o pipeline de pré-processamento dos dados](./requisitos.md#pré-processamento-e-armazenamento-dos-dados) | 29/11 | B |
| Pré-processamento e armazenamento dos dados | [Definir um sistema de versionamento dos dados e modelos](./requisitos.md#pré-processamento-e-armazenamento-dos-dados) | 29/11 | A |
| Modelagem | [Automatizar todo o pipeline end-to-end para criação e avaliação de modelos](./requisitos.md#pré-processamento-e-armazenamento-dos-dados) | 03/12 | A |

## Desenvolvimento e avaliação dos modelos

| Grupo | Requisito | Data de entrega | Conceito | 
|-------|-----------|-----------------|----------|
| Modelagem | [Implementação de um pipeline para geração de um modelo baseline](./requisitos.md#modelagem) | 29/11 | C |
| Modelagem | [Implementação da CNN descrita no artigo de referência](./requisitos.md#modelagem) | 06/12 | B |
| Modelagem | [Implementação de um modelo de rede neural com outras características mas que tenham, no mínimo, um desempenho similar ao modelo descrito no artigo de referência.](./requisitos.md#modelagem) | 06/12 | A |

## Apresentação dos resultados

| Grupo | Requisito | Data de entrega | Conceito | 
|-------|-----------|-----------------|----------|
| Apresentação dos resultados | [Identificar as melhores métricas para avaliação dos modelos](./requisitos.md#avaliação-e-apresentação-dos-resultados) | 22/11 | C |
| Apresentação dos resultados | [Definir um pipeline correto para avaliação dos modelos](./requisitos.md#avaliação-e-apresentação-dos-resultados) | 29/11 | C |
| Apresentação dos resultados | [Apresentar os resultados obtidos com os modelos desenvolvidos](./requisitos.md#avaliação-e-apresentação-dos-resultados) | 06/12 | B |
| Apresentação dos resultados | [Apresentar os modelos desenvolvidos e comparar os resultados obtidos com os resultados apresentados no artigo](./requisitos.md#avaliação-e-apresentação-dos-resultados) | 06/12 | A |
| Apresentação dos resultados | [Entregar um relatório técnico em markdown no repositório do projeto](./requisitos.md#avaliação-e-apresentação-dos-resultados) | 06/12 | A |

## Deploy dos sistemas e modelos

| Grupo | Requisito | Data de entrega | Conceito | 
|-------|-----------|-----------------|----------|
| Deploy | [Armazenar as versões dos modelos usando uma ferramenta específica para isto](./requisitos.md#deploy) | 29/11 | C |
| Deploy | [Implementar um site web que demonstra o modelo treinado](./requisitos.md#deploy) | 29/11 | B |
| Deploy | [Implementar uma rotina para análise em lote de imagens](./requisitos.md#deploy) | 29/11 | B |
| Deploy | [Implementar uma infra-estrutura de log para monitoramento do modelo](./requisitos.md#deploy) | 03/12 | B |
| Deploy | [Deploy automático da aplicação ao atualizar o branch main](./requisitos.md#deploy) | 03/12 | A |
| Deploy | [Rotinas de testes automatizados para o site web e para a rotina em lote](./requisitos.md#deploy) | 03/12 | A |

## Organização da equipe

| Grupo | Requisito | Data de entrega | Conceito | 
|-------|-----------|-----------------|----------|
| Gestão de projetos | [Manter um kanban atualizado diariamente](./requisitos.md#gestão-de-projetos) | Diário | {OK, NOK} |
| Organização dos repositórios | [Todos os códigos devem ser salvos em arquivos `.py` e todos os relatórios (incluindo apresentação) devem ser escritos em Markdown](./requisitos.md#entregáveis-e-estrutura-dos-repositórios) | 06/12 | {OK, NOK} |
| Documentação | [Documentação adequada nos repositórios e artefatos do projeto](./requisitos.md#documentação) | 06/12 | {OK, NOK} |
| Compreensão do problema | [Participação no curso da DASA por todos os membros da equipe](./requisitos.md#compreensão-do-problema) | 06/11 | {OK, NOK} |
| Gestão de projetos | [Commits diários e relevantes por parte de todos os integrantes da equipe](./requisitos.md#gestão-de-projetos) | Diário | {OK, NOK} |
| Gestão de projetos | [Commits organizados e claros](./requisitos.md#gestão-de-projetos). Por favor, considerem este [documento](https://bit.ly/insper_commits) de recomendações. | Diário | {OK, NOK} |

## Regras gerais

Se a equipe ficar com conceito D então todos os membros estão automaticamente reprovados. 

Para as equipes que tiverem conceito C ou superior, os itens de organização da equipe serão utilizados para definir o sinal do conceito (positivo, neutro ou negativo). Se todos os itens de organização da equipe estiverem OK então o conceito será positivo. Se algum item estiver NOK então o conceito será neutro. Se dois itens estiverem NOK então o conceito será negativo. Se três ou quatro itens estiverem NOK então a equipe receberá um conceito a menos do que o conceito obtido na rubrica. Se cinco ou seis itens estiverem NOK então a equipe receberá dois conceitos a menos do que o conceito obtido na rubrica.

## Faltas

Se o estudante faltar mais que 4 aulas durante a sprint então o seu conceito será no máximo B. Se o estudante faltar mais que 6 aulas durante a sprint então o seu conceito será no máximo C. Se o estudante faltar mais que 8 aulas então estará automaticamente reprovado. 

Esta regra pode ser resumida pela equação abaixo: 

$$
f(faltas)=
\begin{cases}
Reprovado & \quad \text{if $faltas \geq 9$}\\ 
C & \quad \text{if $faltas \geq 6$}\\
B & \quad \text{if $faltas \geq 4$}\\
\text{Sem limite de conceito} & \quad \text{if $faltas < 4$}
\end{cases}
$$