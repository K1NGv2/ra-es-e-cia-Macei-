# Verificação da demonstração

Revisão realizada em 23/10/2026. Fluxo verificado: navegar pela vitrine → buscar/filtrar rações → abrir detalhes → preparar consulta no WhatsApp.

## Resultado

- Compilação TypeScript em modo estrito e build Vite concluídos.
- Cinco testes automatizados aprovados: busca sem acentos, combinação de busca e categoria, ordenação sem alterar os dados, mensagens demonstrativas e codificação de URLs.
- Menu mobile abre e fecha; selecionar “Produtos” fecha o menu e navega à seção.
- Busca por “racao caes” retorna as duas rações para cães. Termo sem correspondência exibe estado vazio e recuperação funcional.
- Filtro “Para gatos” retorna dois produtos. Ordenação Z–A coloca “Ração para gatos castrados” antes de “Ração para gatos adultos”.
- Selecionar uma categoria pela vitrine limpa a pesquisa anterior e mostra os itens correspondentes.
- Detalhes de produto abrem em diálogo acessível e fecham com Escape.
- Galeria abre, navega pelas setas do teclado e fecha com Escape. Enquadramentos de fotos revisados visualmente.
- FAQ abre e apresenta a explicação de preços fictícios.
- Todas as âncoras internas encontram suas seções. Os 19 links de WhatsApp da página principal usam o número comercial correto e mensagens codificadas.
- Nenhuma mensagem foi enviada e nenhum pedido foi realizado durante os testes.
- Navegador sem erros ou avisos de console observados no fluxo.
- Cores de textos secundários ajustadas para contraste de pelo menos 4,5:1 nos pares revisados.

## Responsividade

| Largura da janela | Colunas de produtos | Menu | Rolagem horizontal |
|---|---:|---|---|
| 360 px | 2 | Mobile | Não |
| 390 px | 2 | Mobile | Não |
| 430 px | 2 | Mobile | Não |
| 768 px | 3 | Mobile | Não |
| 1024 px | 4 | Desktop | Não |
| 1440 px | 4 | Desktop | Não |
| 1920 px | 4 | Desktop | Não |

O scrollbar do navegador consome 15 px da área útil. A verificação compara `scrollWidth` com `clientWidth`, sem ocultar overflow horizontal da página.

## Desempenho e limites

- Fontes locais, imagens de produtos em WebP, carregamento tardio abaixo do hero, imagem principal priorizada e animações respeitando `prefers-reduced-motion`.
- CSS compilado próximo de 46 kB e JavaScript próximo de 476 kB antes de gzip; JS comprimido próximo de 153 kB. A captura longa de Instagram fornecida tem aproximadamente 3,5 MB e só é requisitada abaixo da vitrine. Fotografias originais individuais poderão reduzir esse custo numa versão de produção.
- A verificação responsiva foi feita no navegador integrado, sem emulação de hardware ou rede móvel. Não foi executada auditoria Lighthouse nem medição de Core Web Vitals em produção.
- O HTML independente incorpora código, imagens e fontes, e foi conferido estruturalmente. A política do navegador integrado bloqueia `file://`; por isso, seu funcionamento por abertura direta deve ser conferido no navegador do apresentador. A aplicação compilada equivalente foi testada via HTTP local.
- Endereço, estoque, preços reais, taxas/prazos do delivery e retirada continuam sujeitos à confirmação comercial. Sem ofertas nem avaliações fictícias.
- Nenhum site foi publicado.
