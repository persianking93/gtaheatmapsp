# Mapa de Calor - Roubos de Veículos em São Paulo, capital

Projeto com foco em análise e interpretação de dados espaciais georreferencidos disponíveis ao público.

## Ideia Principal

Isolar os dados disponíveis sobre furtos e roubos de veículos na Secretaria de Segurança Pública do Estado de São Paulo (SSP-SP) e, com isso, gerar áreas para clusterização dos dados discretos (pontos) assim como interpolar estes pontos para a criação de um mapa de calor; este mapa de calor indica quais áreas onde há maior e menor incidência destas ocorrências.

## Metodologia

O projeto foi realizado em três etapas distintas:
  *Aquisição dos dados
  *Tratamento e organização
  *Elaboração do modelo e interpretação

### Aquisição dos dados

Os dados foram adquiridos em formato .xmlx à partir da base de dados da SSP-SP, com seu API que gera uma planilha contendo as informações das ocorrências

### Tratamento e organização

Utilizando-se a biblioteca GeoPandas, foi adicionado aos dados uma nova coluna de formato espacial (neste caso, pontos) para a geração do elementos discretos no mapa.

### Elaboração do modelo e interpretação

O modelo foi elaborado usando a biblioteca Folium, que permite a sobrepor os dados elaborados sobre um mapa interativo de diversas fontes (desde Google Maps até ESRI World Map). A interpretação procurou levar em conta as características geográficas e de ocupação urbana do município para explicar a densidade de ocorrências em cada região.
