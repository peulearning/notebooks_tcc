# 📊 Projeto de TCC: HealScan - Visão Computacional

<div align="center">
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python">
  <img src="https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252" alt="Google Colab">
  <img src="https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white" alt="Keras">
  <img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white" alt="TensorFlow">
</div>

---

## 🧠 Sobre o Projeto

Este repositório contém uma coleção de notebooks desenvolvidos em Python voltados para a construção, treinamento e avaliação de modelos de **Visão Computacional**, com foco em aplicações reais e classificação de imagens (foco no projeto **HealScan**).

Os experimentos foram realizados utilizando o **Google Colab**, permitindo o uso de recursos computacionais acelerados (GPU/TPU), o que facilitou o treinamento e a iteração rápida de redes neurais profundas.

> **💡 Objetivo Principal:** Explorar e aplicar técnicas modernas de Deep Learning para Visão Computacional, criando modelos robustos, eficientes e otimizados que possam ser utilizados em aplicações práticas (como integração mobile *offline-first*), especialmente em contextos que exigem alta precisão de classificação.

---

## 🚀 Tecnologias Utilizadas

* **Linguagem & Ambiente:** 🐍 Python | ☁️ Google Colab
* **Deep Learning:** 🤖 Keras (API de alto nível do TensorFlow)
* **Manipulação de Dados:** 🔢 NumPy | Pandas
* **Visualização:** 📊 Matplotlib | Seaborn
* **Avaliação de Métricas:** 🧪 Scikit-learn

---

## 📁 Estrutura dos Notebooks (Pipeline)

Os notebooks estão organizados de forma estritamente sequencial, representando o fluxo completo de desenvolvimento e engenharia do modelo de visão computacional:

### `1.` 📂 Pré-processamento de Dados
* Carregamento e organização estrutural das imagens.
* Redimensionamento (Resizing) e Normalização dos tensores.
* Separação estratificada dos dados em conjuntos de **Treino, Validação e Teste**.

### `2.` 🔄 Data Augmentation
Aplicação de técnicas para aumentar a variabilidade do dataset, simulando condições reais e reduzindo o *overfitting*:
* Rotação, Zoom e Translação.
* *Flip* horizontal e ajuste de brilho.
* **Objetivo:** Melhorar a generalização do modelo diante de imagens inéditas.

### `3.` 🏗️ Construção dos Modelos
Exploração de diferentes arquiteturas e abordagens:
* **CNNs Customizadas:** Redes Convolucionais criadas do zero para *baseline*.
* **Transfer Learning:** Utilização de arquiteturas pré-treinadas com foco em eficiência computacional, com destaque para a **MobileNetV2**.

### `4.` 🎯 Treinamento
* Definição da topologia e dos hiperparâmetros.
* Configuração de *Loss Functions* e Otimizadores (Adam, SGD).
* Monitoramento em tempo real de métricas críticas (Acurácia e Loss).

### `5.` 📈 Avaliação de Desempenho
* Análise detalhada via **Matriz de Confusão** e Relatório de Classificação.
* Geração de curvas de aprendizado (Acurácia/Loss).
* Análise da curva ROC e cálculo da métrica AUC.

### `6.` ⚡ Otimização
* *Fine-tuning* das camadas base dos modelos de Transfer Learning.
* Ajuste fino de hiperparâmetros.
* Implementação de *Callbacks* como **Early Stopping** e **ReduceLROnPlateau** (Redução de taxa de aprendizado).

### `7.` 📦 Exportação e Testes Finais
* Salvamento dos pesos e da arquitetura dos modelos treinados (preparação para conversão para `.tflite`, por exemplo).
* Validação final com o conjunto de teste (dados nunca antes vistos pelo modelo).

---

## 📊 Resultados Alcançados

Os modelos foram rigorosamente avaliados utilizando métricas clássicas de classificação. Os destaques dos experimentos incluem:

* ✔️ **Boa capacidade de generalização** perante o conjunto de testes.
* ✔️ **Redução significativa de overfitting** após a aplicação de *Data Augmentation*.
* ✔️ **Melhoria expressiva de desempenho** ao adotar estratégias de *Transfer Learning* (MobileNetV2), equilibrando alta acurácia com baixo custo computacional.

---

## ▶️ Como Executar

1.  Acesse o [Google Colab](https://colab.research.google.com/).
2.  Faça o upload dos notebooks deste repositório (`Arquivo > Fazer upload de notebook`).
3.  Monte o seu Google Drive executando a célula correspondente, caso os datasets estejam armazenados lá.
4.  Certifique-se de alterar o tempo de execução para GPU (`Ambiente de execução > Alterar o tipo de ambiente de execução > T4 GPU`).
5.  Execute as células sequencialmente.
6.  Ajuste os diretórios de origem das imagens nos blocos de código iniciais conforme a sua estrutura de pastas.

---

## 📌 Observações

* Os notebooks foram desenvolvidos com foco educacional, experimental e acadêmico.
* Os resultados de acurácia e *loss* podem variar ligeiramente dependendo da semente aleatória (*seed*) e do *hardware* alocado pelo Google Colab no momento da execução.

---

## 👨‍💻 Autor

**Pedro Henrique Araújo Mattos Ribeiro** 
*Bacharelando em Sistemas de Informação Turma 121 - Instituto Federal do Norte de Minas Gerais Campus Januária*
