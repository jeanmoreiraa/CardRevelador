## Explicação dos Arquivos do Card Revelador
Vou explicar o que cada um dos arquivos faz neste projeto de Card Revelador, que é basicamente um cartão interativo que vira quando clicado:
## 1. cardrevelador.html
Este é o arquivo HTML principal que estrutura a página. Ele:

Define um documento HTML básico com configurações iniciais (DOCTYPE, linguagem, meta tags)
Importa o arquivo CSS (style.css) para estilização
Define o título da página como "Card Revelador"
Cria uma estrutura de div com classe "card" que contém:

Uma div "card-inner" com duas faces:

"card-front" com o texto "Curtitu o post?"
"card-back" com o texto "Então curta, comente e compartilhe <3"




Importa o arquivo JavaScript (script.js) para adicionar interatividade

## 2. script.js
Este é o arquivo de JavaScript que adiciona a funcionalidade interativa. Ele:

Seleciona o elemento com classe "card" na página
Adiciona um event listener para detectar cliques no cartão
Quando o cartão é clicado, ele adiciona ou remove a classe "flip", o que faz o cartão virar graças ao CSS

## 3. style.css
Este arquivo CSS define toda a estilização do cartão e da página:

Configura o corpo da página com fundo escuro (#0a0a0a)
Centraliza o conteúdo na tela
Define o tamanho do cartão (280px x 350px)
Implementa o efeito 3D de virar o cartão usando:

perspective para criar profundidade 3D
transform-style: preserve-3d para manter o efeito 3D
transition para animar a mudança suavemente
backface-visibility: hidden para esconder o verso do cartão


Define estilos diferentes para a frente (fundo branco, texto preto) e verso (fundo cinza escuro, texto branco)
Usa transform: rotateY(180deg) para virar o cartão quando a classe "flip" é adicionada

Juntos, estes três arquivos criam um cartão interativo que vira quando clicado, revelando uma mensagem diferente no verso.
