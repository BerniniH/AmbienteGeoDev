# Dados do Satélite SNPP e a Importância das Imagens Noturnas
Os dados utilizados neste script provêm do satélite Suomi National Polar-orbiting Partnership (SNPP), que é uma peça fundamental na observação da Terra. O satélite fornece imagens noturnas através do sensor VIIRS (Visible Infrared Imaging Radiometer Suite), que consegue captar frentes de fogo e outras emissões de calor durante a noite. Essa capacidade é vital para o monitoramento contínuo de incêndios, já que muitos eventos ocorrem ou se intensificam durante a noite, quando a observação tradicional fica limitada.

A captura de imagens noturnas por meio de satélites é baseada na radiação térmica e infravermelha, o que permite a visualização mesmo em ausência de luz solar. No contexto do monitoramento de incêndios, essa capacidade ajuda a identificar focos de calor que podem se transformar em grandes incêndios.

# O que é o GIBS e o Geoserviço Disponibilizado
O Global Imagery Browse Services (GIBS) é um serviço que fornece imagens da Terra em alta resolução, quase em tempo real, com dados de satélites de observação ambiental da NASA. Ele utiliza geoserviços como WMS (Web Map Service) para transmitir essas imagens, o que permite o acesso dinâmico a dados de satélites, mapas de temperatura, anomalias térmicas e muito mais. O GIBS torna esses dados acessíveis em várias plataformas e é essencial para análises em tempo real, como o monitoramento de incêndios florestais.

visite: https://www.earthdata.nasa.gov/eosdis/science-system-description/eosdis-components/gibs

# Estrutura do Código
O código foi estruturado para ser simples e eficiente. Ele utiliza o serviço WMS para obter imagens noturnas e focos de calor noturnos diretamente no mapa interativo. As camadas são controladas por checkboxes que permitem ao usuário habilitar ou desabilitar as visualizações em tempo real. Isso torna o script altamente interativo e flexível para diferentes tipos de análise, como o monitoramento de frentes de fogo noturnas.

Criação do mapa interativo centrado na área desejada.
Adição de camadas WMS (imagens noturnas e focos de calor) do GIBS.
Integração de controles de usuário para habilitar/desabilitar camadas.
Exibição final em uma interface fácil de usar.

# Visualizador de Camadas WMS da NASA

Este script Python usa a biblioteca `ipyleaflet` para exibir um mapa interativo com camadas WMS da NASA. O mapa mostra imagens noturnas e focos de calor noturnos (anomalias térmicas).

## Dependências

* `ipyleaflet`
* `ipywidgets`

## Como usar

1. **Instale as dependências:**

2. **Execute o script:**
   Abra o script em um ambiente Jupyter Notebook ou Google Colab e execute todas as células.

3. **Interaja com o mapa:**
   * Use os controles de zoom e panorâmica para navegar pelo mapa.
   * Use as caixas de seleção para mostrar/ocultar as camadas de imagens noturnas e focos de calor.


## Dados

Os dados WMS são fornecidos pelo GIBS (Global Imagery Browse Services) da NASA.

## Agradecimentos

* NASA GIBS
* ipyleaflet
* ipywidgets

## Autor

Henrique Bernini
