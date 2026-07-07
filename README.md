# Inspeção Visual de Transistores THT (YOLOv26)

Este projeto implementa um sistema de detecção de defeitos em componentes eletrônicos (transistores THT) utilizando a arquitetura **YOLO26**. O sistema é capaz de identificar componentes íntegros (`good`), com pinos cortados (`cut-lead`), encapsulamento danificado (`damaged-case`) ou mal posicionados (`misplaced`).

## 🛠️ Tecnologias
- **Deep Learning:** YOLO26n (via Ultralytics)
- **Interface:** Gradio (web app interativo)
- **Ambiente:** Google Colab / Python

## 🚀 Como reproduzir

1. **Dataset:** O modelo foi treinado com o dataset disponível no [Roboflow Universe](https://universe.roboflow.com/project-wzlvl/transistor).
2. **Treinamento:** Abra o notebook `Projeto_Final_Visão_Computacional.ipynb` no Google Colab.
3. **Execução:** Siga as células de instalação e carregamento de pesos.
4. **Interface:** Ao rodar a última célula, o Gradio gerará um link público (`gradio.live`). Basta clicar, fazer o upload da imagem de um transistor e visualizar a detecção.

## 📊 Resultados
O modelo apresenta métricas de detecção robustas (mAP50 de 0.86), com o detalhamento técnico e a análise crítica de viés de dados disponível no artigo acadêmico (`relatorio_final.pdf`) incluído neste repositório.

## 📁 Estrutura
- `/weights/best.pt`: Pesos do modelo treinado.
- `/images_results/`: Gráficos de treinamento e matriz de confusão.
- `Projeto_Final_Visão_Computacional.ipynb`: Código completo de treino e teste.
- `relatorio_final.pdf`: Artigo técnico detalhado.
