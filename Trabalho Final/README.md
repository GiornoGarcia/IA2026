Tipos Sanguíneos

Este projeto visa treinar uma IA para que ela possa auxiliar os especialisatas de saúde na identificação de tipos sanguíneos, divididos entre A+, A-, B+, B-, AB+, AB-, O+ e O-, sendo atraves do envio de imagens do Dataset ABO-BTI ABO Blood Typing que possue diversas amostras de cada tipo para treinamento da IA.

Nome do Dataset: ABO-BTI: BO Blood Typing Image Dataset
Fonte: Kaggle
Número de amostras e features: 432 amostras, 54 para cada tipo, 8 tipos sanguíneos.
Link para download: https://www.kaggle.com/datasets/saradaas/abo-bti-bo-blood-typing-image-dataset
Breve descrição das principais variáveis: Este banco de dados contém imagens e informações de doadores para 8 grupos sanguíneos: A+, A–, B+, B–, O+, O–, AB+, AB–.
Foi coletado em duas instituições de saúde em Annaba, Argélia: o Centro Hospitalar Universitário Dr. Dorban e o Hospital Especializado Abdallah Nouaouria El Bouni.
A coleta do conjunto de dados ABO-BTI foi feita utilizando os padrões da Organização Mundial da Saúde (OMS) para tipagem sanguínea ABO e RhD.


Problemática: Classificação multiclasse, onde o modelo deve identificar uma entre várias categorias de tipos sanguíneos (A, B, AB e O, positivos e negativos) a partir de imagens. A entrada são imagens e a saída é uma classe específica entre sete possibilidades. A métrica mais adequada para avaliação é o F1-score, complementada pela acurácia.

Tecnologias utilizadas

Python 3.10+
TensorFlow / Keras
NumPy
Pandas
Scikit-learn
Matplotlib
Google Colab
Google Drive

Instalação

# =====================================================
# INSTRUÇÕES DE INSTALAÇÃO E EXECUÇÃO DO PROJETO
# =====================================================

# 1. (Opcional, recomendado) Criar ambiente virtual
python -m venv venv

# Ativar ambiente virtual (Windows)
venv\Scripts\activate

# Ativar ambiente virtual (Linux/Mac)
source venv/bin/activate


# 2. Instalar dependências necessárias
pip install tensorflow pandas numpy matplotlib seaborn scikit-learn


# 3. (Opcional) Instalar tudo via requirements.txt
pip install -r requirements.txt


# =====================================================
# CONTEÚDO DO requirements.txt
# =====================================================
tensorflow
pandas
numpy
matplotlib
seaborn
scikit-learn


# =====================================================
# OBSERVAÇÃO
# =====================================================
# Este projeto também pode ser executado no Google Colab,
# onde o TensorFlow já vem pré-instalado por padrão.

Resultados principais

Melhor modelo: Rede Neural Convolucional (CNN)
Acurácia: 96,25%
F1-score: ~0,96 (média geral das classes)
Margem de erro: 12,5% (considerando 5 erros em 40 imagens)

Etrutura do repositório

Meu Drive
--Colab Notebooks
    --Diário de Bordo
        --Dataset_Tipos_Sanguíneos
            --ABO-BTI ABO Blood Typing
                --ABO-BTI_Images
        --ABO-BTI_Images_Teste
