> A cutout of the [Preserv-BR](http://git.digital-guard.org/preserv-BR) data,  with a geographic profile, collecting sources since 2021.

Recorte dos dados de [Preserv-BR](http://git.digital-guard.org/preserv-BR), com perfil geográfico, coletando fontes datadas de 2021 (2019?) em diante. Neste repositório, "PreservCutGeo-BR2021", os recortes são mantidos por pacote doado e por *layer*. Os pacotes são relativos a um doador (ex. prefeitura) e os *layers* conforme [convenções do projeto Preserv](http://git.digital-guard.org/preserv/blob/main/docs/pt/ftypes.md#com-geometria).

Para maiores detalhes consultar a documentação:

* [**Documentação geral de todos os repositórios PreservCutGeo**](https://github.com/digital-guard/preserv/blob/main/docs/pt/man-diversos.md#load-arquivos-do-cutgeo-a-partir-de-um-diret%C3%B3rio) (parcial).
* [**Documentação das especificidades deste repositório**](docs/README.md) (em construção).
* Instruções para a recuperação em massa dos arquivos GeoJSON desejados deste git.

## Lembretes para quem atualiza

1. Usar sempre os *targets make* de Preserv, conforme instruções. Não realizar procedimentos manuais.
2. Realizar a publicação em duas etapas, primeiro em *branch* apartado depois homologação seguida de publicação no *branch master*.
3. A Wiki e as *issues* deste repositório não devem ser habilitadas, usar o Preserv-BR para discutir questões de dados específicos BR, e o Preserv para bugs e discussões relativas à metodologia, makefile ou algoritmos.

## Lembretes para o usuário

### Organização das pastas e arquivos

A pasta [/data](data) é a pasta geral dos dados. Exemplo de Belo Horizonte, pacote doado `pk0008.01`:<br/> na pasta [/data/MG/BeloHorizonte/_pk0008.01/geoaddress](data/MG/BeloHorizonte/_pk0008.01/geoaddress) encontram-se todos os pontos de localização geográfica com respectivos dados de endeço. Suponhamos a *"RUA DOS INDEPENDENTES, 26"* que encontra-se no arquivo [**`pts_7h2wjv.geojson`**](data/MG/BeloHorizonte/_pk0008.01/geoaddress/pts_7h2wjv.geojson) da pasta *geoaddress*. <br/>O nome do arquivo pode ser lido da seguinte forma:
* prefixo `pts_` e extensão `.geojson` indica que são pontos formatados em GeoJSON.
* `7h2wjv` é o "prefixo Geohash" de todos os pontos contidos no arquivo.

Para navegar pelos dados de forma mais amigável usar a páginas no site, atualmente em construção [addressforall.org/teste2](http://addressforall.org/teste2).

### Downloads

Para rastrear ou fazer *download* os dados primários doados pela Prefeitura de Belo Horizonte, ver [listagem de dados primários da Digital-Guard](http://docs.digital-guard.org/preserv/pt/list-primaryData-byJurisdic/) ou, conforme configurado em [BR-MG/BeloHorizonte/_pk0008.01](https://github.com/digital-guard/preserv-BR/blob/main/data/MG/BeloHorizonte/_pk0008.01/make_conf.yaml): *download* dos  arquivos originais (preservados por 20 anos) de todos os [pontos em *shapefile* (`1ce29a5`)](http://dl.digital-guard.org/1ce29a555565be5f540ab0c6f93ac55797c368293e0a6bfb479a645a5a23f542.zip).

### Colaboração e contato sobre falhas

Usar issues do Preserv-BR.

-----

## Aviso legal
Os dados deste repositórios **não foram consolidados e são todos *"tal qual original cedido pelo doador"***. Alguns *pacotes doados* podem se mostrar complementares e a grande maioria pode se mostrar redundante, repetindo grandes porções de dados. A confiabilidade de cada pacote será aferida posteriormente, bem como a consolidação: a finalidade maior deste repositório é permitir que o público consulte os dados originais e faça uso dos mesmos conforme sua preferência.

A **licença de cada pacote** (*package* numerado) é aquela ofertada pelo doador, e permanece a mesma para os dados do presente recorte. Por isso não existe uma licença uniforme para todos os dados do presente repositório, deve-se consultar a cada pasta de `_pkXXX`.
