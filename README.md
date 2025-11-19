# 🏭 Eficiência Energética na Indústria 4.0: Análise de Dados e Simulação em Siderúrgica

## Integrantes
- Gabriel Nacarelli Pinheiro – RM: 565298 
- Mateus Patrício Pereira – RM: 564695
- Raphael Talarico – RM: 565219

## Sobre o Projeto

Este projeto aborda o desafio da sustentabilidade em ambientes industriais de alto consumo. Utilizando **dados reais** de uma indústria siderúrgica, desenvolvemos uma solução baseada em Análise de Dados e Simulação Computacional para otimizar o consumo energético, reduzir custos operacionais e mitigar a emissão de carbono.

A solução conecta o **Futuro do Trabalho** com a responsabilidade ambiental, demonstrando como a tomada de decisão baseada em dados (Data-Driven) pode transformar rotinas produtivas.

---

## Fonte de Dados (Dados Reais)

Os dados utilizados neste projeto são provenientes de uma **Siderúrgica (Steel Industry)** localizada na cidade de Gwangyang, Coreia do Sul.
* **Fonte:** UCI Machine Learning Repository (DAEWOO Steel Co. Ltd).
* **Volume:** 35.040 medições (registros a cada 15 minutos durante um ano inteiro).
* **Variáveis Principais:** Consumo de Energia Ativa (kWh), Potência Reativa (kVarh), Emissões de CO₂ (tCO₂), Fator de Potência e Tipos de Carga (*Light*, *Medium*, *Maximum*).

---

## Objetivos e Solução Proposta

O objetivo central é responder: **"Como podemos tornar uma indústria pesada mais eficiente e sustentável sem prejudicar a produção?"**

A solução foi desenvolvida em duas frentes complementares:

### 1. Diagnóstico de Eficiência (Opção A)
Realizamos uma Análise Exploratória de Dados (EDA) profunda para identificar padrões de desperdício.
* **Metodologia:** Criação de **Mapas de Calor (Heatmaps)** para cruzar hora do dia vs dia da semana.
* **Descoberta:** O consumo crítico e o desperdício de energia reativa concentram-se nos **dias úteis entre 08h e 18h**, coincidindo com tarifas energéticas mais caras.
* **Diagnóstico:** A fábrica opera com alta ineficiência reativa durante os picos de carga (*Maximum_Load*).

### 2. Simulação de Solução Sustentável (Opção C)
Desenvolvemos um algoritmo em Python para simular a modernização da planta.
* **Integração de Renováveis:** Simulação da instalação de uma usina solar fotovoltaica de **150 kWp**, modelada com curvas de geração senoidais baseadas na incidência solar.
* **Gestão Inteligente de Tarifas:** Algoritmo que calcula o impacto financeiro de migrar o consumo da rede para a geração própria nos horários de ponta (tarifas elevadas).

---

## Impacto na Rotina Produtiva e Sustentabilidade

A aplicação desta solução promove melhorias diretas no ambiente de trabalho:

* **Ambientes Mais Econômicos:** A simulação financeira projeta uma redução drástica nos custos fixos, liberando capital para investimento em segurança e tecnologia.
* **Operação Inteligente:** A automação da análise de dados elimina a necessidade de leitura manual de medidores e permite ajustes proativos de carga (Load Shifting).
* **Responsabilidade Ambiental:** A redução direta do consumo da rede elétrica diminui a demanda por fontes fósseis nos horários de pico, e uma consequente descarbonização da operação.

### Resultados da Simulação (Estimados)

| Métrica | Resultado Anual | Impacto |
| :--- | :--- | :--- |
| **Economia Financeira** | **~R$ 118.790,00** | Redução direta de OPEX (Custo Operacional). |
| **Energia Economizada** | **~25%** da demanda | Menor dependência da rede pública. |
| **Sustentabilidade** | **~104 Toneladas de CO₂** | Equivalente ao plantio de centenas de árvores. |

---

## Ferramentas

* **Linguagem:** Python
* **Bibliotecas de Análise:** `pandas`, `numpy`
* **Visualização de Dados:** `matplotlib`, `seaborn`
* **Ambiente de Desenvolvimento:** Google Colab

---

## Como Executar o Projeto

Para replicar as análises e simulações:

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/](https://github.com/)[SEU-USUARIO]/Energy-Efficiency-Analysis.git
    ```
2.  **Abra o Notebook:**
    Recomendamos utilizar o **Google Colab** para execução sem necessidade de instalação local. Basta fazer upload do arquivo `.ipynb`.
3.  **Carregue os Dados:**
    Certifique-se de que o arquivo `Steel_industry_data.csv` esteja no mesmo diretório do script ou faça o upload na sessão do Colab.
4.  **Execute as Células:**
    Rode o código sequencialmente para gerar os diagnósticos (Heatmaps) e os gráficos de viabilidade econômica.
