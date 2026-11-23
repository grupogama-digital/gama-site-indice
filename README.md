# gama-site-indice

Índice dos grupos de produtos (Linhas com 2 ou mais itens) do site da Gama, usado pelo script
"capa dos cards de grupo" da busca para trocar foto, nome, código e link na hora.

- Só tem dado que o site já mostra sem login: código, nome, link, foto, grade, embalagem, estoque, EAN e código do fabricante.
- **Nunca** colocar aqui preço, custo, cliente ou senha.
- Um arquivo por data: `busca/indice-grupos-AAAA-MM-DD.json`. O script aponta para um arquivo fixo pelo jsDelivr:
  `https://cdn.jsdelivr.net/gh/grupogama-digital/gama-site-indice@main/busca/indice-grupos-AAAA-MM-DD.json`
- Arquivo novo = nome novo + trocar a `URL_INDICE` no head_js (assim não pega cópia velha do cache).

Formato de cada item: `[grupo, nome, slug, foto (1 = <codigo>_1.jpg), unidade, estoque, [valores da grade], ean, sku, marca, fornecedor, id_embalagem, pai]`.
