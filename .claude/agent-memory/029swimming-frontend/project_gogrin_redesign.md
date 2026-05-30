---
name: Gogrin Redesign — Reestruturação Visual 029Swimming
description: Reestruturação visual completa das seções abaixo do hero com estilo Gogrin em 2026-05-27
type: project
---

Reestruturação visual completa das seções abaixo do hero foi realizada em 2026-05-27.

**Why:** O site precisava de mais profundidade visual, hierarquia tipográfica clara, cards modernos com espaçamentos generosos e consistência de layout inspirada no estilo Gogrin (tema WordPress de surf/mergulho).

**How to apply:** Em futuras sessões, o bloco CSS principal do redesign está no `<style id="gogrin-redesign">` logo antes do `<!-- BOAS-VINDAS -->`. Novas alterações devem seguir os mesmos padrões de tokens definidos ali (--sp-gogrin, --card-radius, --card-pad).

## O que foi alterado

### CSS (bloco `<style id="gogrin-redesign">`)
- Token `--sp-gogrin: clamp(5rem, 8vw, 7rem)` — padding vertical generoso
- Token `--card-radius: 20px` — border-radius padrão dos cards
- Eyebrow `.s-eye`: letter-spacing .22em, linha decorativa gradiente ocean→glow de 28px
- Títulos `.s-h2`: clamp(1.6rem, 3.5vw, 2.4rem), font-weight 900, letter-spacing -0.01em
- Lead `.s-lead`: font-size 1rem, line-height 1.85

### Seções modificadas (HTML + CSS)
- **#boas-vindas**: foto com moldura assimétrica 24px/8px, badge maior (2rem), linha decorativa após a foto, texto com line-height 1.85, destaque com border-left + background sutil
- **Brand strip**: linhas decorativas topo e base, font-size aumentado
- **#sobre**: padding e espaçamentos do bloco qs-* refinados
- **#sobre-narrativo**: moldura de foto com cantos 28px/8px, linha decorativa azul lateral esquerda, background bg3 (era bg)
- **#experiencia**: cards com `::before` — linha colorida ocean→glow sempre visível no topo, ícones 64px, padding 2.2rem 1.8rem
- **#diferenciais**: mesmo padrão de linha no topo dos cards, ícones 64px, padding 2.4rem 2rem, gap 1.8rem
- **#depoimentos**: linha colorida no topo, avatar 44px com border, separador interno, CTA ao final da seção
- **#pre-footer**: eyebrow "Nossa Galeria" e título "Momentos que inspiram" adicionados (estavam vazios)

### Preservado intocado
- Hero section completo (vídeo, carrossel, timer, textos, botões)
- Navbar e menu drawer
- Footer
- Seções #professor, #contato, #interesse, #missao
- Todo o JavaScript existente
- Identidade visual (cores, fontes dos tokens originais)
