# Rações & Cia Maceió

Aplicação comercial em React, TypeScript, Vite e Tailwind CSS, com componentes locais no padrão shadcn/ui sobre Radix, ícones Lucide e animações Motion. O foco é a venda de rações e a consulta comercial pelo WhatsApp.

## Apresentar sem instalação

Abra o arquivo **Racoes-e-Cia-Demonstracao.html**, entregue ao lado desta pasta, em um navegador moderno. Todo o código, as fontes e as imagens estão incorporados. Busca, filtros, ordenação, detalhes de produtos, galeria e FAQ funcionam sem servidor. É preciso internet para visitar WhatsApp e Instagram.

## Executar o projeto

Requisitos: Node.js 22.12+ e pnpm. As dependências exatas estão em `pnpm-lock.yaml`.

```sh
pnpm install
pnpm dev
```

Abra a URL local informada pelo Vite. Para verificar e preparar a versão de distribuição:

```sh
pnpm test
pnpm build
pnpm preview
node scripts/standalone.mjs
```

`dist/` contém a versão estática compilada. `scripts/standalone.mjs` gera novamente o HTML independente a partir de `dist/`.

## Atualizar informações

**`src/data/site.ts`** é a fonte central de telefone, Instagram, horários, endereço, categorias, produtos, ofertas, avaliações e FAQ. As imagens ficam em `public/images/`.

- Produtos: use um ID exclusivo, a categoria correspondente e uma imagem. `price` e `brand` são opcionais. Marque `demo: false` somente depois de cadastrar dados reais e autorizados. Confirme os textos do FAQ e os avisos gerais ao trocar todo o catálogo por dados reais.
- Ofertas: a lista começa vazia. Apenas entradas com `verified: true` e validade não expirada são exibidas. Não adicione preços anteriores sem comprovação.
- Avaliações: a seção permanece oculta enquanto não houver entradas autorizadas com `approved: true`. Nome, fonte e link devem ser reais.
- Endereço: o recorte enviado indica Rua Santo Antônio, nº 34, Ponta Grossa. Está marcado `verified: false`, visivelmente pendente de confirmação, e não foi incluído como endereço completo nos dados estruturados. Não há mapa.
- Retirada, cobertura do delivery, taxas e prazos não foram presumidos. O fluxo orienta combinar diretamente com a equipe.
- WhatsApp: `src/lib/catalog.ts` centraliza as mensagens, a codificação dos links e a lógica de busca. Mensagens de produtos fictícios explicitam que o visitante viu um exemplo e deseja consultar opções reais.

## Estrutura

```text
src/
  data/site.ts              Configuração e catálogo
  lib/catalog.ts            Busca, ordenação e WhatsApp
  components/ui/            Button, Dialog e Accordion
  components/Navbar.tsx     Cabeçalho e menu mobile
  components/HeroSection.tsx
  components/Catalog.tsx    Categorias, busca, filtros e produtos
  components/Sections.tsx   Ofertas, delivery, sobre, galeria, FAQ e contato
  components/Footer.tsx
  App.tsx
  styles.css
tests/catalog.test.ts
public/images/
```

## Materiais e demonstração

Logo original preservada. A galeria usa enquadramentos via CSS da captura de Instagram fornecida, com atribuição e indicação de que publicações anteriores não representam ofertas vigentes. O banner de delivery é um material fornecido da marca. Não foram inventadas fotografias da loja.

Animais do hero e imagens de produtos foram gerados com a ferramenta nativa Imagegen. São composições ilustrativas, sem marcas reais. Todos os preços, pesos e produtos da vitrine são fictícios, conforme solicitado. Consulte `ASSETS.md` para os prompts e a origem dos arquivos.

A referência Petocare foi usada apenas para ritmo editorial, espaços e hierarquia visual. Nenhum código Framer, depoimento, serviço de banho/tosa ou dado comercial da referência foi incorporado.

## Publicação

**Nenhuma publicação ou implantação foi feita.** Esta entrega é local. A demonstração usa `noindex, nofollow` e não possui pagamento online nem envio automático de mensagens.

Antes de uma publicação autorizada, confirme catálogo, endereço, informações comerciais e direitos de uso das fotos. Configure domínio, URLs absolutas de Open Graph, canonical, política de privacidade correspondente à operação real e indexação. O Schema.org usa apenas nome, telefone, cidade, Instagram e horários fornecidos, sem avaliações ou ofertas fictícias.

## Verificação

Build TypeScript/Vite, testes de busca e mensagens e revisão do fluxo no navegador. Veja `VERIFICACAO.md` para os resultados e limites.


Atualização solicitada: as fotos reais das seções Sobre e galeria foram substituídas pelas imagens fictícias já geradas (pets e produtos), com legendas ilustrativas. A arte de delivery foi substituída pela quarta imagem enviada, sem a interface do Instagram. Compilação TypeScript/Vite concluída após a troca.
