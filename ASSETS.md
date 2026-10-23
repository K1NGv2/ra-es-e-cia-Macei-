# Origem dos materiais

## Materiais fornecidos

- `public/images/logo-original.png`: logo enviada, preservada sem recriação.
- `public/images/instagram-store.webp`: captura do perfil comercial enviada, convertida em WebP. Enquadramentos são feitos via CSS, sem inventar conteúdo ou remover elementos das fotos.
- `public/images/delivery-original.webp`: arte de delivery enviada, convertida em WebP.
- `public/images/address-original.webp`: recorte com endereço, mantido como referência documental.

## Imagens ilustrativas geradas

Ferramenta: **Imagegen nativa**, sem CLI/API externa. Geradas para esta demonstração e otimizadas em WebP. Não são fotografias de clientes ou registros da loja. Não representam marcas ou embalagens reais.

### Hero — `public/images/hero-pets.webp`

Use case: ads-marketing. Asset type: photorealistic website hero image, right column of Brazilian premium pet shop landing page. Primary request: a friendly adult golden retriever sitting beside a small shorthaired brown tabby cat. Both animals looking toward the camera, dog has a happy natural expression, cat calm and curious. Whole bodies and paws visible, close together with the cat on the right slightly in front of the dog. Warm soft studio lighting, exceptionally realistic soft fur texture, high-end commercial pet photography. The pair fills a nearly square image with generous margin around heads and paws. Genuine transparent background, clean cutout, subtle contact shadow only; no props, no lettering, no logos, no collars, no borders. Website behind this image is rich royal blue with a yellow circle. Animals must appear beautiful and natural, not cartoons. Do not create the website itself.

### Produtos

Prefixo comum: “Use case: product-mockup. Asset type: single product photograph for a pet shop demo catalog. Primary request:”.

- `public/images/food-dog.webp`: an upright premium matte royal blue dog food bag, a golden retriever portrait printed on the front, warm yellow lower section, simple fictional Portuguese packaging text "CÃES ADULTOS" and "FRANGO", no brand names. Beside the bag a small pile of dry brown kibble.
- `public/images/food-cat.webp`: an upright premium matte teal green cat food bag, a tabby cat portrait printed on front, pale mint lower section, simple fictional Portuguese packaging text "GATOS ADULTOS" and "SALMÃO", no brand names. Beside the bag a small pile of dry cat kibble.
- `public/images/snacks.webp`: a small upright premium orange and ivory resealable treat pouch with a tiny clear window showing brown dog biscuits, simple fictional Portuguese packaging text "PETISCOS" and "CARINHO EM CADA MORDIDA", no brand names. Three small bone shaped treats in front.
- `public/images/shampoo.webp`: a premium cylindrical light lavender pet shampoo bottle with a royal blue cap, minimal label with a small line drawing of a dog and simple Portuguese text "SHAMPOO PET", subtle lavender flower at the base, no brand.
- `public/images/toy.webp`: one high quality knotted cotton rope dog chew toy with thick woven threads in mustard yellow and rich royal blue, laid diagonally, both knotted ends and soft tassels fully visible.
- `public/images/bowl.webp`: one beautiful deep royal blue ceramic pet feeding bowl, thick rim, a small debossed paw on the front, 3/4 angle showing its cream inner surface, empty bowl.

Direção comum: foto quadrada, objeto inteiro centralizado, fundo branco, textura realista, sombra suave, margens livres; sem marca real, preço, marca d’água ou objetos extras. As três primeiras imagens usam vista frontal em 3/4 e margem de 15%; as demais usam margem de 18%. Os prompts finais completos estão em `prompts-imagens.json`.

## Referência visual

[Petocare](https://petocare.framer.website/), fornecida pelo cliente: referência de espaçamento, fotografia e ritmo editorial. A implementação é própria, com identidade Rações & Cia e foco em venda de rações. Nenhum código ou imagem comercial do template foi reutilizado.


Atualização solicitada: as fotos reais das seções Sobre e galeria foram substituídas pelas imagens fictícias já geradas (pets e produtos), com legendas ilustrativas. A arte de delivery foi substituída pela quarta imagem enviada, sem a interface do Instagram. Compilação TypeScript/Vite concluída após a troca.
