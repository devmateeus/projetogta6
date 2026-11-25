# Análise de Buscas: GTA 6 🎮

Este é um projeto que desenvolvi utilizando R para analisar o interesse dos brasileiros pelo **GTA 6**, com dados reais extraídos do Google Trends.

A ideia surgiu da vontade de aplicar meus conhecimentos em análise de dados em um tema que está em alta, explorando informações reais, criando visualizações e transformando dados em informações que façam sentido.

## 🎯 Objetivo

Quero entender como o interesse pelo GTA 6 se distribui pelo Brasil e como esse interesse evoluiu ao longo dos últimos anos.

Durante a análise, busco responder algumas perguntas:

- Quais estados brasileiros mais pesquisam por GTA 6?
- Como o interesse pelo jogo evoluiu nos últimos 5 anos?
- Quais acontecimentos provocaram os maiores picos de pesquisa?
- Quais são os assuntos e termos relacionados mais pesquisados?

## 📊 Fonte dos dados

Utilizei o **Google Trends** como fonte de dados, realizando a extração por meio do pacote [`gtrendsR`](https://cran.r-project.org/package=gtrendsR).

**Configurações utilizadas:**
- Termo pesquisado: GTA 6
- Região: Brasil (`geo = "BR"`)
- Período: últimos 5 anos

Uma observação importante: os dados do Google Trends são apresentados em uma escala de 0 a 100. Isso significa que os valores representam o interesse relativo de pesquisa, e não a quantidade absoluta de buscas.

Para facilitar as próximas análises, salvei os dados tratados em arquivos CSV dentro da pasta `data/`.

## 🔎 Etapas do projeto

Até o momento, desenvolvi as seguintes etapas:

- [x] Extração dos dados utilizando `gtrendsR`.
- [x] Análise do interesse por estado brasileiro.
- [x] Criação de gráfico de barras com `ggplot2`.
- [x] Exportação dos dados para CSV.
- [ ] Análise da evolução das pesquisas ao longo do tempo.
- [ ] Identificação dos principais picos de interesse.
- [ ] Investigação dos acontecimentos relacionados aos picos.
- [ ] Análise das pesquisas relacionadas ao GTA 6.

## 📈 Principais resultados

Esta seção será atualizada conforme eu avançar no projeto, incluindo gráficos, observações e descobertas obtidas durante a análise.

## 📁 Estrutura do projeto

```text
projeto-gta6/
├── data/
│   └── pesquisa_por_estado.csv
├── images/
├── projeto_gta6.R
└── README.md
```

## 🛠️ Tecnologias utilizadas

- **R:** linguagem utilizada para desenvolver a análise.
- **gtrendsR:** extração de dados do Google Trends.
- **dplyr:** organização e manipulação dos dados.
- **ggplot2:** criação de gráficos e visualizações.

## 🚀 Como executar

1. Clone este repositório:

```bash
git clone https://github.com/devmateeus/projeto-gta6.git
```

2. Instale os pacotes necessários no R:

```r
install.packages(c("gtrendsR", "dplyr", "ggplot2"))
```

3. Abra o projeto no RStudio e execute o arquivo `projeto_gta6.R`.

**Observação:** caso o Google Trends bloqueie temporariamente alguma requisição (erro 429), aguarde alguns minutos ou utilize os arquivos CSV já disponíveis na pasta `data/`.

## ⚠️ Limitações

- Os dados representam interesse relativo de pesquisa, não o volume absoluto de buscas.
- Os resultados podem variar conforme a data em que a consulta é realizada.
- O Google Trends utiliza amostragem, portanto os valores podem apresentar pequenas variações entre consultas.

## 👨‍💻 Autor

**Mateus Dantas**

Estudante de análise de dados, compartilhando projetos práticos e documentando minha evolução na área.

- [GitHub](https://github.com/devmateeus)
- [LinkedIn](https://www.linkedin.com/in/mateeusdantas/)

---

*Projeto desenvolvido como parte da minha jornada de aprendizado em análise de dados com R.*