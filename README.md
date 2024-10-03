
# Fuzzy Controle Arcondicionado
Este projeto implementa um sistema de controle temperatura de ar-condicionado utilizando lógica fuzzy. 
Com o objetivo de indicar a temperatura ideal do ar-condicionado com base em fatores como a temperatura ambiente, umidade, tamanho do cômodo e problemas respiratórios do usuário.

# Descrição do Projeto
Este sistema fuzzy simula o controle da temperatura do ar-condicionado em resposta a entradas ambientais e condições de saúde, ajustando a temperatura de forma inteligente para maximizar o conforto e a segurança do usuário.

## Variáveis de Entrada

- **Temperatura Ambiente (°C):** Varia de 0 a 40°C, categorizada como fria, amena ou quente.

- **Umidade (%):** Varia de 0 a 100%, categorizada como baixa, média ou alta.

- **Tamanho do Cômodo (m²):** Varia de 9 a 60m², categorizado como pequeno, médio ou grande.

- **Problema Respiratório:** Categorizado como sem, leve ou grave (representado em graus de 0 a 100).

## Variável de Saída
- **Temperatura do Ar-condicionado (°C):** O sistema pode sugerir valores entre 15 e 28°C, categorizados como desligado, baixa, média ou alta.

## Regras de Controle Fuzzy
As regras fuzzy controlam como a temperatura do ar-condicionado deve ser ajustada com base nos valores das entradas. Por exemplo:

- **Ar-condicionado desligado:** Quando a temperatura ambiente é fria ou o usuário tem problemas respiratórios graves com umidade baixa.

- **Temperatura alta:** Quando a umidade é média e o problema respiratório é grave, ou em condições de temperatura amena e cômodos pequenos/médios.

- **Temperatura média:** Quando a temperatura é amena e o cômodo é grande com umidade média ou alta.

- **Temperatura baixa:** Quando a temperatura ambiente é quente ou amena com alta ou média umidade.

## Defuzzificação
O método de defuzzificação utilizado é o **mom** (Maximum of Maximum), que seleciona o valor médio da saída fuzzy.
## Stack utilizada

- **Python:** Linguagem de programação principal utilizada para desenvolver a lógica do sistema fuzzy.

- **Scikit-Fuzzy:** Biblioteca Python para lógica fuzzy, usada para definir e controlar as variáveis fuzzy e regras do sistema.

- **Numpy:** Biblioteca Python para computação científica, utilizada para criar os universos de entrada e saída e realizar cálculos matemáticos eficientes.

- **Matplotlib** (internamente usada pelo Scikit-Fuzzy): Ferramenta de visualização para gerar gráficos das funções de pertinência e da saída fuzzy ajustada.

- **Google Colab:** Ambiente de notebooks utilizado para o desenvolvimento, simulação e execução do código.



## Demonstração

![Grafico de temperatura](https://github.com/DanyloHenrique/FuzzyControleArcondicionado/blob/main/graficos/grafico-temperatura.png)

![Grafico de umidade](https://github.com/DanyloHenrique/FuzzyControleArcondicionado/blob/main/graficos/grafico-umidade.png)

![Grafico de tamanho do comodo](https://github.com/DanyloHenrique/FuzzyControleArcondicionado/blob/main/graficos/grafico-tamanhoComodo.png)

![Grafico de problema respiratório](https://github.com/DanyloHenrique/FuzzyControleArcondicionado/blob/main/graficos/grafico-problemaRespiratorio.png)

![Grafico de temperatura do ar-condicionado](https://github.com/DanyloHenrique/FuzzyControleArcondicionado/blob/main/graficos/grafico-temperaturaArcondicionado.png)

