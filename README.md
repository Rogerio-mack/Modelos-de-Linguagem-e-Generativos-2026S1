# Modelos_de_Linguagem_e_Generativos
rogerio.oliveira@mackenzie.br

<br>

### **Link dos Encontros Síncronos**

> * [09 Março](https://teams.microsoft.com/l/meetup-join/19%3ameeting_OTlmMTY5YTEtMDgxYS00NDhjLWIxMDktM2ZlOTQ1ZmI0Yjkw%40thread.v2/0?context=%7b%22Tid%22%3a%2251da9440-4e5e-47b3-8e5c-4817f6f43c04%22%2c%22Oid%22%3a%22e7fc012e-6f57-4879-9416-93179af90e74%22%7d) | [23 Março](https://teams.microsoft.com/l/meetup-join/19%3ameeting_OTlmMTY5YTEtMDgxYS00NDhjLWIxMDktM2ZlOTQ1ZmI0Yjkw%40thread.v2/0?context=%7b%22Tid%22%3a%2251da9440-4e5e-47b3-8e5c-4817f6f43c04%22%2c%22Oid%22%3a%22e7fc012e-6f57-4879-9416-93179af90e74%22%7d) | [30 Março](https://teams.microsoft.com/l/meetup-join/19%3ameeting_OTlmMTY5YTEtMDgxYS00NDhjLWIxMDktM2ZlOTQ1ZmI0Yjkw%40thread.v2/0?context=%7b%22Tid%22%3a%2251da9440-4e5e-47b3-8e5c-4817f6f43c04%22%2c%22Oid%22%3a%22e7fc012e-6f57-4879-9416-93179af90e74%22%7d)

<br>

### Exercícios (20%)

Ex1. `scikit-ML-<seu nome>.ipynb`, aprendizado supervisionado
Ex2. `scikit-MLP-<seu nome>.ipynb`, MLP

Link para entrega dos exercícios [aqui](https://drive.google.com/drive/folders/15IQW5jpljaU1W_Ol0G1sU67gFKJF6a8E?usp=drive_link). 

<br>

### **Projeto: Simulação de Opinião Pública (*Silicon Sampling*) (80%)**

Com base em uma pesquisa de opinião do [Cesop](https://www.cesop.unicamp.br/) (Centro de Estudos de Opinião Pública) desenvolver um modelo LLM e um modelo de aprendizado supervisionado para simulação das respostas dos questionários e comparar seus resultados. [Escolha aqui a pesquisa de opinião](https://drive.google.com/drive/folders/10Zv1waT-aTPFsYhZ6l1CSa3feDEBZ1R2?usp=sharing).

1. **Organização e datas**. Trabalho em grupo. Sugestão de 2-3 grupos. Entrega e apresentação do projeto no final do curso, com data a definir. Cada grupo deve escolher uma pesquisa de opinião diferente para o trabalho.
2. **Requisitos mínimos**. Ter como ponto de partida o artigo *Simulating Public Opinion: Comparing Distributional and Individual-Level Predictions from LLMs and Random Forests*, disponível na [pasta](https://drive.google.com/drive/folders/10Zv1waT-aTPFsYhZ6l1CSa3feDEBZ1R2?usp=sharing). Empregar no mínimo 200 simulações Comparar acuracidade (verificar métricas), distribuições das respostas e explicabilidade (importância relativa das variáveis preditoras). Simular ao menos 200 respondentes (10% dos dados), incluindo o maior número possível de características e respostas (sugestão: começe com um pequeno número respondentes, características e respostas, e aumente gradualmente).     
3. **Ferramentas**. Empregue somente modelos e recursos abertos, sendo 100% executável e aberto. Preferencialmente executar 100% em um notebook Colab. 
4. **GitHub**. Implementar um GitHub com o projeto.
5. **Entrega**. No formato de um artigo SBC, preferencialmente em Latex. Apresentação opcional no YouTube (máximo 5min) com o link a ser incluído no GitHub.
6. **Rubrica**. Modelo LLM, 3p (quantidade de atributos e respostas, qualidade dos prompts e aderência das respostas); Modelo Supervisionado, 2p (separação de dados, parametrização do modelo); Análise e Comparação dos resultados, 3p (métricas empregadas, repetições e/ou bootstrapping, gráficos comparativos, técnicas de explicabilidade); Artigo e Aspecto Geral do Trabalho, 2p (Apresentação, fundamentação, referências, apresentação dos resultados).

**Extra**: Esse projeto pode ser estendido adicionando-se a comparação com a simulação de respostas a partir do *fine-tunning* do modelo. Este trabalho entretanto, já daria uma dissertação. 

<br>

## Aula 1

* [Questionário pré-curso](https://forms.gle/LkD3H8LBB6GpvZLv7)
* [Plano de Ensino](https://github.com/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Plano_de_Ensino_Modelos_de_Linguagem_e_Generativos_20250416.pdf)
* [Introdução](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/MLG_01_Introducao.ipynb)

> * Leitura complementar (Cap 1): Alammar, Jay, and Maarten Grootendorst. [Hands-on large language models: language understanding and generation.](https://github.com/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Hands-On-LLM/Jay%20Alammar%2C%20Maarten%20Grootendorst%20-%20Hands-On%20Large%20Language%20Models_%20Language%20Understanding%20and%20Generation%20(2024%2C%20O%E2%80%99Reilly%20Media)%20-%20libgen.pdf) O'Reilly Media, Inc., 2024.
<br>

> *Programa; Visão geral do curso; Introdução ao processamento de linguagem natural; representações vetorais BOW, TF-IDF; similaridade cosseno; outras representações vetorais; tarefas de modelos de linguagem; importância dos termos no aprendizado de máquina.*

## Aula 2

* [Aprendizado de Máquina Supervisionado](https://github.com/Rogerio-mack/Machine-Learning-I) *Cap. 1, 4, 5*
> * 1. [Introdução ao Aprendizado de Máquina](https://colab.research.google.com/github/Rogerio-mack/Machine-Learning-I/blob/main/ML1_introducao.ipynb)
> * 4. [Classificação: Knn](https://colab.research.google.com/github/Rogerio-mack/Machine-Learning-I/blob/main/ML4_Knn.ipynb)
> * 5. [Árvores de Decisão e Seleção de Atributos](https://colab.research.google.com/github/Rogerio-mack/Machine-Learning-I/blob/main/ML5_DecisionTrees.ipynb)

<br>

> *Aprendizado de Máquina (Supervisionado): Cap1. Classificação e Regressão; Cap4. Knn; Cap. Árvores de Decisão; Fronteira de Decisão; Sobreajuste.*

## Aula 3

* [Entenda como empregar os estimadores de regressão e classificação do scikit-learn](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/IA_scikit_learn_estimadores.ipynb)
* [Aprendizado Supervisionado: Breast Câncer](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/scikit_learn_breast_cancer.ipynb)
* [Classificação e Métricas](https://colab.research.google.com/github/Rogerio-mack/Modelos-de-Linguagem-e-Generativos-2026S1/blob/main/Overfitting_Treinamento_e_Teste.ipynb)

* [Deep Learning I: Modelos Sequenciais e Autoencoders](https://github.com/Rogerio-mack/Deep-Learning-I)
> * 1. [Introdução aos Modelos Neurais](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T1.ipynb)
> * 2. [MLP Modelo Multilayer Perceptron](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T2.ipynb)

<br>

> *Aprendizado de Máquina (Supervisionado): Métricas: Acuracidade, Precisão, Recall; Conjuntos de Treinamento e Teste; Uso dos estimadores do sci-kitlearn;*
> *Redes Neurais: Perceptron.*
 
> ## Aula 4

* [Deep Learning I: Modelos Sequenciais e Autoencoders](https://github.com/Rogerio-mack/Deep-Learning-I)
> * 1. [Introdução aos Modelos Neurais](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T1.ipynb)
> * 2. [MLP Modelo Multilayer Perceptron](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T2.ipynb)
>   3. [Tensores, GPU, AutoGrad e Grafos de Execução](https://colab.research.google.com/github/Rogerio-mack/Deep-Learning-I/blob/main/T3.ipynb)

> *Redes Neurais: Perceptron; Aprendizado e conceito de Backpropagation; XOR Problem; Redes Multi-layer Perceptron; Modelo MLP com Sci-Kit learn; Otimização de Hiper-parâmetros;*
> *Deep Learning: Frameworks; Tensores, GPU, AutoGrad e Grafos de Execução; Diferentes arquiteturas de Redes.*
