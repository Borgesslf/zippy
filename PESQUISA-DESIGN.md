# Dulce — pesquisa de referências de e-commerce e responsividade

Pesquisa realizada em **29 de outubro de 2026** para a primeira loja PWA Dulce.
**Método:** inspeção de páginas públicas e seus elementos acessíveis (categorias, textos, listagens, filtros, ordenação, chamadas de compra e retirada). Padrões sintetizados e aplicados em layout original. Não reproduzimos HTML, CSS, imagens proprietárias, logotipos ou scripts das lojas pesquisadas. A inspeção textual não permite confirmar os breakpoints exatos de cada site; as faixas abaixo são **decisões próprias de projeto**, não extração do CSS das referências.

## As 10 lojas

| Referência | Página analisada | Padrões encontrados | O que faz sentido para Dulce |
| --- | --- | --- | --- |
| Sephora | https://www.sephora.com.br/ | Categorias nítidas (maquiagem, perfume, skincare, cabelos), destaques editoriais | Menu simples, entrada por categorias e hero marcante |
| Natura | https://www.natura.com.br/c/cabelos-produtos | Navegação por linha capilar e comunicação mais lifestyle | Catálogo com tom acolhedor; cuidado com o tipo de produto |
| O Boticário | https://www.boticario.com.br/cabelos | Filtros por necessidade capilar, card com preço e ação de sacola, comunicação de clique e retire | Categorias fáceis e retirada como serviço principal |
| Eudora | https://www.eudora.com.br/site-todo | Catálogo organizado, preço em destaque e cards escaneáveis | Hierarquia do card: marca, título, preço, adicionar |
| Beleza na Web | https://www.belezanaweb.com.br/cabelos/ | Taxonomia por tipo de cabelo/necessidade, descrição resumida, filtros | Busca e navegação que não exigem conhecer marca |
| Sallve | https://www.sallve.com.br/collections/loja | Grade direta, ordenação e destaque para favoritos | Vitrine leve, CTA visível, filtros compactos |
| Creamy | https://www.creamy.com.br/produtos | Filtro por benefícios, contagem de itens, opções de ordenação | Contador de resultados e ordenação funcional |
| Granado/Phebo | https://phebo.granado.com.br/sabonetes | Identidade coesa, produtos e preços fáceis de conferir, kits | Visual editorial sofisticado e cards limpos |
| Braé | https://www.brae.com.br/produtos?order=OrderByTopSaleDESC | Destaque em haircare; ordenação, preço, descrição breve e botão de comprar | Cabelos como categoria protagonista |
| Época Cosméticos | https://prd.epocacosmeticos.com.br/colecao/330 | Filtros, lista de produtos, preço e ação de compra bem visível | Foco em achar/selecionar sem etapas desnecessárias |

## Decisões de design aplicadas

- Identidade original Dulce: rosa iogurte mais fechado **#BF7891**, ameixa **#4B313D**, branco-creme **#FBF8F6**.
- Hero editorial com imagem de autocuidado **ilustrativa** (Pexels), e texto legível separado da imagem.
- Quatro cartões de categoria com foco em cabelos, perfumaria, corpo & banho e kits/presentes; filtro rápido ao clicar.
- Faixa de marcas **somente como prévia demonstrativa**, sem indicar estoque real.
- Cards com marca, produto, breve identificação, preço e ação explícita “Adicionar à sacola”.
- Busca por nome e marca, filtros por categoria, ordenação por menor/maior preço e nome.
- Sacola persistida localmente com contagem nos ícones do desktop e celular.
- Pedido por formulário e preferência de retirada. **Não é uma reserva garantida**. O número oficial do salão ainda precisa ser configurado.
- Menu inferior de fácil alcance em telas pequenas; barra de filtros rolável na horizontal.

## Responsividade projetada

| Largura do dispositivo | Apresentação |
| --- | --- |
| Acima de 1140 px | Menu completo, hero em duas colunas, quatro cards por linha |
| 781 a 1140 px | Tipografia e espaços reduzidos sem perder o grid |
| 421 a 780 px | Hero empilhado, categorias e vitrine em duas colunas, barra inferior fixa |
| 351 a 420 px | Produtos mais compactos, busca e ordenação lado a lado |
| Até 350 px | Espaçamento e arte reduzidos para telas estreitas |

**Acessibilidade e performance:** botões com rótulos, contraste textual, alt na imagem editorial, foco visível, prefer-reduced-motion, CSS sem biblioteca, suporte offline básico da PWA (cache do shell). Dependência externa de fontes e foto pode não aparecer offline; CSS mantém cores de fundo como fallback.

## Validação feita

- JavaScript compilou em verificação sintática.
- Chaves do CSS balanceadas.
- HTML com uma abertura e fechamento de `main`.
- IDs únicos, e todas as âncoras internas apontam para elementos presentes.
- Presença de eventos de busca, ordenação, filtros e navegação móvel.

**Limite:** ainda não houve teste visual por navegador real em todos os tamanhos e dispositivos nem teste de envio ao número oficial; verificar após a publicação, principalmente iPhone/Safari e Android/Chrome.

## Pendente para publicar como loja real

1. Receber logo, número de WhatsApp oficial, endereço, horários de atendimento.
2. Substituir os **oito itens fictícios**, descrições, preços e ilustrações por catálogo, fotos e estoque confirmados.
3. Definir e configurar hospedagem HTTPS e validar PWA no iOS e Android.
4. Opcional: criar gestão de produtos/pedidos com banco de dados para uso diário.

Crédito da foto editorial demonstrativa: [Pexels](https://www.pexels.com/photo/beauty-products-on-pink-background-6187609/).
