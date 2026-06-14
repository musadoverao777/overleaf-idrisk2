# IDRISK2 — conversão Word → LaTeX (feupteses)

A dissertação foi convertida do manuscrito Word para este projeto LaTeX **feupteses**
(template oficial FEUP/U.Porto), configurado para o curso **M.EIC** (Mestrado em Engenharia Informática e Computação).

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

- [x] **Abstract** (EN) e **Resumo** (PT) escritos em `frontmatter/abstract.tex` (aprovados; sem travessões).
- [ ] **Agradecimentos**: `frontmatter/acknows.tex` (ainda stub TODO).
- [x] **Referências** — bibliografia preenchida e ~96 citações ligadas; 0 citações indefinidas.
      Resolvidas as ambíguas (Zhu→Zhu \& Chen; Zhang→Multimodal LLMs; "Eftimov 2017"→Mezgec et al. 2018)
      e as 6 lacunas: Sadeghi-Tehran 2019 e EFSA 2015 (pág. 26) religadas; e adicionadas 4 referências novas
      — FoodEx2vec (Eftimov et al. 2020), Le et al. 2025 (Sensors), LLaVA-NeXT (Liu et al. 2024),
      Waikar et al. 2026. ("EFSA 2019" não era citação — é a série "EFSA Supporting Publications".)
- [x] **FEAST (Molfetta et al.)** — unificado em **2025** (versão publicada, Frontiers in AI and
      Applications / ECAI, DOI 10.3233/faia251309). Removida a entrada preprint 2026; todas as
      citações apontam para a de 2025.
- [ ] **Co-orientador** — nome em `main.tex` (`Second Supervisor`).
- [ ] **Palavras-chave / Keywords**: confirmar/ajustar as sugeridas em `abstract.tex`.
- [ ] Rever quebras de página de figuras/tabelas e legendas das tabelas.

> `IDRISK2_preview_conteudo.pdf` é uma pré-visualização **do conteúdo** (classe genérica). A capa,
> índices e tipografia FEUP aparecem ao compilar `main.tex` no Overleaf.
