# SparkML na Prática

Este projeto é um exemplo prático de uso do **Apache Spark** com **PySpark** para análise e modelagem de dados, incluindo:

- Configuração do ambiente Spark no Google Colab,
- Uso de `ngrok` para expor a interface web da Spark UI,
- Leitura e pré-processamento de dados JSON com estrutura complexa,
- Aplicação de técnicas de feature engineering (indexação de variáveis categóricas),
- Balanceamento de classes para detecção de fraude,
- Treinamento de um modelo de regressão logística para classificação de transações fraudulentas.

---

## Tecnologias e Bibliotecas

- Apache Spark 3.3.2 (PySpark 3.5.1)
- Java OpenJDK 11
- ngrok (para túnel e acesso remoto à Spark UI)
- Google Colab (ambiente de execução)
- Python 3
- Bibliotecas: findspark, pyspark.ml, cloudpickle

---

## Estrutura do Projeto

- `SparkML_naPratica.ipynb` - notebook contendo:
  - Configuração do ambiente Spark e ngrok no Colab,
  - Leitura do arquivo JSON com esquema customizado,
  - Flatten das estruturas aninhadas no dataframe,
  - Indexação das colunas categóricas para o modelo ML,
  - Preparação e balanceamento dos dados,
  - Treinamento de modelo de Regressão Logística,
  - Avaliação e exibição dos resultados.

---

## Como executar

1. Faça o upload do arquivo JSON `case_final.json` no seu Google Drive na pasta `arquivos e bancos de dados` (ou ajuste o caminho no código).

2. Adicione seu token `ngrok` no Colab como um segredo com o nome `NGROK_TOKEN` (ou altere o código para inserir seu token diretamente).

3. Execute as células do notebook na ordem para:
   - Instalar Java, Spark, PySpark, findspark e ngrok,
   - Configurar o SparkSession e o túnel ngrok para acessar a Spark UI,
   - Carregar e preparar os dados,
   - Treinar o modelo e verificar os resultados.

4. Acesse
---

## Objetivo

Demonstrar o uso do Apache Spark para processamento distribuído e aplicação de Machine Learning com PySpark ML, focando na detecção de fraudes em transações financeiras via análise dos dados Pix.

---

## Notas

- O dataset contém estruturas aninhadas (remetente e destinatário).
- Amostragem dos dados sem fraude foi realizada para balancear a base.
- Modelo utilizado: Regressão Logística com features derivadas.
- Código preparado para expansão com novos modelos ou técnicas.

---

## Autor

Marcio Luiz dos Santos Pereira 
