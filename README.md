# Achei Meus Antecedentes Criminais e Civis

> Ferramenta gratuita de utilidade pública que reúne, em um único mapa interativo do Brasil, os links **oficiais** para emissão de certidões de antecedentes criminais, civis, eleitorais e federais — por estado.

🔗 **Site no ar:** [antecedentes.guiadasegurancadigital.com.br](https://antecedentes.guiadasegurancadigital.com.br/)

---

## Capturas de tela

**Página inicial**
![Tela inicial do Achei Meus Antecedentes](img/Home.png)

**Mapa interativo do Brasil**
![Mapa do Brasil clicável, com os 26 estados e o Distrito Federal](img/mapa-brasil.png)

**Exemplo: estado selecionado (Pará)**
![Exemplo de seleção do estado do Pará, mostrando os links de Polícia Civil, Tribunal de Justiça, TRE e TRF](img/mapa-brasil-exemplo-para.png)

**Órgãos federais**
![Cards dos órgãos federais: Polícia Federal, TSE, TST, Receita Federal/PGFN e STJ](img/orgaos-federais.png)

---

## O problema que resolve

Cada estado brasileiro tem seu próprio sistema de Polícia Civil, Tribunal de Justiça e Tribunal Regional Eleitoral — com domínios, nomes e fluxos completamente diferentes entre si. Quem precisa de uma certidão de antecedentes (para emprego, concurso, processo seletivo, etc.) frequentemente cai em buscas genéricas no Google e acaba em sites de terceiros que cobram por algo que é **gratuito**, ou pior, em páginas fraudulentas.

Esta ferramenta resolve isso reunindo, em um só lugar, **apenas links verificados manualmente** para domínios `.gov.br` e `.jus.br` oficiais — sem cobrar nada e sem coletar nenhum dado pessoal do visitante.

## O que está incluído

- **26 estados + Distrito Federal** (as 27 unidades federativas), cada um com:
  - Polícia Civil (antecedentes criminais estaduais)
  - Tribunal de Justiça (certidões cíveis e criminais)
  - Tribunal Regional Eleitoral (quitação eleitoral)
- **6 Tribunais Regionais Federais** (Justiça Federal, mapeados por jurisdição)
- **5 órgãos federais**: Polícia Federal, TSE, TST (CNDT), Receita Federal/PGFN, STJ

Todos os links foram conferidos manualmente em fontes oficiais — nenhum foi gerado por padrão de URL sem verificação.

## Stack

Projeto **single-file**: HTML, CSS e JavaScript puros, sem build step, sem dependências externas de runtime (além de Google Fonts via CDN). O mapa do Brasil é um SVG com paths reais por UF, clicável via JavaScript vanilla.

Por quê: facilita hospedagem em qualquer ambiente simples (neste caso, hospedagem compartilhada Localweb), sem necessidade de pipeline de build.

## Como rodar localmente

Não há dependências de build. Basta abrir o arquivo diretamente:

```bash
git clone https://github.com/SEU_USUARIO/achei-meus-antecedentes.git
cd achei-meus-antecedentes
# abra index.html no navegador, ou sirva com qualquer servidor estático:
python3 -m http.server 8000
```

## Roadmap

- [x] **v1.0** — Página única (SPA), mapa interativo, 26 estados + Distrito Federal + 6 TRFs + 5 órgãos federais, todos os links verificados manualmente
- [ ] **v1.1** — Compressão/otimização de imagens, ajustes finos de acessibilidade (contraste, navegação por teclado)
- [ ] **v1.2** — Página dedicada de "última verificação" por estado, com data de checagem de cada link
- [ ] **v2.0** — Uma URL própria por estado (ex: `/antecedentes/sp`), permitindo indexação individual em buscadores e SEO direcionado por estado

Contribuições e correções de link são bem-vindas via issue ou pull request.

## Por que isso é open source

Esse projeto nasceu para ajudar o cidadão brasileiro a não cair em golpe ao tentar emitir uma certidão simples. Faz sentido que o código também seja aberto: qualquer pessoa pode auditar os links, sugerir correções, ou adaptar para outro uso de utilidade pública.

## Licença

Distribuído sob a licença [MIT](LICENSE). Uso, modificação e redistribuição são livres, desde que o aviso de copyright e a licença original sejam mantidos.

## Autor

**Pablo Nunes de Oliveira**
Perito em Computação Forense · Analista de Segurança da Informação · Guia da Segurança Digital

- LinkedIn: [linkedin.com/in/pablonoliveirapro](https://www.linkedin.com/in/pablonoliveirapro)
- Instagram: [@pablonoliveirapro](https://www.instagram.com/pablonoliveirapro)
- Site: [guiadasegurancadigital.com.br](https://www.guiadasegurancadigital.com.br/)
