# MBA EXECUTIVO EM BUSINESS ANALYTICS E BIG DATA 

# TRABALHO DE MODELAGEM ESTATÍSTICA AVANÇADA([PDF de Instruções](https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Trabalho%20Modelagem%20Estat%C3%ADstica%20Avan%C3%A7ada.pdf))

**Professor: Paulo Maranhão** 

**Alunos: Americo Freitas, Arleks dos Santos e Luciano Ozorio**

**Prazo: 08/05/2022** 

**Questão 1:** Seguem abaixo cinco bases de dados que se encontram do próprio R onde cada variável resposta encontra-se entre parêntesis. Cada grupo ou cada aluno deve escolher três base de dados. Para cada base de dados deve ser feito uma análise estatística conforme a teoria da disciplina de Modelagem Estatística Avançada. Cada análise deve responder os seguintes itens:

**Bases Selecionadas:** mtcars, quakes e swiss ([Seleção das bases](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/SelecaoBasesDados.html))

**Desenvolvimento dos Ajustes:** [Mtcars](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Mtcars.html), [Swiss](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Swiss.html), [Quakes](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Quakes.html)

> **a)** Usando o R determine o melhor modelo linear possível para a estimar o valor médio de cada variável resposta. Proponha quaisquer transformações que achar necessário para melhorar o ajuste do modelo.
> - **Mtcars:** Aparentemente, o melhor modelo linear possível é: **hp = 53,17 + 0,52disp -28,59wt + 23,58carb**. Não foram necessárias transformações para chegar neste modelo.
> - **Swiss:** O melhor modelo linear possível é: **Fertility = 4.136 -0,002 Agriculture - 0,017 Education + 0,001 Catholic + 0.016 Infant.Mortality**. A transformação realizada, foi a inclusão do log na variável resposta.
> - **Quakes:** O melhor modelo linear possível é: **mag = 5,73 -7,69 lat -9,45 long -2,72 depth + 1,53 stations**. Nenhuma transformação nas variáveis foi aplicada.
> 
> **b)** Os pressupostos dos modelos foram atendidos? Apresente os resultados graficamente e analiticamente (testes formais) comprovando se as suposições foram satisfeitas.
> - **Mtcars:** Todos os pressupostos foram atendidos, as apresentações gráficas estão neste ([link](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Mtcars.html)) 
> - **Swiss:** O teste de Durbin-Watson indica que devemos rejeitar a hipótese de Independência (Não Autocorrelação) dos resíduos, as apresentações gráficas estão neste ([link](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Swiss.html))
> - **Quakes:** Todos os pressupostos foram atendidos, as apresentações gráficas estão neste ([link](http://htmlpreview.github.io/?https://github.com/americofreitasjr/ModelagemEstatisticaAvancada/blob/main/Quakes.html)) 
> 
> **c)** Utilize uma parte dos dados para gerar previsões e intervalos de confiança. É possível dizer que o modelo foi bem ajustado?
> - **Mtcars:** A previsão de hp para os parametros passados com base no modelo, foi 142,5679. E foi establelecido um intervalo de confiançã entre 127,453 e 157,6827.. Pelos resultados apresentados, é possível sim dizer que o modelo foi bem ajustado.
> - **Swiss:** AS previsões e intervalos de confiança não foram gerados, porque mesmo com a transformação nos dados o modelo não ficou bem ajustado, não possibilidando uma previsão Assertiva.
> - **Quakes:** A previsão de mag para os parametros passados com base no modelo, foi 4,231. E foi establelecido um intervalo de confiança entre 4,207 e 4,254. Pelos resultados apresentados, é possível sim dizer que o modelo foi bem ajustado.

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

O melhor modelo linear é: **PROD = 1,64 + 2,91 BALGR + 1,32 REII + 1,99 VALU -2,91 FFD_DVA +2,91 DFD_FVA -3,33 CONS_VA -1,25 EXGR_SERV_FVASH +2,78 IMGRINT_REII -1,74 IMGR_DVASH -7,44 VALU_FFDDVA -2,55 PROD_VASH -5,79 FEXDVAPSH.**

**b)** Quais fatores afetam a variável resposta?

**b)** O modelo é adequado para estimar um valor futuro da variável resposta?

Sim, o modelo gerou uma estimativa para a variável resposta.

**c)** Os pressupostos dos modelos foram atendidos? Apresente os resultados graficamente e analiticamente (testes formais) comprovando se as suposições foram satisfeitas.

Sim.

**d)** Utilize uma parte dos dados para gerar previsões e intervalos de confiança. É possível dizer que o modelo foi bem ajustado?

Como o ajuste não foi passou por todos os pressupostos, significa que o modelo não fará uma previsão
confiável, porém, segue uma simulação de previsão e intervalo de confiança.

* **Obs1:** A análise deve ser feita em forma de relatório e deve ser enviada obrigatoriamente para a pasta “Trabalho de Modelagem Estatística” que se encontra
dentro da aba Entrega de Atividades do E-Class. Quaisquer dúvidas sobre o trabalho podem ser encaminhadas para o e-mail maranhao@ime.eb.br.
* **Obs2:** Um vídeo contendo uma explicação mais detalhada sobre a questão 2 pode ser encontrado no E-Class.
* **Obs3:** A data de entrega do trabalho é 08 de maio de 2022.

