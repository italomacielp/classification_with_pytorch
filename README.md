# 💻 Projetos de Sistemas baseados em Aprendizado de Máquina 

## Projeto 2: Visualização das Camadas da CNN: Um Estudo de Caso
<p align="center">
  <a href="#">
    <img src="results/Modelo%20LeNet.png" alt="Logo" width="800" height="300">
  </a>
</p>

### 🏃 Componentes
1. Paula Souza
2. Ítalo Maciel

### 📌 Descrição do projeto
O Trabalho da Unidade 02 é um Estudo de Caso que visa a Visualização das Camadas da CNN (Rede Neural Convolucional).

O projeto exige a manipulação de componentes específicos, mantendo a arquitetura-base (LeNet-like) como visto em aula, adaptando apenas in_channels se necessário.

A tarefa principal é aplicar a predição da arquitetura da CNN sobre essas imagens,culminando na visualização gráfica de imagens e seus rótulos correspondentes.

O estudo está inserido no contexto da exploração de CNNs com PyTorch e deve ser entregue até o dia 23 de novembro de 2025 (23h59).

### ▶️ Instruções para executar o código
É necessário realizar o upload do notebook disponibilizado no repositório no ![colab](https://colab.research.google.com/). Acessando o menu, seguir o seguinte fluxo: Arquivo → Fazer Upload de Arquivo.

Após realizar o upload, pode executar cada célula ou clicar na opção *Executar tudo*.

### 🚧 Arquitetura
A classe Architecture serve como um contêiner completo para treinamento, validação, análise e visualização de modelos em PyTorch. 

Ela recebe o modelo, a função de perda e o otimizador, configurando automaticamente o dispositivo (CPU/GPU) e gerenciando loaders de treino e validação. A classe cria funções internas de train step e validation step, que executam o forward, calculam a perda, fazem o backward e atualizam os pesos quando necessário, também controla todo o loop de treinamento, armazenando perdas, épocas e permitindo salvar e carregar checkpoints. 

Além disso, oferece métodos para prever novos dados, contar parâmetros, visualizar filtros de camadas convolucionais, registrar hooks para capturar ativações internas e plotar curvas de perda. Por fim, inclui funções utilitárias como definição de semente, avaliação de acurácia por classe e aplicação de operações ao longo dos loaders.

### 🚋 Estrutura da arquitetura base (Modelo LeNet-like)
A arquitetura segue uma estrutura padrão do modelo LeNet, contendo a parte

### 📁  Base de Dados

Nesse trabalho estamos analisando o conjunto de dados MNIST. Esse banco de imagens é um dos mais utilizados em estudos e experimentos envolvendo reconhecimento de padrões, 
servindo como uma base ideal para observar o desempenho de modelos de visão computacional em tarefas simples de classificação.

O MNIST reúne 60.000 imagens em tons de cinza cada uma com resolução 28×28 pixels, contendo registros de dígitos manuscritos.

Esses exemplos estão organizados em 10 categorias, representando os números de 0 a 9. 
Essa estrutura compacta e padronizada facilita a compreensão dos primeiros passos na construção e treinamento de modelos convolucionais.

### 📊 Explicação dos seus resultados e observações

### 🎥 Link para o vídeo da sua apresentação
![LINK DA APRESENTAÇÃO]()

### ✅ Checklist de Entrega

| Item | Descrição | Status |
|------|--------------|--------|
| Dataset | Escolher um dataset do torchvision.datasets | ✅ |
| Arquitetura | Manter a arquitetura-base (LeNet-like) como visto em aula, adaptando apenas in_channels se necessário. | ✅|
| Loss Functions/Métricas | Treinar o modelo e registrar métricas de loss e accuracy (treino/val) | ✅ |
| Hooks | Implementar Hooks para capturar ativações intermediárias. | ✅ |
| Visualização | Visualizar os feature maps de todas camadas. | ✅ |
| Análise | Escrever uma breve análise (1-2 parágrafos) sobre o que foi observado. | ✅ |
| Video | Gravar um vídeo de até 10min sobre o que foi observado. | ☐ |
| Repositório | Organizar um repositório no Github com tudo o que foi desenvolvido, incluindo um arquivo README.md descrevendo todoо trabalho em detalhes. | ✅ |
---