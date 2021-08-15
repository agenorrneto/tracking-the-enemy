# Tracking the enemy: analyzing the SARS-CoV-2 genomic sequencing scenario in Brazil from GISAID data

Nucleic acids are biomolecules very important for life because they are involved in the process of how and when biological information (e.g. our eyes color) is stored, expressed, and transmited to the next generations.
Since the scientific community discovered these molecules (also called DNA and RNA, which are abbreviations people possibly hear sometime in their life) are so critical for living forms on the Earth, much attention has been turned to them. Even virus (like the SARS-CoV-2, the virus that is causing the pandemic we are living) has its own nucleic acid. Thus, knowing the sequence (because nucleic acids are composed of nucleotides sequences, known as nucleotides, like build blocks) is valuable to know at least in part this enemy. The whole DNA or RNA sequence of an organism is called genome and the field that study it and do a lot of other things whith these big sequences is named Genomics.
Many countries, since the pandemic started have done strong efforts to sequence the SARS-CoV-2 genome. For instance (and this is indeed the best example), United Kingdom has sequenced more than 600,000 SARS-CoV-2 genomes[1]. Knowing the enemy that is making a government's country impose three lockdowns, causing more than 120,000 deaths and impacting strongly the economy [2] is essential.

## Objectives
That said, I aim to analyse Brazil genomic sequencing of SARS-CoV-2 scenario and hence:
- how this process is happening in a country of continetal dimensions
- the differences between the years 2020 and 2021
- examples of how this has helped the health authorites to design public policies in the pandemic's context
- the importance of metadata when talking about "genomic surveillance"

## Methods
Great part of data used in this work was extracted from GISAID (LINK HERE), plese explaind about this database. But genomic sequences (which has not been analyzed here) and metadata (which has been) are provided by a wide range of laboratories throughout Brazil. Besides, numbers of cases were xtracted from... The analysis - data cleaning, data handling, and plot building - was perfomed in Google Collab, using the Pyhton language.

## Results
### Top 10 municipalities: an example to follow
Half of the 10 municipalities that have the greatest number of genomes sequenced (Figure 1) are also among the most populated municipalities in Brazil (Rio de Janeiro, Manaus, São Paulo, Fortaleza and Belo Horizonte). Manaus is the capital of Amazonas state. The city has been hard hit by the pandemic, with a first peak of hospitalizations in late April, 2020 and a strong ressurgance in the beggining of 2021 [3], driven by the variant of concern (VOC) P.1. Genomic sequencing helped to understand how this may happened [4] . Aparecida de Goiânia is the second most populated municipality in the state of Goiás, center west region of Brazil. The city has its own strategy of genomic surveillance (when genomics is used to watch very closely the pathogen, because remember we are sequencing its nucleotides, and this information is used with other epidemiological data to support public health authorites' decisions). See [5] for another example of local initiative.

! [./tracking-the-enemy/municipalities_purple.jpg] (./tracking-the-enemy/municipalities_purple.jpg)

### 2020 vs 2021
Figure 2 presents the percentage of sequenced submitted to GISAID in 2020 and 2021 in relation to the total number of sequences (28,00... as of 13th, August). It is evident that Brazil has submitted more sequences in eight months of the current year than in the first year of the pandemic. One reason to this was the P.1 surgance. Also, scientists stress the mass reciept of laboratory raw materials needed for experiments.

### State level
Brazil has 26 states and one federal district. Five states have more than one thousand sequences deposited. Seventeen have a number of genomes sequenced between 100 and 999 sequences. Besides, five states have less than hundred sequences. I also calculated the cumulative number of genomes sequenced by positive cases. Basically, this number tells how many genomes are generated from all the positives cases. None of the states has more tha 1%. As a matter of comparison, the state of Wyoming has a value of 19%. Thta means sequencing one out of every five positive COVID-19 cases.


### Variants
Mutations are changes that can happen on the genetic material (DNA or RNA). Sometimes they do not have any impact in the charactericts we can see. Otherwise, they can also be the basis of diseases or the increased ability of SARS-CoV-2 to infect more people. Since any biological process can involve many factors and we are still learning about the cycle this virus perform in our cells, the needed iformation here is that this process of mutation has been ocurring in the pandemic and some variants harbor mutations that have the ability to spread more quickly, for instance. P.1 or Gamma variant originated in Manaus. Only the fact the number of sequences of this variant in the samples increased so rapidaly (Figure 4A) called the attention of scientist and then they could turn their attention to investigate this specifically with other data related to the sequences (one more point for genomic surveillance).

However these variants can aquire more mutations and turn in more worying versions of SARS-CoV-2. Figure 4B shows the rising of a sublineage called P.1.7. In March, 2021 (months after P.1 surging), P.1.7 - which actually harbor P.1 muations + one new mutation important for transmission - showed a remarkable represatation in samples.

### Why metadata matters?
Metadata, as location, host and lineage are crucial for genomic surveillance. Clinical data is other example.
For instance, from all the brazillian sequences eleven are from dogs and 3 from cats. Of course, the study of how SARS-CoV-2 can infect non-human mammals and which of them is more than sequencing, but these informations are valuable to strat something else.  

## References

[1] https://www.gov.uk/government/news/uk-exceeds-600000-covid-19-tests-genomically-sequenced

[2] https://en.wikipedia.org/wiki/COVID-19_pandemic_in_the_United_Kingdom

[3] https://www.thelancet.com/article/S0140-6736(21)00183-5/fulltext

[4] https://www.nature.com/articles/s41591-021-01378-7

[5] https://www.ufpe.br/agencia/noticias/-/asset_publisher/dlhi8nsrz4hK/content/primeiro-relatorio-da-ufpe-sobre-sequenciamento-do-sars-cov-2-em-caruaru-constata-predominancia-da-variante-p-1/40615

