# Look Me Semijoias

Site estático em HTML, CSS e JavaScript, pronto para GitHub Pages. Não precisa de Node.js, instalação de dependências nem etapa de build.

## Publicação no GitHub Pages

1. Descompacte este ZIP.
2. Crie um repositório no GitHub, por exemplo `look-me-semijoias`.
3. Envie **o conteúdo da pasta**, deixando `index.html`, `style.css`, `app.js` e `assets/` na raiz do repositório. Não envie apenas o ZIP nem coloque uma pasta extra acima do `index.html`.
4. No repositório, acesse **Settings → Pages**.
5. Em **Build and deployment**, selecione **Deploy from a branch**.
6. Selecione a branch que contém os arquivos (normalmente `main`) e a pasta **/ (root)**. Salve.
7. Aguarde a publicação e abra o endereço exibido pelo GitHub.

Os caminhos dos arquivos são relativos e funcionam também em uma URL como `https://SEU-USUARIO.github.io/look-me-semijoias/`.

## Arquivos

- `index.html`: conteúdo e estrutura da loja.
- `style.css`: identidade visual e layout responsivo.
- `app.js`: catálogo, filtros, busca e sacola.
- `assets/look-me.jpg`: foto enviada para a marca.
- `.nojekyll`: mantém a publicação como arquivos estáticos.

## Personalização

Edite a lista `products` no início de `app.js` para trocar os nomes e categorias das peças. A vitrine atual usa ilustrações em SVG e informa explicitamente que se trata de uma prévia. A imagem principal está em `assets/look-me.jpg`.

As fontes são carregadas do Google Fonts; fontes alternativas são usadas quando o serviço não estiver disponível.

## Funcionalidades

- Layout adaptado a celulares e computadores.
- Categorias e busca por nome.
- Sacola com inclusão, exclusão e ajuste de quantidade.
- Persistência da sacola no navegador, quando o armazenamento local estiver disponível.

## Pagamento e operação comercial

Esta versão é uma **prévia da loja**. Os produtos são ilustrativos, não há preços cadastrados, controle de estoque, cálculo de frete, registro de pedidos nem cobrança. O botão de pagamento mostra uma mensagem explicativa e não coleta dados financeiros.

Para receber compras reais, cadastre o catálogo com preços e estoque, defina frete e políticas da loja e integre um provedor de pagamento. Chaves secretas nunca devem ser colocadas neste repositório ou no JavaScript público. Uma integração que usa credenciais privadas precisa de um backend ou serviço seguro externo; o GitHub Pages serve apenas os arquivos estáticos.

## Prévia local

Abra `index.html` no navegador ou execute, dentro desta pasta:

```bash
python3 -m http.server 8000
```

Depois abra `http://localhost:8000`.
