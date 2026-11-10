# 🌍 Global CO₂ Emissions Analysis

### Emissões globais de carbono, eficiência econômica e exposição regulatória | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboards-F2C811?logo=powerbi&logoColor=black) ![DAX](https://img.shields.io/badge/DAX-An%C3%A1lise-0B1F3A) ![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-00A86B)

Análise estratégica das emissões globais de CO₂ com foco em **concentração geográfica, desacoplamento econômico, fontes emissoras, desigualdade per capita e riscos regulatórios**. O projeto utiliza **Power BI, Power Query e DAX** para transformar dados históricos em diagnósticos relevantes para decisões de expansão internacional e descarbonização da cadeia de suprimentos.

**Autores:** Matheus Mannarino e Antônio José  
**Contexto:** Ciência de Dados nos Negócios — Ibmec, 2026  
**Fonte principal:** [Our World in Data — CO₂ and Greenhouse Gas Emissions](https://github.com/owid/co2-data)

---

## 🎯 Problema de negócio

O estudo considera o cenário de uma multinacional brasileira do setor de bens de consumo e energia que planeja expandir internacionalmente e avaliar alternativas de financiamento sustentável, como *green bonds*. Para apoiar o planejamento estratégico, investigamos onde se concentram as emissões, quais economias conseguem crescer com menor intensidade de carbono e quais mercados apresentam exigências regulatórias relevantes.

## 📌 Principais resultados

| Dimensão | Destaque |
|---|---|
| Concentração global | Os **10 maiores emissores** concentravam aproximadamente **69% das emissões globais** em 2024. |
| Crescimento econômico | Há exemplos de **desacoplamento absoluto** (PIB cresce e CO₂ cai) e **relativo** (PIB cresce mais que as emissões). |
| Fontes de emissão | **Carvão** predomina na China; **petróleo**, nos EUA; e **gás natural**, na Argentina. |
| Emissões per capita | A comparação de médias e medianas evidencia **assimetria entre países de um mesmo continente**. |
| Evolução 2000–2024 | **6 de 10 economias estratégicas** selecionadas reduziram emissões per capita; China e Índia registraram aumentos expressivos. |
| Regulação | A exposição depende de instrumentos como **EU ETS e CBAM**, além do setor e do destino das exportações. |

> **Atenção:** emissões totais, emissões por habitante e intensidade carbônica são indicadores diferentes. Os períodos e recortes são específicos de cada pergunta.

## 📊 Dashboards — cinco perguntas de negócio

### 1. Concentração e priorização geográfica

**Pergunta:** onde se concentra a maior responsabilidade pelo volume de emissões?

A análise examina o ranking de grandes emissores e a distribuição por blocos econômicos, identificando mercados com maior participação no total mundial.

![Concentração global](dashboards/Concentração%20Global%20de%20Emissões%20de%20CO₂.png)

<details>
<summary>Ver gráfico complementar — emissões por blocos econômicos</summary>

![Emissões por blocos](dashboards/Infográfico%20de%20Emissões%20de%20CO₂%20por%20Blocos.png)

</details>

### 2. Eficiência econômica e desacoplamento

**Pergunta:** crescimento do PIB exige aumento proporcional das emissões?

A comparação entre PIB e emissões identifica trajetórias de desacoplamento econômico e ressalta que volume de produção e eficiência carbônica não são equivalentes.

![Desacoplamento econômico](dashboards/Painel%20de%20Desacoplamento%20Econômico%20e%20CO₂.png)

<details>
<summary>Ver gráfico complementar — relação PIB e CO₂</summary>

![PIB e emissões](dashboards/Relação%20entre%20PIB%20e%20Emissões%20de%20CO₂.png)

</details>

### 3. Transição energética e fontes críticas

**Pergunta:** quais combustíveis e processos lideram a pegada de carbono de mercados estratégicos?

Investigamos a evolução histórica e a composição das emissões da **China, dos Estados Unidos e da Argentina**, considerando carvão, petróleo, gás natural, cimento e *flaring*.

![Composição das fontes](dashboards/Emissões%20de%20CO₂%20por%20Fonte%20em%202024.png)

<details>
<summary>Ver gráficos complementares — trajetórias dos três países</summary>

**China**

![China](dashboards/Emissões%20de%20CO₂%20da%20China%20em%20Perspectiva.png)

**Estados Unidos**

![EUA](dashboards/Painel%20de%20Emissões%20de%20CO₂%20dos%20EUA.png)

**Argentina**

![Argentina](dashboards/Emissões%20de%20CO₂%20na%20Argentina.png)

</details>

### 4. Dispersão das emissões per capita

**Pergunta:** a média de cada continente representa a realidade da maioria dos países?

A análise combina valores individuais, extremos, médias e medianas para evidenciar a heterogeneidade geográfica das emissões por habitante.

![Distribuição per capita](dashboards/Distribuição%20Global%20das%20Emissões%20de%20CO₂%20per%20Capita.png)

<details>
<summary>Ver gráfico complementar — médias e medianas por continente</summary>

![Continentes](dashboards/Emissões%20de%20CO₂%20por%20Continente%20em%202024.png)

</details>

### 5. Mudança histórica e exposição regulatória

**Pergunta:** quais economias reduziram emissões per capita desde 2000 e onde as empresas podem encontrar barreiras regulatórias mais relevantes?

O estudo compara as variações acumuladas de 2000 a 2024, examina séries históricas e complementa os indicadores com uma avaliação **qualitativa** de instrumentos regulatórios de carbono.

![Variação das emissões](dashboards/Variação%20Global%20das%20Emissões%20de%20CO₂.png)

<details>
<summary>Ver gráficos complementares — evolução e regulação</summary>

**Evolução histórica**

![Evolução](dashboards/Evolução%20Global%20das%20Emissões%20de%20CO₂%20per%20Capita.png)

**Exposição regulatória**

![Regulação](dashboards/Exposição%20Regulatória%20ao%20Carbono%20por%20Mercado.png)

</details>

## 🛠️ Metodologia

1. **Preparação da base:** importação dos dados de CO₂ e da tabela auxiliar de países/continentes no Power BI.
2. **Segmentação:** separação de países e agregados, seleção de períodos e verificação da disponibilidade dos indicadores.
3. **Medidas DAX:** cálculo de totais, participações e variações percentuais, além de comparações entre países e anos.
4. **Visualização:** rankings, gráficos de dispersão, séries temporais, composição de fontes e comparações de média e mediana.
5. **Interpretação:** síntese de insights e implicações para estratégia empresarial, fornecedores e expansão internacional.

**Limitações:** a cobertura histórica varia entre países e indicadores; o mecanismo estatístico de ausência não pode ser determinado apenas pela concentração de lacunas em anos antigos. Indicadores descritivos não estabelecem causalidade. A análise regulatória utiliza informações externas à base OWID, não representa um ranking oficial e depende de setor, localização e mercado de destino.

## 💼 Recomendações executivas

- **Priorizar mercados com visão multidimensional:** avaliar simultaneamente volume de emissões, trajetória, matriz energética e exigências regulatórias.
- **Mapear fornecedores e emissões:** considerar emissões diretas e indiretas, especialmente nas cadeias intensivas em energia.
- **Buscar eficiência carbônica:** acompanhar crescimento econômico e intensidade de emissões, identificando oportunidades de transição energética.
- **Preparar conformidade:** analisar requisitos de reporte e precificação do carbono para produtos e mercados relevantes.

## 📁 Estrutura do repositório

```text
Global-CO2-Emissions-Analysis/
├── dashboards/         # 13 visualizações em PNG
├── data/
│   ├── co2-data.csv
│   └── Dim_Paises_Continentes.csv
├── powerbi/
│   └── Tarefa_de_Analise_AC.pbix
├── docs/
│   ├── Documentacao_CO2_Global_AC_2026.pdf
│   └── Apresentacao_CO2_Global.pptx
└── README.md
```

## ▶️ Como explorar

- **Ver os resultados:** navegue pelas imagens acima ou abra a pasta [dashboards](dashboards).
- **Explorar o relatório:** baixe o [arquivo Power BI (.pbix)](powerbi/Tarefa_de_Analise_AC.pbix) e abra-o no [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
- **Consultar a metodologia:** leia a [documentação completa (PDF)](docs/Documentacao_CO2_Global_AC_2026.pdf).
- **Acessar a apresentação:** veja o [PowerPoint](docs/Apresentacao_CO2_Global.pptx).
- **Reproduzir a análise:** use os CSVs em [data](data) e, se necessário, atualize os caminhos das fontes no Power BI.

## 📚 Fontes

- [Our World in Data — CO₂ and Greenhouse Gas Emissions](https://ourworldindata.org/co2-and-greenhouse-gas-emissions)
- [OWID — Repositório de dados sobre CO₂](https://github.com/owid/co2-data)
- [Comissão Europeia — Carbon Border Adjustment Mechanism (CBAM)](https://taxation-customs.ec.europa.eu/carbon-border-adjustment-mechanism_en)
- [Comissão Europeia — EU Emissions Trading System](https://climate.ec.europa.eu/eu-action/carbon-markets/eu-emissions-trading-system-eu-ets_en)

---

**Matheus Mannarino e Antônio José · Ciência de Dados e Inteligência Artificial · Ibmec · 2026**
