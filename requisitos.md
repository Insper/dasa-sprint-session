# Requisitos do projeto

Este documento descreve os requisitos funcionais e não funcionais do projeto, além de requisitos de estrutura da equipe. Os requisitos deste projeto estão divididos em algumas categorias: 

## Estrutura da equipe

Todas as equipes serão formadas por 4 estudantes. 

* Todas as equipes devem ser divididas em duas sub-equipes: MLEng e MLOps. Neste projeto vamos usar estas duas definições: 

    * **MLEng**: Equipe de Machine Learning Engineering. Esta equipe será responsável pelo entendimento dos dados e desenvolvimento do modelo de machine learning. Em algumas organizações, esta equipe também é chamada de equipe de *Data Science*.
    * **MLOps**: Equipe de Machine Learning Operations. Esta equipe será responsável por todos procedimentos relacionados a leitura e atualização de dados e modelos. Em algumas organizações, esta equipe também é chamada de equipe de *Data Engineering*.

As entregas de cada equipe são descritas em maiores detalhes logo abaixo.

Todas as entregas devem ser feitas via GitHub. Inclusive relatórios ou questionários. Estes devem ser escritos em [Markdown](https://www.markdownguide.org/). 

## Compreensão do problema

* Todos os membros da equipe precisam participar do curso ministrado pela equipe da DASA. O dia e horário deste curso estão na [agenda do projeto](./agenda.md).

* A equipe precisa entregar um documento respondendo as seguintes perguntas:  
    
    - O que é homologous recombination deficiency (HRD) e por que é importante no tratamento do câncer?
    - O que é GIInger e como ele aborda as limitações dos métodos existentes?
    - O que é genomic instability index (GII) e qual sua relação com HRD?
    - Como foi validado o GIInger e quais foram os resultados?

As respostas para estas perguntas precisam ser feitas depois da leitura do artigo: [Pozzorini, Christian et al. **"GIInger predicts homologous recombination deficiency and patient response to PARPi treatment from shallow genomic profiles."** *Cell reports. Medicine* vol. 4,12 (2023): 101344. doi:10.1016/j.xcrm.2023.101344](./referencias/gIInger_paper.pdf)

## Análise exploratória de dados

* A equipe de MLEng precisa entregar um relatório com a análise exploratória dos dados, respondendo as seguintes perguntas:

    - Qual o tamanho do dataset?
    - Quais são as variáveis disponíveis?
    - Quais os tipos de dados disponíveis?
    - Quais são as variáveis de entrada e saída do modelo?
    - Fazer uma análise descritiva univaria e bivariada das variáveis mostrando os principais achados. 

## Pré-processamento e armazenamento dos dados

A equipe da DASA irá disponibilizar o dataset para treinamento e validação em algum serviço de armazenamento de dados privado.

* A equipe de MLOps precisa garantir que os dados estejam disponíveis e acessíveis para a equipe de MLEng. Todo o processo de cópia do dataset para o ambiente de treinamento deve ser automatizado. A equipe de MLOps deve garantir que os dados estejam disponíveis em um ambiente seguro e privado, e que estejam sempre atualizados para a equipe de MLEng. O script de cópia do dataset deve ser parametrizável considerando os cenários de treinamento e validação do modelo. 

* Todo pipeline de pré-processamento dos dados deve ser automatizado e documentado.

* Assim como o código, os dados também precisam fazer uso de um sistema de versionamento. É de responsabilidade da equipe de MLOps definir o sistema de versionamente. Mas, é de responsabilidade de ambas as equipes, MLOps e MLEng, o correto uso do mesmo.

## Modelagem

A equipe do Insper (MLEng e MLOps) precisam entender como funciona e como implementar uma CNN. 

* A equipe do Insper precisa executar o tutorial abaixo para entender como funciona uma CNN e como implementar uma em Keras:

    * https://www.tensorflow.org/tutorials/images/cnn

O tutorial executado precisa estar no repositório do projeto em uma pasta específica. 

* A equipe do Insper precisa entregar um documento que respondendo as seguintes perguntas:

    - O que é uma CNN?
    - Como funciona uma CNN?
    - Como acontece a extração de características em uma CNN?
    - Quais são as principais camadas de uma CNN?
    - O que as camadas de Convolução, Padding e Pooling fazem?
    - O que é uma camada Dense, Dropout, ReLU e Flatten?

* A equipe de MLEng deve implementar uma CNN qualquer para validar o processo de construção do modelo e obter um modelo *baseline*. 

* O modelo baseline deve ser salvo no repositório de modelos do projeto. A equipe de MLOps deve providenciar um repositório de modelos e ferramentas para versionamento dos modelos. Este respositório deve permitir a recuperação de qualquer modelo e sua respecitva versão em qualquer momento.

* A equipe de MLEng deve implementar a CNN descrita no artigo de referência e comparar os resultados com o modelo baseline. 

* A equipe de MLEng poderá implementar um modelo de rede neural com outras características que não as descritas no artigo de referência e comparar os resultados com o modelo descrito no artigo.

## Avaliação e apresentação dos resultados

* A equipe de MLEng deve ser capaz de identificar quais são as melhores métricas para avaliação dos modelos.

* A equipe de MLEng deve apresentar os resultados obtidos com os modelos desenvolvidos, considerando as métricas escolhidas.

* A equipe do Insper deve ser capaz de ler o artigo referência e entender quais foram as métricas utilizadas no artigo. 

* A equipe do Insper deve ser capaz de apresentar o modelo desenvolvido e comparar os resultados obtidos com o modelo baseline.

* A equipe do Insper deve ser capaz de apresentar o modelo desenvolvido e comparar os resultados obtidos com o modelo descrito no artigo.  

## Deploy do modelo

* Os modelos desenvolvidos pela equipe do Insper devem ser armazenados em algum serviço de armazenamento e devem ter um controle de versão. Este controle de versão deve permitir recuperar qualquer versão do modelo pré-existente. 

* A equipe do Insper deve desenvolver um site web para demonstrar o uso do modelo. Um site onde a partir do upload do um heatmap apresentar a tomada de decisão sobre o mesmo. A equipe do Insper deve se organizar para decidir quem será responsável por este componente. 

* A equipe de MLOps deve criar uma infra-estrutura de *log* para registrar o uso do modelo. Todas as classificações precisam ser armazenadas, o heatmap utilizado e os resultados relacionados com o heatmap, assim como outras informações, tais como, data, hora e versão do modelo utilizada. 

* A equipe do Insper deve desenvolver uma forma de uso do modelo em lote, ou seja, a partir de um arquivo com vários heatmaps, o modelo deve ser capaz de analisar todos os heatmaps e retornar um arquivo com os resultados.

* O mesmo serviço de *log* utilizado para o site web também deve ser utilizado para o uso em lote.

## Entregáveis e estrutura dos repositórios

* Cada equipe deve organizar os entregáveis do projeto em dois repositórios. Este repositório para os dados, scripts e modelos, e um segundo repositório para as aplicações que irão usar o modelo. 

* Os dados utilizados neste projeto não poderão ser armazenados no repositório do GitHub. As ferramentas para armazenamento e controle de versão dos dados deverão ser outras. 

* Todos os relatórios precisam ser escritos em Markdown e armazenados no repositório do projeto, inclusive a apresentação final. 

* Os scripts para pré-processamento dos dados, treinamento dos modelos e avaliação dos modelos precisam estar escritos em Python de preferência. Por favor, tentem utilizar o mínimo possível Jupyter Notebook para estas tarefas. O controle de versão dos scripts em Jupyter Notebook é muito difícil de ser feito. Talvez, o único momento onde será necessário usar Jupyter notebook é no pré-processamento dos dados e na análise exploratório. Mesmo assim, recomenda-se salvar um arquivo `.py` com a versão final.

## Gestão do projeto

* A equipe do Insper deve manter um kanban do projeto atualizado diariamente. A ferramenta de kanban deve ser a do GitHub Projects. 

* Os commits feitos nos repositórios devem ser feitos de forma organizada e com mensagens claras. 

* Os commits devem ser feitos no mínimo uma vez por dia. 