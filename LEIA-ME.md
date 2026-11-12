# Art & Fé — site estático

Site em HTML, CSS e JavaScript, sem APIs, bibliotecas externas ou serviços pagos. Para visualizar, abra `index.html` ou execute `python -m http.server 4173` nesta pasta e acesse http://localhost:4173.

## Catálogo e páginas de produto

- Na página principal, cada peça aparece com uma foto de capa. As fotos adicionais ficam somente na página individual, aberta ao clicar na imagem.
- Clique na foto de um crucifixo para abrir sua página de detalhes em outra aba. As miniaturas selecionam outras fotos reais da peça.
- O catálogo e as páginas de produto têm botões para Mercado Livre e Shopee. Até inserir os endereços dos anúncios, os botões levam a buscas de crucifixos artesanais nessas plataformas.
- Para direcionar ao anúncio correto, preencha `mercadoLivre` e `shopee` do item correspondente em `products.js`.
- Edite o mesmo arquivo para definir título, descrição, dimensões e preço reais. Esses dados seguem como “sob consulta” até serem fornecidos.
- As fotografias da galeria estão em `assets/products/`; outras fotos originais foram preservadas em `assets/originais/`.
- O WhatsApp está configurado com o número e a mensagem informados. A compra e o pagamento não são processados pelo site.

## Logo

A logo original não foi localizada nos arquivos acessíveis. Quando a disponibilizar, coloque-a como `assets/logo.svg` ou `assets/logo.png` e atualize o cabeçalho/rodapé de `index.html` e `produto.html`.

## Editor visual

Abra `editor.html` no site servido localmente para alterar nome, descrição, dimensões, valor, fotos e links de cada peça. Salvar neste navegador atualiza a prévia no mesmo navegador. Para levar as alterações ao site publicado, baixe `products.js` pelo editor e substitua o arquivo correspondente antes de publicar.

## Abrir o editor

Com o servidor local ligado, abra http://localhost:4173/editor.html. Ele não aparece na navegação da loja; as alterações são locais a este navegador até baixar o arquivo atualizado.


O editor tem duas abas: **Produtos** (incluindo medidas, materiais e acabamento) e **Página principal** (textos, fotos da abertura e da seção artesanal, além das fotos de capa editadas por produto). Para salvar uma cópia para hospedagem, baixe `products.js` e `content.js` e substitua os arquivos correspondentes.


No editor, use **Escolher foto de capa do computador** para adicionar a imagem que aparece na página principal. Use **Adicionar fotos ao detalhe do produto** para a galeria. As imagens são reduzidas no próprio navegador e incorporadas em `products.js`/`content.js` quando baixados; não precisam de serviço externo.

A seleção de uma foto mostra o nome do arquivo e salva a alteração local automaticamente. Recarregue a página principal para conferir a nova capa.

Na página inicial, clique em **Editar esta vitrine** para abrir os campos de nome, valor e foto diretamente em cada cartão. As alterações são salvas no navegador.

Cada produto tem campos separados para a foto da página inicial (`homepageImage`) e a foto principal da página de detalhes (`image`). O controle **Foto da página inicial** altera apenas o cartão da vitrine.
