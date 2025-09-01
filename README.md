![Python](https://img.shields.io/badge/python-v3.7-blue)
![Dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
![Status](https://img.shields.io/badge/status-up-brightgreen)

<h1 align="center">
  <img src="https://github.com/0nurB/BioPredictionRPI-1.0/blob/main/assets/logoBio.png" alt="BioPrediction" width="500">
</h1>

<h4 align="center">Descoberta de redes de interações proteína-proteína em plantas: uma abordagem para inovação no melhoramento genético e estudo da biodiversidade da America do Sul</h4>

<h4 align="center">Explorando a Biodiversidade da América do Sul</h4>

<p align="center">
  <a href="https://github.com/0nurB/Plantas-ppi">Entrada</a> •
  <a href="http://autoaipandemics.icmc.usp.br">AutoAI-Pandemics</a> •
  <a href="#installing-dependencies-and-package">Instalando</a> •
  <a href="#how-to-use">Como usar</a> •
  <a href="#citation">Citações</a> 
</p>

<h1 align="center"></h1>


## Main

**Artigo publicado:** em progesso...


## Abstract

Apesar da elevada capacidade agrícola de países do MERCOSUL, a América Latina figura entre as regiões mais afetadas pela insegurança alimentar, que em 2024 já alcançou mais de 2 bilhões de pessoas no mundo. A intensificação das mudanças climáticas contribui diretamente para esse cenário: fenômenos como o El Niño intensificam secas, enquanto a redução da disponibilidade de água e o aumento das temperaturas comprometem a estabilidade da produção agrícola global. Nesse contexto, torna-se urgente repensar estratégias para garantir a segurança alimentar. Entre as alternativas mais promissoras estão as inovações biotecnológicas, em especial o melhoramento genético, que busca desenvolver cultivos mais resistentes a estresses abióticos e capazes de sustentar a produtividade diante de condições climáticas cada vez mais adversas.
O desenvolvimento de organismos geneticamente modificados depende da identificação de genes associados à resistência a estresses abióticos, processo que passa pela compreensão das interações proteína–proteína (PPIs). Embora técnicas laboratoriais para caracterização de PPIs sejam eficazes, apresentam alto custo e baixa escalabilidade. Métodos in silico baseados em inteligência artificial (IA) têm avançado nesse campo, especialmente aqueles que exploram a estrutura primária das proteínas para prever interações de forma rápida e em larga escala.
Neste estudo, propomos um modelo preditivo baseado em IA voltado para o clado Viridiplantae, englobando espécies agrícolas relevantes da América do Sul. O modelo alcançou 93% de acurácia em dados balanceados de plantas e 85% em eucariotos em geral, superando métodos publicados anteriormente. A principal contribuição está no equilíbrio entre alta especificidade e robuste frente à diversidade estrutural, mesmo em cenários desbalanceados, situação que engloba a procura de interações por amostragem aleatória, onde a fração de positivas estimada é de apenas 1,5 a cada 100 pares aleatórios.
Além da validação em múltiplas espécies, o modelo foi utilizado para minerar 3 milhões de novas interações de muita alta probabilidade, envolvendo mais de 200 mil proteínas que antes não tinham interações nessa categória. Esses resultados sustentam a proposta de criação do Brazilian Repositorium for Protein–Protein Interactions, que reunirá interações de confiança e dados exclusivos da biodiversidade sul-americana. Tal iniciativa visa apoiar pesquisas em biotecnologia vegetal, acelerar a descoberta de alvos para o melhoramento genético e contribuir para a resiliência agrícola frente às mudanças climáticas.

* No melhor do nosso conhecimento é o modelo mais bem validado do estado-da-arte para para predição binária de PPIs;
  -  Inclui validação por conceitos evolutivos e por estrutura de proteína, sendo realizado em espécies de todo o domínio de eucariotos
  -  Propoe métodos de comparação estrutural na validação.
  -  Propoe estimativa da fração de verdadeiros positivos em novas amostras
*  Primeiro modelo a estimar a precisão no mundo real (amostras aleatórias)
* Mineração de 3M de interações de muita alta probabilidade para plantas e algas.

* Esse projeto propoe aspectos práticos de descoberta de PPIs visando melhorar nossos bancos géneticos que suportem melhoramento genetico para enfretar mudanças climáticas. Em breve, o modelo contará com interfaces de uso ou meios de aplicação para não programadores ou especialistas de IA, bem como a versão 2.0 incluindo predições para todos os eucariotos.
* Esse projeto faz parte de um projeto maior o AutoIA-Pandemics que visa desenvolver aplicações de IA que possam auxiliar no estudo de pandemias.


## Maintainers

* Bruno Rafael Florentino

* **Contato:** brunorf1204@usp.br


## Rode no Google Cobab
Em progresso uma versão dos arquivos para rodar pelo Google Colab, online e sem necessidade de instação do python.


## Rode localmente

### Instale a dependencias e pacotes

#### Via miniconda (Terminal)

Baixando os dados e dependencias:

```sh
$ git clone https://github.com/0nurB/BioPredictionPPI.git BioPredictionPPI

$ cd BioPredictionPPI

```

**1 - Install Miniconda:** 

```sh

See documentation: https://docs.conda.io/en/latest/miniconda.html

$ wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh

$ chmod +x Miniconda3-latest-Linux-x86_64.sh

$ ./Miniconda3-latest-Linux-x86_64.sh

$ export PATH=~/miniconda3/bin:$PATH

```

**2 - Create environment:**

```sh

conda env create -f ambiente_base.yml

```

**3 - Activate environment:**

```sh

conda activate ambiente_base

```
## Como usar

Existem dois arquivos tipo jupter notebook para serem utilizados:

- novas_predicoes.ipynb : para dados não rotulados, permite a predição, alinhamento e calculado da precisão média em amostras aleatórias. Exemplo com as proteínas da jabuticabeira.
- performance_testes.ipynb : para dados rotulados, permite mensurar performance em qualquer conjunto de dados, contém um exemplo completo de como utilizar.


## Citation

Em processo de finalização para submissão a revista...
