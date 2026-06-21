### Sentiment Analysis on Brazilian App Reviews 🇧🇷 ###

Sentiment classification on real Brazilian Play Store reviews, combining text analysis with star ratings.

*[Leia em português](#análise-de-sentimentos-em-reviews-de-apps-brasileiros-)*

---

### Overview ###

This project applies NLP techniques to real-world app reviews collected directly from the Google Play Store, with a focus on **informal Brazilian Portuguese** — slang, typos, and natural language patterns that most English-centric NLP tutorials don't cover.

### Why this project? ##

Most NLP portfolio projects rely on English datasets. This one tackles real Brazilian Portuguese text, which is technically more challenging and closer to what local companies (fintechs, retail, delivery apps) actually deal with.

### Status ###

In progress

- [ OK ] Data collection (Google Play Scraper)
- [ OK ] Text cleaning and preprocessing
- [ OK ] Sentiment labeling based on star ratings
- [ OK ] Exploratory data analysis
- [ ] Machine Learning classification model
- [ ] Interactive dashboard

### Tech stack ###

- Python
- pandas
- google-play-scraper
- matplotlib / seaborn
- scikit-learn *(next step)*

### How to run ###

```bash
pip install -r requirements.txt
```

Then open the notebooks in `notebooks/` and run them in order.

### Project structure ###

```
├── data/
│   ├── raw/          # raw collected data
│   └── processed/    # cleaned and labeled data
├── notebooks/        # Jupyter notebooks
├── src/              # reusable Python scripts (upcoming)
└── requirements.txt
```

### Methodology notes ###

- Star ratings (1-5) are used as the sentiment label (1-2 = negative, 3 = neutral, 4-5 = positive), since they're a more reliable signal than inferring sentiment from emojis alone.
- Emojis were removed during text cleaning — the verbal content combined with the star rating already provides sufficient signal for sentiment classification.

---

### Análise de Sentimentos em Reviews de Apps Brasileiros 🇧🇷 ###

Classificação de sentimento em reviews reais da Play Store brasileira, combinando análise de texto com a nota em estrelas.

## Visão geral

Este projeto aplica técnicas de NLP em avaliações reais de aplicativos coletadas diretamente da Google Play Store, com foco em **português brasileiro informal** — gírias, erros de digitação e padrões de linguagem que a maioria dos tutoriais de NLP (focados em inglês) não cobre.

### Por que esse projeto? ###

A maioria dos projetos de portfólio em NLP usa datasets em inglês. Este projeto lida com texto real em português brasileiro, o que é tecnicamente mais desafiador e mais próximo do que empresas locais (fintechs, varejo, apps de delivery) realmente enfrentam.

## Status

Em desenvolvimento

- [x] Coleta de dados (Google Play Scraper)
- [x] Limpeza e pré-processamento de texto
- [x] Rotulagem de sentimento via nota
- [x] Análise exploratória
- [ ] Modelo de classificação (Machine Learning)
- [ ] Dashboard interativo

### Tecnologias ###

- Python
- pandas
- google-play-scraper
- matplotlib / seaborn
- scikit-learn *(próxima etapa)*

### Como rodar o projeto ###

```bash
pip install -r requirements.txt
```

Depois abra os notebooks em `notebooks/` e rode em ordem.

## Estrutura do projeto ###

```
├── data/
│   ├── raw/          # dados brutos coletados
│   └── processed/    # dados limpos e rotulados
├── notebooks/        # notebooks Jupyter
├── src/              # scripts Python reutilizáveis (em breve)
└── requirements.txt
```

## Notas de metodologia ###

- A nota em estrelas (1-5) é usada como rótulo de sentimento (1-2 = negativo, 3 = neutro, 4-5 = positivo), por ser um sinal mais confiável do que inferir sentimento apenas a partir de emojis.
- Emojis foram removidos na limpeza de texto — o conteúdo verbal combinado com a nota já fornece sinal suficiente para a classificação de sentimento.