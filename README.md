# Modelos_de_Linguagem_e_Generativos
rogerio.oliveira@mackenzie.br

<br>

### **Link dos Encontros Síncronos**

> * [09 Março](https://teams.microsoft.com/l/meetup-join/19%3ameeting_OTlmMTY5YTEtMDgxYS00NDhjLWIxMDktM2ZlOTQ1ZmI0Yjkw%40thread.v2/0?context=%7b%22Tid%22%3a%2251da9440-4e5e-47b3-8e5c-4817f6f43c04%22%2c%22Oid%22%3a%22e7fc012e-6f57-4879-9416-93179af90e74%22%7d) | [23 Março](https://teams.microsoft.com/l/meetup-join/19%3ameeting_OTlmMTY5YTEtMDgxYS00NDhjLWIxMDktM2ZlOTQ1ZmI0Yjkw%40thread.v2/0?context=%7b%22Tid%22%3a%2251da9440-4e5e-47b3-8e5c-4817f6f43c04%22%2c%22Oid%22%3a%22e7fc012e-6f57-4879-9416-93179af90e74%22%7d) | [30 Março](https://teams.microsoft.com/l/meetup-join/19%3ameeting_OTlmMTY5YTEtMDgxYS00NDhjLWIxMDktM2ZlOTQ1ZmI0Yjkw%40thread.v2/0?context=%7b%22Tid%22%3a%2251da9440-4e5e-47b3-8e5c-4817f6f43c04%22%2c%22Oid%22%3a%22e7fc012e-6f57-4879-9416-93179af90e74%22%7d)

<br>

### Exercícios (20%)

* Ex1. `scikit-ML-<seu nome>.ipynb`, Implemente um modelo de Aprendizado Supervisionado com o scikit-learn
* Ex2. `scikit-MLP-<seu nome>.ipynb`, Implemente o modelo anterior com um MLP do scikit-learn. Varie diferentes parâmetros do MLP e compare os resultados.
* Ex3. `NLP-<seu nome>.ipynb`, Encontre uma base de dados em português para treinar um modelo Supervisionado para análise de sentimento. Depois de treinado o modelo gere com algum LLM um conjunto de 100 frases (50 positivas e 50 negativas). Empregue o seu modelo para classificar as 100 frases. Compare e discuta os resultados do seu modelo com o *ground-true* (a classificação dada pelo LLM).
* Ex4. `DeepLearning-<seu nome>.ipynb`, Empregue os dados do exercício anterior. No lugar do TF-IDF, empregue agora o embedding de algum modelo LLM e treine um classificador com TensorFlow ou PyTorch. Empregue o seu modelo para classificar as 100 frases do exercício anterior. Compare e discuta os novos resultados com o *ground-true* (a classificação dada pelo LLM).
* Ex5. `ImgTransfer-<seu nome>.ipynb`, Empregue um dos modelos pré-treinados de imagens TensorFlow (https://www.tensorflow.org/api_docs/python/tf/keras/applications?hl=en), exceto os modelos VGG+ e ResNet+ já vistos em sala, para **classificação binária** de imagens de sua escolha. 
  
Link para entrega dos exercícios [aqui](https://drive.google.com/drive/folders/15IQW5jpljaU1W_Ol0G1sU67gFKJF6a8E?usp=drive_link). 

<br>

### **Projeto: Simulação de Opinião Pública (*Silicon Sampling*) (80%)**

Com base em uma pesquisa de opinião do [Cesop](https://www.cesop.unicamp.br/) (Centro de Estudos de Opinião Pública) desenvolver um modelo LLM e um modelo de aprendizado supervisionado para simulação das respostas dos questionários e comparar seus resultados. [Escolha aqui a pesquisa de opinião](https://drive.google.com/drive/folders/10Zv1waT-aTPFsYhZ6l1CSa3feDEBZ1R2?usp=sharing).

1. **Organização e datas**. Trabalho em grupo. Sugestão de 2-3 grupos. Entrega e apresentação do projeto no final do curso, com data a definir. Cada grupo deve escolher uma pesquisa de opinião diferente para o trabalho.

- `Democracia` = Lucas Nascimento, Matheus Moreira
- `Desigualdade` = Maria José, Ana Ribeiro
- `Racismo` = Lucas Braga, Thiago Keller, Renato Rosa

#### Sugestão de Cronograma

| Até | Atividade |
|-|-|
| 14-Mar | Escolha do Grupo, a Pesquisa, Entendimento do Projeto (leitura do artigo) e dados |
| 21-Mar | Geração de respostas simuladas via o modelo de Aprendizado de Máquina Supervisionado |
| 28-Mar | Geração de respostas simuladas via LLM |
| 04-Abr | Comparativo dos resultados dos modelos |
| 11-Abr | Elaboração do artigo (texto do trabalho) e organização do repositório |
| 15-Abr | Ajustes e entrega final |

#### Sugestão de Roteiro de Apresentação (máx 15min)

| Slide | Conteúdo |
|-|-|
| 1 | Apresentação do Questionário empregado |
| 2 | Seleção dos dados para os modelos e Preparação dos Dados (alternativamente em um slide separado) |
| 3 | Modelo Supervisionado (modelo empregado, seus hiperparâmetros, conjuntos de treinamento e teste) |
| 4 | Métricas e resultados do modelo Supervisionado |
| 5 | Modelo LLM empregado (características e justificativa da escolha) |
| 6 | Geração e execução dos prompts (+exemplos dos prompts gerados) |
| 7 | Métricas e resultados do modelo LLM |
| 8 | Comparação dos modelos |
| 9 | Conclusão |

2. **Requisitos mínimos**. Ter como ponto de partida o artigo *Simulating Public Opinion: Comparing Distributional and Individual-Level Predictions from LLMs and Random Forests*, disponível na [pasta](https://drive.google.com/drive/folders/10Zv1waT-aTPFsYhZ6l1CSa3feDEBZ1R2?usp=sharing). Empregar no mínimo 200 simulações Comparar acuracidade (verificar métricas), distribuições das respostas e explicabilidade (importância relativa das variáveis preditoras). Simular ao menos 200 respondentes (10% dos dados), incluindo o maior número possível de características e respostas (sugestão: começe com um pequeno número respondentes, características e respostas, e aumente gradualmente).     
3. **Ferramentas**. Empregue somente modelos e recursos abertos, sendo 100% executável e aberto. Preferencialmente executar 100% em um notebook Colab. 
4. **GitHub**. Implementar um GitHub com o projeto.
5. **Entrega**. No formato de um artigo SBC, preferencialmente em Latex. Apresentação opcional no YouTube (máximo 5min) com o link a ser incluído no GitHub.
6. **Rubrica**. Modelo LLM, 3p (quantidade de atributos e respostas, qualidade dos prompts e aderência das respostas); Modelo Supervisionado, 2p (separação de dados, parametrização do modelo); Análise e Comparação dos resultados, 3p (métricas empregadas, repetições e/ou bootstrapping, gráficos comparativos, técnicas de explicabilidade); Artigo e Aspecto Geral do Trabalho, 2p (Apresentação, fundamentação, referências, apresentação dos resultados).
7. **Vídeo**. Máximo 10min, YouTube e link no GitHub.

**Extra**: Esse projeto pode ser estendido adicionando-se a comparação com a simulação de respostas a partir do *fine-tunning* do modelo. Este trabalho entretanto, já daria uma dissertação. 

<br>

## Aula 1 Introdução

* [Questionário pré-curso](https://forms.gle/LkD3H8LBB6GpvZLv7)
* [Plano de Ensino](https://github.com/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Plano_de_Ensino_Modelos_de_Linguagem_e_Generativos_20250416.pdf)
* [Introdução](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/MLG_01_Introducao.ipynb)

> * Leitura complementar (Cap 1): Alammar, Jay, and Maarten Grootendorst. [Hands-on large language models: language understanding and generation.](https://github.com/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Hands-On-LLM/Jay%20Alammar%2C%20Maarten%20Grootendorst%20-%20Hands-On%20Large%20Language%20Models_%20Language%20Understanding%20and%20Generation%20(2024%2C%20O%E2%80%99Reilly%20Media)%20-%20libgen.pdf) O'Reilly Media, Inc., 2024.
<br>

> *Programa; Visão geral do curso; Introdução ao processamento de linguagem natural; representações vetorais BOW, TF-IDF; similaridade cosseno; outras representações vetorais; tarefas de modelos de linguagem; importância dos termos no aprendizado de máquina.*

## Aula 2 Aprendizado de Máquina Supervisionado

* [Aprendizado de Máquina Supervisionado](https://github.com/Rogerio-mack/Machine-Learning-I) *Cap. 1, 4, 5*
> * 1. [Introdução ao Aprendizado de Máquina](https://colab.research.google.com/github/Rogerio-mack/Machine-Learning-I/blob/main/ML1_introducao.ipynb)
> * 4. [Classificação: Knn](https://colab.research.google.com/github/Rogerio-mack/Machine-Learning-I/blob/main/ML4_Knn.ipynb)
> * 5. [Árvores de Decisão e Seleção de Atributos](https://colab.research.google.com/github/Rogerio-mack/Machine-Learning-I/blob/main/ML5_DecisionTrees.ipynb)

<br>

> *Aprendizado de Máquina (Supervisionado): Cap1. Classificação e Regressão; Cap4. Knn; Cap. Árvores de Decisão; Fronteira de Decisão; Sobreajuste.*

## Aula 3 Métricas de Classificação, Conjuntos de Treinamento e Teste, Neurônio Perceptron

* [Entenda como empregar os estimadores de regressão e classificação do scikit-learn](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/IA_scikit_learn_estimadores.ipynb)
* [Aprendizado Supervisionado: Breast Câncer](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/scikit_learn_breast_cancer.ipynb)
* [Classificação e Métricas](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Overfitting_Treinamento_e_Teste.ipynb)

* [Deep Learning I: Modelos Sequenciais e Autoencoders](https://github.com/Rogerio-mack/Deep-Learning-I)
> * 1. [Introdução aos Modelos Neurais](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T1.ipynb)
> * 2. [MLP Modelo Multilayer Perceptron](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T2.ipynb)

<br>

> *Aprendizado de Máquina (Supervisionado): Métricas: Acuracidade, Precisão, Recall; Conjuntos de Treinamento e Teste; Uso dos estimadores do sci-kitlearn;*
> *Redes Neurais: Perceptron.*
 
## Aula 4 Redes Neurais

* [Deep Learning I: Modelos Sequenciais e Autoencoders](https://github.com/Rogerio-mack/Deep-Learning-I)
> * 1. [Introdução aos Modelos Neurais](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T1.ipynb)
> * 2. [MLP Modelo Multilayer Perceptron](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T2.ipynb)
>   3. [Tensores, GPU, AutoGrad e Grafos de Execução](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T3.ipynb)

> * Leitura complementar (explore): Zhang, A., Lipton, Z. C., Li, M., & Smola, A. J. (2023). [Dive into deep learning](https://d2l.ai/). Cambridge University Press.

> *Redes Neurais: Perceptron; Aprendizado e conceito de Backpropagation; XOR Problem; Redes Multi-layer Perceptron; Modelo MLP com Sci-Kit learn; Otimização de Hiper-parâmetros;*

## Aula 5 Processamento de Linguagem Natural

* [Luhn e Zipf Law](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Zipf_Law.ipynb)
* [Bag of Words, TF-IDF, Word Embeddings](https://github.com/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/IMT_TFIDF_word2vec.pdf)
* [TF-IDF, TfidfVectorizer e Feature Importance](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/TFIDF_Feature_Importance.ipynb)
* [Natural Language Processing with Python – Analyzing Text with the Natural Language Toolkit](https://www.nltk.org/book/)

> * Extra: [TensorFlow Word2Vec](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/TF_word2vec.ipynb)

> * Leitura complementar: Christopher Manning, Richard Socher. [Natural Language Processing with Deep Learning. Lecture Notes: Part I Word Vectors I: Introduction, SVD and Word2Vec](https://web.stanford.edu/class/cs224n/readings/cs224n-2019-notes01-wordvecs1.pdf)
 
> *Tarefas de NLP; Lei de Zipf; Stop Words; Pré processamento de Linguagem: Stemming e Lematização; Bag of Words; TF-IDF, TfidfVectorizer para ML; Normalização; Introdução ao Word Embeddings;*

## Aula 6 Embeddings e Deep Learning

* [Word Embedding](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Word_Embedding_spaCy_Gensim.ipynb)
* [Deep Learning I: Modelos Sequenciais e Autoencoders](https://github.com/Rogerio-mack/Deep-Learning-I)
* 1. [Tensores, GPU, AutoGrad e Grafos de Execução](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T3.ipynb)
* 2. [Modelos Sequenciais e Classificação com TensorFlow](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T4.ipynb)
* 3. [Modelos Sequencias com PyTorch](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T6.ipynb)

* [Um exemplo completo: TF-IDF, LLM-Embedding, Classificações Scikit-Learn, TensorFlow e Torch](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/TFIDF_Embedding_Classifier.ipynb)

> *Introdução ao Word Embeddings;Deep Learning: Frameworks; Tensores, GPU, AutoGrad e Grafos de Execução; Diferentes arquiteturas de Redes.*

## Aula 7 Embeddings e Deep Learning

* [Um exemplo completo: TF-IDF, LLM-Embedding, Classificações Scikit-Learn, TensorFlow e Torch](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/TFIDF_Embedding_Classifier.ipynb)
* [Representação Interna em uma Rede Neural](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Representacao_Interna_NN.ipynb)

> * Link complementar: https://poloclub.github.io/transformer-explainer/
> * Leitura complementar: Guillaume Klein et. al [OpenNMT: Open-Source Toolkit for Neural Machine Translation](https://nlp.seas.harvard.edu/2018/04/03/attention.html#encoder-and-decoder-stacks), also [**The Annotated Transformer**](https://nlp.seas.harvard.edu/2018/04/03/attention.html#encoder-and-decoder-stacks). Ou se preferir de uma forma mais didática
[**How Transformers Work: A Detailed Exploration of Transformer Architecture**](https://www.datacamp.com/tutorial/how-transformers-work)

> *Representação interna de uma rede neural; Treinamento de modelos TensorFlow e PyTorch com embeddings*

## Aula 8 Redes Convolucionais: Modelos Neurais com Imagens

* [TF Classificação de Dígitos MNIST, MLP X Conv2D](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/MLG_TF_MNIST_Classifier.ipynb)
* [CNN Explainer](https://poloclub.github.io/cnn-explainer/)
* [Classificação de Imagens: Keras/TensorFlow](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/MLG_TF_ImageClassifier.ipynb)
* [Classificação de Imagens: VGG16](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/AI_TF_ImageClassifier_VGG16.ipynb)
* [Object Detection: Yolo, ResNet](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Yolov5_Resnet50_object_detection.ipynb)

> *Convolução; Kernel, padding, pooling; Redes convolucionais; Modelos pré-treinados*

## Aula 9 Transformers & Fine Tune

* [Como os Transformers Funcionam?](https://github.com/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/4.md)
> * [Explorando os mecanismos de Atenção e a arquitetura Transformers](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Attention_and_Transformers_Explorer.ipynb)
* [Deep dive into Atenção e Transformers](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Atencao_QKV_transformers.ipynb)
* [Diferentes Tarefas com LLMs: *o pulo do gato!*](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/LLMs_Text_Classification.ipynb)

> * Leitura complementar: Géron, A. (2022). Hands-on machine learning with Scikit-Learn, Keras, and TensorFlow. [Chapter 17](https://drive.google.com/file/d/1pJAWwpLgzD4sJGYFHWsxNpWCfKwRk-qX/view?usp=sharing). O'Reilly Media, Inc.

> *Visão geral da arquitetura transformers; mecanismo de atenção; fine tune de modelos*

## Aula 10 Fine Tune LLMs, Bancos de Dados Vetoriais e RAG

* [Capítulo 6: Chabots Inteligentes na Saúde: Implementações com Modelos Abertos e Dados Próprios](https://github.com/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Capitulo_6_LLM.pdf)
* [Fine-Tunning ResNet18 com PyTorch Lightning (PL)](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Fine_Tune_Images_PyTorch_Lightning.ipynb)
* [Fine-Tunning com Hugging Face API Trainer, LoRA e QLoRA](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Hugging_Face_Trainer_API_LoRA.ipynb)
* [NoSQL Databases e Vector Stores](https://colab.research.google.com/github/Rogerio-mack/data-engineering/blob/main/A05_SQL_NoSQL.ipynb)

#### Um pipeline completo em português

* [Modelo Causal](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Modelo_Causal.ipynb)
* [Modelo Embedding](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Modelo_Causal.ipynb)
* [Modelo RAG](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Modelo_RAG.ipynb)
* [Modelo RAG FAISS](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Modelo_RAG_FAISS.ipynb)
> * [Modelo RAG FAISS](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Modelo_SQuAD.ipynb)

## Aula 11 LLM Agents e Métricas

* [LLM Metrics](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/LLM_metrics.ipynb)
* [LLM Agents](https://colab.research.google.com/github/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/LLM_Agentes.ipynb)

> * Leitura complementar (Cap 12, **Automating Preference Evaluation Using Reward Models**): Alammar, Jay, and Maarten Grootendorst. [Hands-on large language models: language understanding and generation.](https://github.com/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/Hands-On-LLM/Jay%20Alammar%2C%20Maarten%20Grootendorst%20-%20Hands-On%20Large%20Language%20Models_%20Language%20Understanding%20and%20Generation%20(2024%2C%20O%E2%80%99Reilly%20Media)%20-%20libgen.pdf) O'Reilly Media, Inc., 2024.

> * Leitura complementar, Khaled Bayoudh (2024) [**A survey of multimodal hybrid deep learning for computer vision: Architectures, applications, trends, and challenges**](https://github.com/Rogerio-mack/Modelos_de_Linguagem_e_Generativos/blob/main/multimodal_concatenate.pdf)

>> **Aula 12 Yolo (Hands On)**  - 15 de Abril de 2026 às 19:20 - 21:00, Prédio 31 - Sala 401

>> **Pré-Apresentação dos Projetos (10-15min)**

## Entrega dos Projetos: Checklist das entregas no GitHub, 22.04 18:30-19:00h
