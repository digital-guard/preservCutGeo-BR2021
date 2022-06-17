# Belo Horizonte

Recorte dos dados originais doados com lincença aberta para uso público.

Cada evento de doação relativo a um doador específico gera uma entrada de dados, identificada pelo respectivo pacote. Por exemplo doações da prefeitura de Belo Horizonte a partir de 2020, como `pk0008.01`.

Na pasta [_pk0008.01/geoaddress](_pk0008.01/geoaddress) encontram-se todos os pontos de localização geográfica com respectivos dados de endereço.
Por exemplo a <br/>*"RUA DOS INDEPENDENTES, 26"* encontra-se no arquivo [`pts_7h2wjv.geojson`](_pk0008.01/geoaddress/pts_7h2wjv.geojson) da pasta. <br/>O nome do arquivo pode ser lido da seguinte forma:
* prefixo `pts_` e extensão `.geojson` indica que são pontos formatados em GeoJSON.
* `7h2wjv` é o "prefixo Geohash" de todos os pontos contidos no arquivo.

![](../../../../docs/assets/ScreenshotBH-pts1.png)

Para saber em qual  "prefixo Geohash" se encontra o ponto que deseja, veja as instruções abaixo e use o <br/>aplicativo de Geohash https://www.movable-type.co.uk/scripts/geohash.html

Para rastrear ou fazer *download* os dados primários doados pela Prefeitura de Belo Horizonte, ver [listagem de dados primários da Digital-Guard](http://docs.digital-guard.org/preserv/pt/list-primaryData-byJurisdic/) ou, conforme configurado em [BR-MG/BeloHorizonte/_pk0008.01](https://github.com/digital-guard/preserv-BR/blob/main/data/MG/BeloHorizonte/_pk0008.01/make_conf.yaml): *download* dos  arquivos originais (preservados por 20 anos) de todos os [pontos em *shapefile* (`1ce29a5`)](http://dl.digital-guard.org/1ce29a555565be5f540ab0c6f93ac55797c368293e0a6bfb479a645a5a23f542.zip).
