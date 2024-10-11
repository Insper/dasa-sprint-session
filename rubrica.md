# Rubrica

A rubrica deste projeto será dividida em algumas categorias: 

## Compreensão do problema

[ ] Todos os membros da equipe precisam participar do curso ministrado pela equipe da DASA.

[ ] A equipe precisa entregar um documento respondendo as seguintes perguntas:  
    
- O que é homologous recombination deficiency (HRD) e por que é importante no tratamento do câncer?
- O que é GIInger e como ele aborda as limitações dos métodos existentes?
- O que é genomic instability index (GII) e qual sua relação com HRD?
- Como foi validado o GIInger e quais foram os resultados?

As respostas para estas perguntas precisam ser feitas depois da leitura do artigo: Pozzorini, Christian et al. **"GIInger predicts homologous recombination deficiency and patient response to PARPi treatment from shallow genomic profiles."** *Cell reports. Medicine* vol. 4,12 (2023): 101344. doi:10.1016/j.xcrm.2023.101344

## Análise exploratória de dados

[ ] A equipe de MLEng precisa entregar um relatório com a análise exploratória dos dados, respondendo as seguintes perguntas:

- Qual o tamanho do dataset?
- Quais são as variáveis disponíveis?
- Quais os tipos de dados disponíveis?
- Quais são as variáveis de entrada e saída do modelo?
- Qual a distribuição das variáveis?

## Pré-processamento e armazenamento dos dados

A equipe da DASA irá disponibilizar o dataset para treinamento e validação em algum serviço de armazenamento de dados privado.

[ ] A equipe de MLOps precisa garantir que os dados estejam disponíveis e acessíveis para a equipe de MLEng. Todo o processo de cópia do dataset para o ambiente de treinamento deve ser automatizado. A equipe de MLOps deve garantir que os dados estejam disponíveis em um ambiente seguro e privado, e que estejam sempre atualizados para a equipe de MLEng. O script de cópia do dataset deve ser parametrizável considerando os cenários de treinamento e validação do modelo. 

[ ] Todo pipeline de pré-processamento dos dados deve ser automatizado e documentado.

[ ] Assim como o código, os dados também precisam fazer uso de um sistema de versionamento. É de responsabilidade da equipe de MLOps definir o sistema de versionamente. Mas, é de responsabilidade de ambas as equipes, MLOps e MLEng, o correto uso do mesmo.

## Modelagem

A equipe do Insper (MLEng e MLOps) precisam entender como funciona e como implementar uma CNN. 

[ ] A equipe do Insper precisa executar pelo menos um dos dois tutoriais abaixo para entender como funciona uma CNN e como implementar uma em Python.

* https://www.tensorflow.org/tutorials/images/cnn
* https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html

O tutorial que foi executado precisa estar no repositório do projeto em uma pasta específica. 

[ ] A equipe do Insper precisa entregar um documento que respondendo as seguintes perguntas:

- O que é uma CNN?
- Como funciona uma CNN?
- Como acontece a extração de características em uma CNN?
- Quais são as principais camadas de uma CNN?
- O que as camadas de Convolução, Padding e Pooling fazem?
- O que é uma camada Dense, Dropout, ReLU e Flatten?

[ ] A equipe de MLEng deve implementar uma CNN qualquer para validar o processo de construção do modelo e obter um modelo baseline. 

[ ] O modelo baseline deve ser salvo no repositório de modelos do projeto. A equipe de MLOps deve providenciar um repositório de modelos e ferramentas para versionamento dos modelos. Este respositório deve permitir a recuperação de qualquer modelo e sua respecitva versão em qualquer momento.

[ ] A equipe de MLEng deve implementar a CNN descrita no artigo de referência e comparar os resultados com o modelo baseline. 

[ ] A equipe de MLEng deve implementar um modelo de classificação de HRD utilizando uma CNN.


## Avaliação e apresentação dos resultados



## Deploy do modelo

[ ] Os modelos desenvolvidos pela equipe do Insper devem ser armazenados em algum serviço de armazenamento e devem ter um controle de versão. Este controle de versão deve permitir recuperar qualquer versão do modelo pré-existente. 

[ ] A equipe do Insper deve desenvolver um site web para demonstrar o uso do modelo. Um site onde a partir do upload do um heatmap apresentar a tomada de decisão sobre o mesmo. A equipe do Insper deve se organizar para decidir quem será responsável por este componente. 


## Entregáveis e estrutura dos repositórios
