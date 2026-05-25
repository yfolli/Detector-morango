# Projeto de Visão Computacional: Detecção de Qualidade de Morangos

Este projeto tem como objetivo a implementação de um pipeline de visão computacional para a classificação automática de morangos em duas categorias: **'Morango Bom'** e **'Morango Ruim'**, utilizando a arquitetura YOLO (You Only Look Once).

## 🛠️ Tecnologias e Ferramentas
* **Modelo:** YOLOv8 (framework Ultralytics)
* **Dataset:** Imagens anotadas via Roboflow
* **Ambiente de Desenvolvimento:** Google Colab
* **Armazenamento e Integração:** Google Drive
* **Linguagem:** Python

## 📊 O Pipeline de Desenvolvimento
O projeto foi estruturado em etapas essenciais de engenharia de software e IA:
1. **Coleta e Rotulagem:** Seleção e anotação de imagens para criar a base de dados.
2. **Treinamento:** Processo de aprendizado onde o modelo ajustou seus pesos para distinguir os padrões das classes.
3. **Validação:** Análise da convergência do modelo através de métricas de treino (`results.png`).
4. **Inferência:** Execução de testes em novas imagens para verificar o funcionamento do sistema.



[Image of machine learning data pipeline]


## 🔍 Análise de Resultados: Por que algumas imagens funcionam e outras não?

O projeto atingiu seu objetivo técnico, que era a criação de um **Pipeline de IA funcional**. No entanto, observou-se uma variação significativa na precisão da detecção. Abaixo, a análise técnica dessa ocorrência:

### 1. Limitação da Base de Dados (Dataset)
O treinamento foi realizado com uma base restrita de **10 imagens**. Em modelos de aprendizado profundo (*Deep Learning*), essa quantidade é insuficiente para que o modelo aprenda características gerais (como variações de iluminação, diferentes ângulos de câmera ou texturas distintas). Por isso, o modelo funciona apenas em casos específicos que se assemelham muito às fotos utilizadas no treinamento inicial.

### 2. Validação do Pipeline
O código foi construído de forma robusta e validado com sucesso em cenários controlados. A detecção funcionou em casos específicos, provando que o fluxo de integração (Colab + Drive + Pesos do YOLO) está operante. A falha em detecções mais complexas não é uma falha de código, mas uma evidência direta da dependência de um dataset maior (*Data-driven*).

### 3. Conclusão Técnica
Este projeto funcionou como uma **Prova de Conceito (PoC)**. A discrepância entre as imagens que o modelo identifica e as que ele ignora nos permite concluir que:
* O sistema de detecção está operacional.
* A precisão é diretamente proporcional à diversidade e volume do dataset.
* O próximo passo lógico é a aplicação de técnicas de *Data Augmentation* para tornar o modelo mais resiliente a variações.



## 🚀 Lições Aprendidas
Este trabalho permitiu compreender na prática que a IA vai muito além da codificação. A qualidade da solução está na qualidade da curadoria dos dados. O desafio enfrentado não foi um erro, mas uma etapa fundamental no aprendizado de qualquer engenheiro de dados.

---
*Projeto desenvolvido como parte do aprendizado em Visão Computacional e IA.*
