# AGENTS.md: instruções gerais para a IA

## Objetivo
Gerar um site de portfólio pessoal em um único arquivo `index.html` (CSS e JS inline), pronto para abrir no navegador, sem build e sem servidor.

## Fluxo obrigatório (nesta ordem)
1. Antes de codificar, proponha a direção visual: 2 a 3 frases por referência listada em `referencias.md`, explicando por que ela combina com o perfil de `identidade.md`.
2. Só depois gere o código.
3. Ao final da resposta, inclua a seção "Decisões de design", relacionando paleta, tipografia, layout e interações a uma intenção.

## Stack
- HTML, CSS e JavaScript puros. Sem frameworks e sem bibliotecas, exceto Google Fonts e, se necessário, um CDN de ícones.
- Comente apenas os trechos não óbvios.
- Nomes de código em inglês. Textos visíveis ao usuário em português do Brasil.

## Regras de layout (inegociáveis)
- O site não tem scroll vertical. A navegação entre seções é feita pelo menu em roda.
- Dentro de cada seção, a rolagem é somente horizontal. Apenas o conteúdo da seção se move; o menu e o cabeçalho ficam fixos.
- Elementos próximos às bordas da seção são menores e crescem conforme se aproximam do centro da tela.
- NENHUM card. Nada de caixas genéricas com sombra, borda arredondada e fundo branco ou escuro, em nenhuma seção.
- Evite o visual de template padrão: sem hero com gradiente roxo, sem grade de ícones iguais, sem botões pill genéricos.

## Responsividade
- O site deve funcionar bem no celular e no computador.
- No celular, a rolagem horizontal responde ao toque (swipe).
- O menu hambúrguer é funcional no celular.

## Qualidade
- Nenhum erro no console.
- Respeite `prefers-reduced-motion` nas animações.
- Acessibilidade: navegação por teclado (setas esquerda/direita para a rolagem horizontal), contraste adequado e `alt` em todas as imagens.
- Se algum dado estiver faltando, use um placeholder visível e liste os placeholders no final da resposta.
