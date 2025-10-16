# Tainacan Explorer

Explorando alternativas de visualização de obras do Acervo Artístico da UFSM, usando a API do Tainacan.


## Características

- Página minimalista em um único arquivo, puramente em HTML, CSS e JavaScript

  - Pros: controle total, fácil "deploy" (basta fazer upload de um único arquivo), ilustração de tecnologias web de base, etc.
  - Contras: pouco escalável, sem reuso de componentes, manutenção discutível, etc.

- Carrega até 100 imagens do Tainacan (no caso em questão, há menos de 100 itens no Acervo, então vai carregar e mostrar todas)

- Fonte das imagens: JSON com atributos selecionados

  https://tainacan.ufsm.br/acervo-artistico/wp-json/tainacan/v2/collection/2174/items?perpage=100&fetch_only=id,title,document,thumbnail

  (atributo `items.thumbnail` contém diferentes versões da imagem da obra)

## Links

- Acervo Artístico da UFSM: https://www.ufsm.br/pro-reitorias/pre/cca/divisao-de-museus-ufsm/acervo-artistico-ufsm
- API do Tainacan: https://redocly.github.io/redoc/?url=https://github.com/tainacan/tainacan-wiki/raw/master/dev/openapi.json
- Tainacan: https://tainacan.org
- Tainacan Discourse Group (fórum/grupo de usuários): https://tainacan.discourse.group/ 
- Post no fórum de usuários sobre caso de uso da API: https://tainacan.discourse.group/t/harvest-from-other-tainacan/1879/2
