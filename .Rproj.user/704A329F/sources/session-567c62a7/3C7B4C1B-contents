# Análise de Buscas: GTA 6

Projeto de análise de dados em R que investiga o interesse dos brasileiros pelo **GTA 6**, usando dados reais do Google Trends.

## Objetivo

Entender como o interesse pelo jogo se distribui pelo Brasil e ao longo do tempo, respondendo perguntas como:

- Quais estados mais pesquisam por GTA 6?
- Como o interesse evoluiu nos últimos 5 anos?
- Quais momentos (trailers, adiamentos, anúncios) provocaram picos de busca?
- Quais são as buscas relacionadas mais populares?

## Dados

Os dados vêm do **Google Trends**, obtidos pelo pacote [`gtrendsR`](https://cran.r-project.org/package=gtrendsR):

- **Termo:** "GTA 6"
- **Região:** Brasil (`geo = "BR"`)
- **Período:** últimos 5 anos

> **Atenção:** os valores do Google Trends vão de 0 a 100 e são **relativos**. O 100 representa o pico de interesse dentro do período e da região consultados, e não o número real de buscas.

Os dados tratados são salvos em `data/` para que o script não dependa do Google a cada execução.

## O que foi feito

- [x] Importação dos dados com `gtrendsR`
- [x] Interesse por estado, com gráfico de barras ordenado (`ggplot2`)
- [x] Exportação dos dados para CSV
- [ ] Evolução do interesse ao longo do tempo
- [ ] Identificação dos picos de busca e dos eventos relacionados
- [ ] Análise das buscas relacionadas

## Principais resultados

_Em andamento. Adicione aqui as conclusões depois de concluir a análise._

<!-- Exemplo:
![Pesquisa por estado](images/pesquisa_por_estado.png)
-->

## Estrutura do projeto

```
projeto-gta6/
├── data/
│   └── pesquisa_por_estado.csv
├── images/
├── projeto_gta6.R
└── README.md
```

## Tecnologias

- R
- gtrendsR
- dplyr
- ggplot2

## Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/devmateeus/projeto-gta6.git
   ```
2. Instale os pacotes (apenas na primeira vez):
   ```r
   install.packages(c("gtrendsR", "dplyr", "ggplot2"))
   ```
3. Abra o projeto no RStudio e execute `projeto_gta6.R`.

Se o Google bloquear a requisição (erro 429), aguarde alguns minutos ou use o CSV já salvo em `data/`.

## Limitações

- O Google Trends mostra interesse relativo, não volume absoluto de buscas.
- Os resultados podem mudar conforme a data em que a consulta é feita.

## Autor

Mateus Dantas, [LinkedIn](www.linkedin.com/in/mateeusdantas)