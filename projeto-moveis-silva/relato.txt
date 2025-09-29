No nosso código havia alguns pequenos erros que dificultavam a organização como um todo do código.
Melhoramos a organização.
Para melhor acessibilidade, mudamos todas as unidades em "px" para "rem". Isso permite que o site se adapte 
ao tamanho de fonte que o usuário configurou no navegador.

Corrigimos o erro que tinha no menu. O problema estava na: 
Ex:
--- <li><a href="servicos.html" aria-current="page">Início</a></li> ---- 

O código [ aria-current="page" ] estava sempre no link da página de início. Por isso o menu destacado era sempre o botão
"Início". Em cada página, colocamos o código aria-current="page" no hfref. Com isso, o menu da página que está aberta
voltou a ficar em destaque, corrigindo o erro em questão.

Foi testado no Devtools e está funcionando perfeitamente em todas as telas. O site está se ajustando em colunas ou 
listas (quando a página é muito pequena), o que mostra que o flexbox, grid e media queries estão funcionando.