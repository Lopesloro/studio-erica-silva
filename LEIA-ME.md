# Studio Érica Silva

Landing page do estúdio de beleza da Érica Silva, em Jaguariúna.
Estática pura: HTML, CSS e um bloco de JavaScript. Sem build.

## O que falta antes de virar site definitivo

1. **Preços.** Os três serviços estão com `R$ X`. Procurar por `PRECOS:` no
   `index.html` e trocar pelos valores reais.
2. **Fotos.** As duas imagens em `assets/` são provisórias, geradas por IA e em
   baixa resolução (200x112). Por isso levam `filter: blur()` e `transform:
   scale()` no CSS, que transformam o defeito em campo de luz. Ao colocar as
   fotos reais da Érica, REMOVER o filter e o scale do `.hero img` e do
   `.banner img`.

## Decisões que não são gosto

- **Dialeto Hospitalidade** do padrão da casa: Cormorant Garamond em caixa alta
  com tracking .14em, nenhuma sans no site inteiro, zero sombra, pílula vazada.
- **O conteúdo nasce visível.** O `.reveal` só esconde quando o JavaScript marca
  `<html class="js">`, e uma rede de segurança de 2,5s revela tudo de qualquer
  jeito. Sem isso, qualquer falha do IntersectionObserver deixa a página em
  branco, que é o que já acontece em outras páginas da casa quando abertas pelo
  navegador de dentro do Instagram.
