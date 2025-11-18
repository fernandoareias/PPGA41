# RSL Protocolos - Revisão Sistemática da Literatura sobre Design de Novos Protocolos de Rede

## 📋 Sobre o Projeto

Este projeto contém uma **Revisão Sistemática da Literatura (RSL)** focada no estudo de novos protocolos de rede, especificamente protocolos de camada de aplicação. A pesquisa analisa publicações científicas dos últimos 5 anos (2020-2025) extraídas de bases de dados acadêmicas de renome.

## 🎯 Objetivo

Realizar uma análise sistemática e abrangente das publicações científicas sobre design de novos protocolos de rede, identificando tendências, padrões e áreas de interesse na pesquisa acadêmica.

## 📊 Estrutura do Projeto

```
PPGA41/
├── analises/
│   └── analise.ipynb          # Notebook Jupyter com todas as análises
├── bases/
│   ├── acm.bib                 # Referências da ACM Digital Library
│   ├── IEEE Xplore Citation... # Referências da IEEE Xplore
│   └── web-of-science.bib      # Referências do Web of Science
├── exports/
│   ├── data_extraction.xls     # Dados extraídos dos estudos selecionados
│   ├── protocolos_dominios.csv # Tabela de protocolos por domínio
│   └── study_selection.xls     # Dados da seleção de estudos
├── graficos/
│   ├── accepted_articles_per_source.png
│   ├── articles_per_source.png
│   └── final_articles_per_year.png
└── README.md
```

## 📈 Estatísticas Principais

### Volume de Publicações
- **Total de publicações analisadas**: 396
- **Publicações aceitas**: 27
- **Taxa de aceitação**: 6.8%
- **Período analisado**: 2020-2025

### Distribuição por Ano
| Ano | Total | Aceitas | Taxa de Aceitação |
|-----|-------|---------|-------------------|
| 2020 | 35 | 7 | 20.0% |
| 2021 | 37 | 7 | 18.9% |
| 2022 | 51 | 1 | 2.0% |
| 2023 | 108 | 4 | 3.7% |
| 2024 | 108 | 6 | 5.6% |
| 2025 | 57 | 2 | 3.5% |

### Critérios de Rejeição
- **Estudo fora do escopo**: 92.39%
- **Estudos secundários ou terciários**: 4.89%
- **Sem acesso**: 2.17%
- **Livros**: 0.27%
- **Estudos anteriores a 2020**: 0.27%

## 🔍 Análises Realizadas

### QS1: Evolução do Volume de Publicações
Análise temporal da evolução do número de publicações sobre design de protocolos de rede nos últimos 5 anos.

### QS2: Estudos Mais Influentes
Identificação dos top 5 estudos mais relevantes baseado em critérios como:
- Presença de DOI
- Recência da publicação
- Qualidade do abstract
- Presença de palavras-chave
- Veículo de publicação (IEEE, ACM, Springer, Elsevier)

### QS6: Distribuição Geográfica
Análise da distribuição geográfica das publicações, identificando países e continentes com maior produção científica no tema.

### Análise de Tópicos e Palavras-chave
- Identificação das principais palavras-chave
- Categorização por áreas de interesse (Segurança, IoT, Redes, Web, Cloud, etc.)
- Geração de nuvem de palavras

### Domínios de Aplicação
Identificação dos principais domínios onde novos protocolos são desenvolvidos:
- **IoT**: 9 publicações
- **Geral**: 7 publicações
- **Wireless**: 3 publicações
- **MAC**: 2 publicações
- **P2P**: 1 publicação

### Simuladores Utilizados
Análise das ferramentas de simulação utilizadas nas pesquisas:
- Não informado/Não utilizado: 14
- Próprio: 3
- OMNeT++: 2
- OPNET: 2
- Outros: NS-3, Spin, Blockchain Network Simulator, etc.

## 🛠️ Tecnologias Utilizadas

- **Python 3.12**
- **Jupyter Notebook**
- **Bibliotecas principais**:
  - `pandas`: Manipulação e análise de dados
  - `matplotlib`: Visualização de dados
  - `seaborn`: Visualizações estatísticas avançadas
  - `wordcloud`: Geração de nuvens de palavras
  - `fuzzywuzzy`: Correspondência de strings
  - `networkx`: Análise de redes (se aplicável)

## 📚 Bases de Dados Utilizadas

1. **ACM Digital Library**
2. **IEEE Xplore**
3. **Web of Science**

## 📁 Arquivos Principais

### `analises/analise.ipynb`
Notebook Jupyter contendo todas as análises estatísticas, visualizações e processamento de dados. Inclui:
- Carregamento e limpeza de dados
- Análises temporais
- Análises geográficas
- Análise de palavras-chave e tópicos
- Geração de gráficos e visualizações

### `exports/study_selection.xls`
Planilha Excel contendo os dados da seleção de estudos, incluindo:
- Status (Accepted/Rejected)
- Critérios de seleção
- Informações bibliográficas
- Metadados das publicações

### `exports/data_extraction.xls`
Planilha Excel com dados extraídos dos estudos aceitos, incluindo:
- Nome dos protocolos
- Domínios de aplicação
- Universidades envolvidas
- Países das publicações
- Simuladores utilizados

## 🚀 Como Utilizar

### Pré-requisitos

```bash
pip install pandas matplotlib seaborn wordcloud fuzzywuzzy networkx jupyter
```

### Executar Análises

1. Abra o Jupyter Notebook:
```bash
jupyter notebook analises/analise.ipynb
```

2. Execute as células sequencialmente para reproduzir as análises.

3. Os gráficos serão exibidos inline e podem ser salvos na pasta `graficos/`.

## 📊 Principais Resultados

### Top 5 Estudos Mais Influentes
1. **ACP+: An Age Control Protocol for the Internet** (2024) - Score: 24
2. **PC-RPL: Joint Control of Routing Topology and Transmission Power** (2020) - Score: 23
3. **Kadcast-NG: A Structured Broadcast Protocol for Blockchain Networks** (2023) - Score: 23
4. **Novel Architecture and Heuristic Algorithms for Software-Defined Wireless Sensor Networks** (2020) - Score: 21
5. **Understanding the Long Tail Latency of TCP in Large-Scale Cloud Networks** (2025) - Score: 21

### Principais Veículos de Publicação
- ACM Digital Library: 16 publicações
- IEEE Digital Library: 4 publicações
- IEEE/ACM Trans. Netw.: 3 publicações
- ACM Trans. Sen. Netw.: 1 publicação

### Top Palavras-chave
- transport protocols (4 ocorrências)
- tcp (3 ocorrências)
- protocols (3 ocorrências)
- application layer protocol (2 ocorrências)
- low latency communication (2 ocorrências)

## 📝 Notas

- Os dados foram coletados até outubro de 2025
- A taxa de aceitação baixa (6.8%) reflete critérios rigorosos de seleção
- A maioria das rejeições (92.39%) ocorreu por estudos fora do escopo definido
- O pico de publicações ocorreu em 2023 e 2024 (108 publicações cada)

## 👤 Autor

Projeto desenvolvido no contexto da disciplina PPGA41 do programa de mestrado.

## 📄 Licença

Este projeto é acadêmico e destinado a fins de pesquisa e estudo.

---

**Última atualização**: 2025
