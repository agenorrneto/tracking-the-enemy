# Tracking the enemy: analyzing the SARS-CoV-2 genomic sequencing scenario in Brazil from GISAID data

Nucleic acids are biomolecules very important for life because they are involved in the process of how and when biological information (e.g. our eyes color) is stored, expressed, and transmitted to the next generations.
Since the scientific community discovered these molecules (also called **DNA** and **RNA**, which are abbreviations people possibly hear sometime in their life) are so critical for living forms on the Earth, much attention has been turned to them. Even viruses (like SARS-CoV-2, the virus that is causing the pandemic we are living in) has its own nucleic acid. Thus, knowing the sequence (because nucleic acids are composed of nucleotides sequences, A, G, C, T, U, like build blocks) is valuable to know at least in part this enemy. The whole DNA or RNA sequence of an organism is called genome and the field that study it and do a lot of other handling with these big sequences is named **Genomics**.
Many countries, since the pandemic started, have done strong efforts to sequence the SARS-CoV-2 genome. For instance (and this is indeed an excellent example), the United Kingdom has sequenced more than 600,000 SARS-CoV-2 genomes[1]. Knowing the enemy that is making a government's country impose three lockdowns, causing more than 120,000 deaths and impacting strongly the economy [2] is essential. Brazil has been heavily affected by the pandemic and this in part was due to variants (which can be identified through genomics).

## Objectives
That said, I aim to analyse Brazil genomic sequencing of SARS-CoV-2 scenario and hence:
- how this process is happening in a country of continental dimensions
- the differences between the 2020 and 2021
- examples of how this has helped the health authorities to design public policies in the pandemic's context
- the importance of metadata when talking about "genomic surveillance"

## Methods
Great part of data used in this work was extracted from [GISAID](https://www.gisaid.org), the main database for SARS-CoV-2 genome sequence sharing. But genomic sequences (which has not been analyzed here) and metadata (which has been) are provided by a wide range of laboratories throughout Brazil. Besides, numbers of cases were retrieved from numbers notified by state health secretaries. The analysis - data cleaning, data handling, and plot building - was perfomed in Google Collab, using the Pyhton language. It is important to note that: (a) the numbers presented here are going to change considering that new sequences will be submitted by scientists in Brazil (this is really good) and (b) the graphs that use "year/month" may have low numbers for the nearest months, beacuse sequences are still being submitted and, also it is hard to do "real-time sequencing", that is, there is some delay (this is not a goood news).

## Results
### Top 10 municipalities
Half of the 10 municipalities that have the greatest number of genomes sequenced (Rio de Janeiro, Manaus, São Paulo, Fortaleza and Belo Horizonte) (Figure 1) are also among the most populated municipalities in Brazil. Manaus is the capital of Amazonas state. The city has been hard hit by the pandemic, with a first peak of hospitalizations in late April, 2020 and a strong resurgance in the begining of 2021 [3], driven by the variant of concern (VOC) P.1. Genomic sequencing helped to understand how this may have happened [4]. Aparecida de Goiânia is the second most populated municipality in the state of Goiás, in the center west region of Brazil. The city has its own strategy of genomic surveillance (when genomics is used to watch the pathogen very closely, because remember we are sequencing its nucleotides, and this information is used with other epidemiological data to support public health authorities' decisions). See [5] for another example of local initiative.


**Figure 1**
![Figure 1](municipalities_purple_of.jpg)



Figure 2 shows the contribution of these municipalities to the whole set of sequences (only genomes where the municipality is known), which corresponds to almost one third of the sequences.


**Figure 2**

![Figure 2](municipalitiescontribution.jpg)


### 2020 vs 2021
Figure 3 presents the percentage of sequences submitted to GISAID in 2020 and 2021 in relation to the total number of sequences (28,00... as of 13th, August). It is evident that Brazil has submitted more sequences in eight months of the current year than in the first year of the pandemic. One reason to this was the P.1 surgance. Besides, scientists stress the mass receipt of laboratory raw materials needed for experiments [6].

**Figure 3**
![Figure 3](20vs21.jpg)


### State level
Brazil has 26 states and one federal district. Five states have more than one thousand sequences deposited. Seventeen have a number of genomes sequenced between 100 and 999 sequences. Besides, five states have less than a hundred sequences. I also calculated the cumulative number of cases sequenced (CCS). Basically, this number tells how many genomes are generated from all the positive cases. None of the states achieve more than 1% in this measurement. As a matter of comparison, the state of Wyoming, USA has a value of 19.70%. That means sequencing one out of every five positive COVID-19 cases [7]. The states of Amazonas e Rio de Janeiro (bold) show the two highest values, while PiauÍ (italic) has the lowest one.

|    | STATE               |   Genomes sequenced |   Cumulative nº of cases(08/14/2021) |   Cumulative Cases Sequenced (%) |
|---:|:--------------------|--------------------:|-------------------------------------:|-----------------------------:|
|  0 | SAO PAULO (SP)          |               10857 |                              4164587 |                    0.260698  |
|  1 | **RIO DE JANEIRO (SP)**      |                4997 |                              1080746 |                    0.462366  |
|  2 | **AMAZONAS (AM)**            |                1714 |                               421434 |                    0.406707  |
|  3 | GOIAS (GO)               |                1603 |                               777171 |                    0.206261  |
|  4 | RIO GRANDE DO SUL   |                1530 |                              1390173 |                    0.110058  |
|  5 | PARANA              |                 964 |                              1408273 |                    0.0684526 |
|  6 | PERNAMBUCO          |                 831 |                               600002 |                    0.1385    |
|  7 | BAHIA               |                 751 |                              1208878 |                    0.0621237 |
|  8 | PARA                |                 749 |                              1133146 |                    0.0660992 |
|  9 | SANTA CATARINA      |                 629 |                              2019435 |                    0.0311473 |
| 10 | MINAS GERAIS        |                 561 |                               926017 |                    0.060582  |
| 11 | CEARA               |                 549 |                               577872 |                    0.0950037 |
| 12 | ALAGOAS             |                 369 |                               232635 |                    0.158618  |
| 13 | MARANHAO            |                 339 |                               276821 |                    0.122462  |
| 14 | SERGIPE             |                 327 |                               343001 |                    0.095335  |
| 15 | PARAIBA             |                 297 |                               427511 |                    0.0694719 |
| 16 | ESPIRITO SANTO      |                 257 |                               550920 |                    0.0466492 |
| 17 | RIO GRANDE DO NORTE |                 247 |                               362246 |                    0.0681857 |
| 18 | AMAPA               |                 238 |                               122012 |                    0.195063  |
| 19 | MATO GROSSO DO SUL  |                 142 |                               362732 |                    0.0391474 |
| 20 | ACRE                |                 134 |                                87487 |                    0.153166  |
| 21 | TOCANTINS           |                 129 |                               214482 |                    0.0601449 |
| 22 | MATO GROSSO         |                  93 |                               505031 |                    0.0184147 |
| 23 | RORAIMA             |                  50 |                               459095 |                    0.010891  |
| 24 | DISTRITO FEDERAL    |                  42 |                               121908 |                    0.0344522 |
| 25 | RONDONIA            |                  34 |                               260723 |                    0.0130407 |
| 26 | *PIAUI*               |                  19 |                               313345 |                    0.0060636 |


A choropleth map is shown below (Figure 4) with the same information presented in the two first columns of the previous table.


**Figure 4**

![Figure 4](map_of.png)


### Variants
Mutations are changes that can happen on the genetic material (DNA or RNA). Sometimes they do not have any impact on the characteristics we can see. Otherwise, they can also be the basis of diseases or the increased ability of SARS-CoV-2 to infect more people. Since any biological process can involve many factors and we are still learning about the cycle this virus performs in our cells, the needed information here is that this process of mutation has been occurring in the pandemic and some variants harbor mutations that have the ability to spread more quickly, for instance. The P.1 or Gamma variant originated in Manaus. Only the fact the number of sequences of this variant in the samples increased so rapidly (Figure 5) called the attention of scientist and then they could turn their attention to investigate this specifically with other data related to the sequences (one more point for genomic surveillance).

![Figure 5](p1overtime.jpg)

However these variants can acquire more mutations and turn into more worrying versions of SARS-CoV-2 [8]. Figure 6 shows the rising of a sublineage called P.1.7. 
In March, 2021 (months after P.1 surging), P.1.7 - which actually harbors P.1 mutations + one new mutation important for transmission - showed a remarkable represatation in samples.

![Figure 6](p17overtime.png)

### Why metadata matters?
Metadata, as location, host and lineage are crucial for genomic surveillance. Clinical data is other example.
For instance, from all the brazillian sequences eleven are from dogs and 3 from cats. Of course, the study of how SARS-CoV-2 can infect non-human mammals and which of them is more than sequencing, but these informations are valuable to strat something else.  

## Conclusion
Despite the low number of sequences submitted to GISAID in 2020, Brazil is increasing its efforts to improve this scenario: recently, Fiocruz (Fundação Oswaldo Cruz) committed to deliver 36000 sequences in one year [9]. It is important to fix **disproportionately between states**, **invest and train personnel for data analysis and interpretation**, and **make the use of genomic data common in public health policies design**.

## References

[1] UK exceeds 600,000 COVID-19 tests genomically sequenced - https://www.gov.uk/government/news/uk-exceeds-600000-covid-19-tests-genomically-sequenced

[2] https://en.wikipedia.org/wiki/COVID-19_pandemic_in_the_United_Kingdom

[3] https://www.thelancet.com/article/S0140-6736(21)00183-5/fulltext

[4] https://www.nature.com/articles/s41591-021-01378-7

[5] https://www.ufpe.br/agencia/noticias/-/asset_publisher/dlhi8nsrz4hK/content/primeiro-relatorio-da-ufpe-sobre-sequenciamento-do-sars-cov-2-em-caruaru-constata-predominancia-da-variante-p-1/40615

[6] https://www.uol.com.br/vivabem/noticias/redacao/2021/06/06/e-preciso-estudar-mais-o-genoma-do-sars-cov-2-para-entender-suas-mutacoes.htm

[7] Wyoming Leading The Nation In Sequencing COVID-19 Virus Variants - https://www.wyomingpublicmedia.org/health/2021-08-06/wyoming-leading-the-nation-in-sequencing-covid-19-virus-variants

[8] Emergence and spread of SARS-CoV-2 P.1 (Gamma) lineage variants carrying Spike mutations 𝚫141-144, N679K or P681H during persistent viral circulation in Amazonas, Brazil. - https://virological.org/t/emergence-and-spread-of-sars-cov-2-p-1-gamma-lineage-variants-carrying-spike-mutations-141-144-n679k-or-p681h-during-persistent-viral-circulation-in-amazonas-brazil/722

[9] 'Gestores têm que rever planos porque Delta está em vários estados', diz Fiocruz - https://www.cnnbrasil.com.br/saude/2021/08/10/gestores-tem-que-rever-planos-porque-delta-esta-em-varios-estados-diz-fiocruz
