# BH Escolas — Layout para GitHub

Template de interface para um localizador de escolas de Belo Horizonte.

## Como usar

1. Substitua `data/escolas.geojson` pelos seus dados.
2. Mantenha as geometrias como `Point` em WGS84 (`EPSG:4326`) e coordenadas no formato `[longitude, latitude]`.
3. Mantenha ou adapte os campos usados em `src/app.js`:
   - `nome`
   - `endereco`
   - `bairro`
   - `regional`
   - `rede`
   - `etapa`
4. Publique no GitHub Pages.

## O que o layout faz

- Busca endereço em Belo Horizonte.
- Mostra a localização no mapa.
- Calcula tempo estimado até as escolas próximas.
- Permite alternar entre carro e caminhada.
- Filtra por rede e etapa.
- Desenha a rota da residência até a escola escolhida.

## Atenção

O cálculo de tempo é estimado pela rede viária. O exemplo usa Nominatim e OSRM públicos e não representa trânsito em tempo real. Para uma aplicação municipal de produção, utilize infraestrutura/provedor de geocodificação e roteamento compatível com a escala de acesso e as políticas dos serviços.
