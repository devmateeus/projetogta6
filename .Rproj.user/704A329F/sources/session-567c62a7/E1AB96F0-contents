# Pacotes -----------------------------------------------------------------
# Rode as linhas abaixo UMA vez só e depois deixe comentadas:
# install.packages("gtrendsR")
# install.packages("ggplot2")
# install.packages("dplyr")

library(gtrendsR)
library(ggplot2)
library(dplyr)

# Importação dos dados ----------------------------------------------------
res <- gtrends(keyword = "GTA 6", geo = "BR", time = "today+5-y")

pesquisa_por_regiao <- res$interest_by_region %>%
  select(location, hits) %>%
  rename(estado = location, qntvezes = hits)

print(pesquisa_por_regiao)

# Exportação (para não depender do Google toda vez) -----------------------
dir.create("data", showWarnings = FALSE)
write.csv(pesquisa_por_regiao, "data/pesquisa_por_estado.csv", row.names = FALSE)

# Visualização ------------------------------------------------------------
ggplot(pesquisa_por_regiao, aes(x = reorder(estado, qntvezes), y = qntvezes)) +
  geom_col(fill = "steelblue") +
  coord_flip() +
  theme_minimal() +
  labs(title = "Pesquisa por estado: GTA 6",
       x = NULL,
       y = "Interesse relativo (0 a 100)")
