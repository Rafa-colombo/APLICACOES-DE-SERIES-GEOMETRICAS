# 🏀 Aplicações de Séries Geométricas: Simulação 3D em Python

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Física](https://img.shields.io/badge/Física-Cinemática-orange?style=for-the-badge)
![Matemática](https://img.shields.io/badge/Matemática-Cálculo%203-green?style=for-the-badge)

## 📖 Sobre o Projeto
Este é um projeto interdisciplinar que une **Cálculo 3, Estatística e Física** através da programação. O sistema implementa um algoritmo em Python focado em simular o lançamento de uma bola, modelando o comportamento matemático dos seus saltos sucessivos e seus movimentos em um plano 3D. 

A estrutura do código e a física desenvolvida formam uma base sólida para demonstrações de séries geométricas e servem de excelente material de apoio para apresentações em eventos acadêmicos de ciência e tecnologia, como o COBICET.

## ✨ Funcionalidades e Motor Físico

* **Múltiplos Ambientes Gravitacionais:** Escolha entre 5 corpos celestes (Terra, Marte, Júpiter, Vênus e Lua), cada um com sua gravidade específica e uma identidade visual 3D própria na simulação.
* **Física de Materiais:** O simulador possui um banco de dados com a densidade e o coeficiente de restituição de 8 materiais diferentes (Borracha, PVC, Madeira, Gelo, Cimento, Ferro, Aço e Ósmio), permitindo o cálculo dinâmico da massa e do comportamento do impacto.
* **Resistência do Ar (Arrasto):** A simulação não ocorre no vácuo perfeito. O sistema calcula o arrasto atmosférico atuando na esfera utilizando a formulação de Stokes, onde o coeficiente de Stokes é definido por:
    $$b = 6 \pi \eta r$$
    *(Sendo $\eta$ a viscosidade do ar e $r$ o raio da bola).* 
* **Renderização 3D em Tempo Real:** Utiliza a biblioteca `vpython` para desenhar o ambiente, a trajetória parabólica com rastro e a colisão no solo, ajustando o centro da câmera dinamicamente.
* **Geração de Gráficos Analíticos:** Plota instantaneamente o decaimento exponencial da altura e da distância horizontal a cada quique, demonstrando visualmente o comportamento da Série Geométrica.
* **Interface de Relatórios Integrada:** Utiliza `tkinter` para gerar uma tabela de dados (Dataframe) com o resumo da simulação, calculando a razão analítica entre as alturas dos quiques sucessivos para validar o coeficiente de restituição:
    $$e = \sqrt{\frac{h_n}{h_{n-1}}}$$

## 🚀 Instruções para Execução da Simulação

Preparamos duas formas de rodar o projeto, garantindo acessibilidade para todos os usuários:

### Opção 1: Caso você já tenha o Python instalado no computador 🐍
1. Clone este repositório ou faça o download dos arquivos.
2. Localize o arquivo `rodar.bat` na pasta raiz do projeto.
3. Dê dois cliques sobre ele.
4. A simulação será compilada e iniciada automaticamente.

### Opção 2: Caso você NÃO tenha o Python instalado ⚙️
Não se preocupe, é possível rodar a versão portátil sem precisar instalar nada:
1. Acesse o nosso [Drive do Projeto](https://drive.google.com/drive/u/1/folders/1hrkQ6KT9Tzk2gR-ZWeA1-NuMl6duYgnH).
2. Baixe e extraia a pasta `exe_vLeve.zip` para dentro do diretório deste projeto.
3. Dê dois cliques no arquivo `start.bat`.
4. O programa será executado utilizando o interpretador Python portátil que acompanha os arquivos extraídos.

## 👨‍💻 Contato e Contribuições
Sinta-se à vontade para explorar o código, abrir *issues* para tirar dúvidas ou enviar *pull requests* com melhorias para o algoritmo!
