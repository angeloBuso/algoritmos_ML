<img alt="header title" scale = "50%" width="100%" src="https://github.com/angeloBuso/angeloBuso/blob/main/image/Imagem2.jpg?raw=true">

<img alt = "qr-code" align = "right" width="10%" src="https://github.com/angeloBuso/angeloBuso/blob/main/image/angelobuso.png?raw=true">

<h1>Ciências de dados e os métodos científicos</h1>

Os **métodos científicos** exige que qualquer pessoa seja capaz de replicar os mesmos resultados, considerando as mesmas premissas.

**Ciência** é um metamorfose do **senso comum**, ambos buscam de alguma forma gerar conhecimento útil para soluções de problemas da humanidade.

A diferença é que, para o método científico há um **rigor** para se obter uma conclusão. *"Rigor"* significa  *exatidão extremada*, *rigidez*, sendo assim, a **ciência** nada mais é que uma especialização do **senso comum** com um controle disciplinado de seu uso.

Apenas o que é **problemático** é pensado. Um problema advém de uma desordem, uma inquietude, um desconforto. Neste enredo, o desconforto é a manisfestação do problema, através de uma referência anterior da ordem. Pois, para saber o que é desordem, *a priori* tem-se a noção da ordem!!!

Então o cientista de dados tem que ter a capacidade de reconhecer a desordem, ajudar ou formular o problema de forma clara e conhecer a ordem para estabelecer uma solução!!

Para tal missão, usamos **modelos** que é uma construção mental da ordem. Modelo é um artefato que tem forte relação com a **teoria** (conexão entre o fenômeno). Sendo assim exige revistar **todo conhecimento** existente sobre o assunto problemático. As **hipóteses** são lançadas com o objetivo de conduzir os esforços para reestabelcer a ordem, são as perguntas propostas, as tentativas de explicar o fenômeno pesquisado. **Modelagem** e **Simulação** computacional é a emulação da realidade, mas modelado por computadores, em que serão exercitados experimentos para (i) avaliação e (ii) melhoria/otimização de seu desempenho - modelo em questão, é a realidade em um ambiente controlado.

De forma resumida acima, compreendemos que os métodos científicos, aplicado em **Ciência de dados**, visa adotar tais métodos na infinidade dos **dados** em que somos expostos, como objetivo de transformar esses últimos em **conhecimento!!**

---
<h1>Projetos de Data Science</h1>

Checklist para aplicar aos projetos de *Data Science*. Baseado nos *frameworks* CRISP-DM, nesta técnica, os dados sugerem qual modelo usar, ou seja, o modelo se ajusta aos dados.

    Problema -> Dados-> Análise Exploratória-> Modelo-> Conclusão
    

Não trata-se é um *checklist* rígido ou imutável. É um norte para conduzir nos projetos de Ciência de Dados.

## 1. Compreensão do Problema de Negócio

* Visão holística e delimitação do escopo do projeto
* Quais serão os usos da solução
* Existência de algo similar
* Métricas de performance e o mínimo esperado para o escopo do projeto
* Premissas básicas do projeto e conhecimento das Regras de Negócios!!

## 2. Coleta e Exploração dos Dados

* Coleta de dados, observar:
    * Extenções dos arquivos
    * Timeframe dos dados
    * Acessos aos bancos de dados consultados
* Quanto a Exploração:
    * Comprender cada atributo/coluna e suas características:
    * Representatividade
    * Tipo (Categórica; Numérica; Estruturada; Não Estruturada)
    * Valores ausentes/missing
    * Estatística descritiva dos atributos/coluna
    * Distribuição dos dados (Gaussiana; Uniforme; Logarítmica)
    * Correlações entre os dados (PS. Correlação NÃO tem efeito de causalidade)
* Identificar a variável alvo (target)
* Visualizar graficamente os dados
* Identificar possíveis transformações
* Identificar os dados extras que podem ser úteis

## 3. Preparar os Dados

* Algoritmos de Machine Learning, esperam receber os dados em formatos específicos
* Modularizar as funções de transformações


1. Transformação de atributos
    * Aterações das variáveis já existentes (renomear, alterar índices, exluir atributo sem relevância)
    * Preencher os valores ausentes/missing
    * Alterar tipos de dados para representação mais fidedigna
2. *Feature Scaling*
    * Normalizar ou padronizar *features*

3. *Feature Engineering*
    * Discretizar variáveis contínuas
    * Decompor *features* (categóricas, data, tempo)
    * Aplicar transformações às variáveis
    * Agregar *features* para gerar novas
    * Usar *Dummies*
    
4. *Feature Selection*
    * Redução de dimensionalidade dos dados
    
5. Divisão dados:
    * Treino
    * Teste
    * Validação
    
## 4. Construção do Modelo

* Automatizar o maior número de passos possíveis
* Boa prática: utilizar mais de um modelo e comparar as performances
* Uso de técnicas de validação cruzada (*cross-validation*)
* Identificar os melhores estimadores
* Métodos *Ensemble* vs modelos *individuais*
* *Tuning do modelo* ajustes dos *hyperparametros*
* Testar o desempenho do mesmo com o dados de **teste**.

## 5. Apresentação da Solução e Deploy

* Documentar todos as etapas
* Lembre-se: o modelo preditivo **espera** receber os novos dados com (i) as mesmas estruturas passadas no treinamento e (ii) os mesmos pré-processamento realizado
* Tornar todos os passos replicáveis (método científico)
* Storytelling - decisores desconhecem a parte técnica
* Ver qual o melhor gráfico para contar cada *insight* descoberto
* Escrever testes unitários -> cada vez mais o produto final da ciêcnia de dados deve ser **escalável para implementar** em produção.
* Criar rotinas de monitoramento e alertas
* Determinar quando atualizar o modelo
