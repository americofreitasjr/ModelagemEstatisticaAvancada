# MBA EXECUTIVO EM BUSINESS ANALYTICS E BIG DATA 

# TRABALHO DE MODELAGEM ESTATÍSTICA AVANÇADA([PDF de Instruções](https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Trabalho%20Modelagem%20Estat%C3%ADstica%20Avan%C3%A7ada.pdf))

**Professor: Paulo Maranhão** 

**Prazo: 08/05/2022** 

**Questão 1:** Seguem abaixo cinco bases de dados que se encontram do próprio R onde cada variável resposta encontra-se entre parêntesis. Cada grupo ou cada aluno deve escolher três base de dados. Para cada base de dados deve ser feito uma análise estatística conforme a teoria da disciplina de Modelagem Estatística Avançada. Cada análise deve responder os seguintes itens:

**Bases Selecionadas:** mtcars, quakes e swiss ([Seleção das bases](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/SelecaoBasesDados.html))

**Desenvolvimento dos Ajustes:** [Mtcars](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Mtcars.html), [Swiss](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Swiss.html), [Quakes](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Quakes.html)

> **a)** Usando o R determine o melhor modelo linear possível para a estimar o valor médio de cada variável resposta. Proponha quaisquer transformações que achar necessário para melhorar o ajuste do modelo.
> - **Mtcars:** Aparentemente, o melhor modelo linear possível é: **0,516disp; -28,592wt; 23,576carb**.  Não foram necessárias transformações para chegar neste modelo.
>
> **b)** Os pressupostos dos modelos foram atendidos? Apresente os resultados graficamente e analiticamente (testes formais) comprovando se as suposições foram satisfeitas.
> - **Mtcars:** Todos os pressupostos foram atendidos, as apresentações gráficas estão neste ([link](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Mtcars.html)) 
>
> **c)** Utilize uma parte dos dados para gerar previsões e intervalos de confiança. É possível dizer que o modelo foi bem ajustado?
> - **Mtcars:** As previsões estão neste ([link](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Mtcars.html)). Pelos resultados apresentados, é possível sim dizer que o modelo foi bem ajustado.

### *Bases de Dados:*
* mtcars (hp)
* LifeCycleSavings (sr)
* quakes (mag)
* swiss (fertility)
* trees (volume)

**Questão 2:** Imagine que uma empresa de determinado país quer fazer um estudo sobre a produção bruta do país. Para isso resolveu utilizar a base de dados da Organização para a Cooperação e Desenvolvimento Econômico (OECD) cujos dados podem ser encontrados no seguinte sítio:

**([Ajuste do Modelo](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Canada.html)).**

https://stats.oecd.org/Index.aspx?DataSetCode=IO_GHG_2021#

A empresa decidiu utilizar os dados encontrados na popular queries, especificamente
os dados contidos nas planilhas disponíveis na **Trade in Value Added (TiVA) 2021 ed:
Principal Indicators.**

Dessa forma, foi solicitado ao grupo de estudos do **MBA Executivo em Business Analytics e Big Data da FGV** um relatório sobre os dados constantes na base de dados, onde a **variável resposta** a ser estudada é a variável **Produção Bruta**. Dessa forma, cada grupo ou cada aluno (trabalho individual) deve escolher uma país ou um
grupo de países (ex: União Europeia, G20, países não membros da OECD, etc) e responder as seguintes questões:

**a)** Usando o R determine o melhor modelo linear possível para a estimar o valor médio da variável resposta. Proponha quaisquer transformações que achar necessário para melhorar o ajuste do modelo.

**b)** Quais fatores afetam a variável resposta?

**b)** O modelo é adequado para estimar um valor futuro da variável resposta?

**c)** Os pressupostos dos modelos foram atendidos? Apresente os resultados graficamente e analiticamente (testes formais) comprovando se as suposições foram satisfeitas.

**d)** Utilize uma parte dos dados para gerar previsões e intervalos de confiança. É possível dizer que o modelo foi bem ajustado?

* **Obs1:** A análise deve ser feita em forma de relatório e deve ser enviada obrigatoriamente para a pasta “Trabalho de Modelagem Estatística” que se encontra
dentro da aba Entrega de Atividades do E-Class. Quaisquer dúvidas sobre o trabalho podem ser encaminhadas para o e-mail maranhao@ime.eb.br.
* **Obs2:** Um vídeo contendo uma explicação mais detalhada sobre a questão 2 pode ser encontrado no E-Class.
* **Obs3:** A data de entrega do trabalho é 08 de maio de 2022.

