# IDRISK2 — conversão Word → LaTeX (feupteses)

A dissertação foi convertida do manuscrito Word para este projeto LaTeX **feupteses**
(template oficial FEUP/U.Porto), configurado para o curso **MIA**.

## O que foi feito

- `main.tex` configurado: `\usepackage[mia]{feupteses}`, título, autora (Bianca Oliveira),
  orientador **Prof. Luís Paulo Reis** e um campo para o **co-orientador**.
- Corpo dividido por capítulos: `body/chapter1.tex` … `body/chapter8.tex`
  (Introduction, Background, Literature Review, Methodology, Evaluation and Results,
  Discussion, Conclusion, Future Work).
- Figuras extraídas para `figures/fig1.png … fig5.png` (em ambientes `figure` com legenda).
- Tabelas convertidas (booktabs/longtable); equações e símbolos preservados.
- `frontmatter/abbrevs.tex` preenchido com a lista de acrónimos (48 entradas).
- `frontmatter/abstract.tex` (Resumo PT + Abstract EN) e `frontmatter/acknows.tex`
  criados como **stubs com `TODO:`** (a vermelho).
- `backmatter/bibliography.bib` **preenchido com 99 referências** (juntei os teus dois `.bib`,
  removi duplicados e o conteúdo default FPGA/neuromorphic).
- **90 citações em texto** "(Autor, ano)" convertidas automaticamente para `\parencite{...}` /
  `\textcite{...}`. Verifiquei: todas as chaves existem e a lista de referências gera ~86 entradas.

## Como usar no Overleaf

1. Comprimir a pasta `overleaf-idrisk2/` num `.zip` **ou** ligar via Git.
2. No Overleaf: *New Project → Upload Project* (o zip) ou *Import from GitHub*.
3. Definir o documento principal como `main.tex`. Compilador: **pdfLaTeX** (o template usa Biber
   para a bibliografia — o Overleaf trata disso automaticamente).
4. Partilhar o link (botão *Share*) para enviar ao orientador.

## TODO antes da entrega

- [ ] **Abstract** (EN) e **Resumo** (PT) — `frontmatter/abstract.tex`.
- [ ] **Agradecimentos** — `frontmatter/acknows.tex`.
- [ ] **Referências (quase feito)** — bibliografia preenchida e 92 citações já ligadas.
      Ambiguidades resolvidas: Zhu 2024 → Zhu \& Chen; Zhang 2024 → Multimodal LLMs;
      "Eftimov 2017" era Mezgec \& Eftimov (ano corrigido p/ 2018).
      Faltam ~6 citações sem entrada no `.bib` (adicionar a referência ou corrigir autor/ano):
      **EFSA 2019, Eftimov 2020, Le 2025, Liu 2024, Sadeghi-Tehran 2019, Waikar 2026**.
      Confirmar ainda a inconsistência Molfetta et al. 2025/2026.
- [ ] **Co-orientador** — nome em `main.tex` (`Second Supervisor`).
- [ ] **Palavras-chave / Keywords** — confirmar em `abstract.tex`.
- [ ] Rever quebras de página de figuras/tabelas e legendas das tabelas.

> `IDRISK2_preview_conteudo.pdf` é uma pré-visualização **do conteúdo** (classe genérica). A capa,
> índices e tipografia FEUP aparecem ao compilar `main.tex` no Overleaf.
