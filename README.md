# Capacitação de Git e GitHub

![Git](https://img.shields.io/badge/Git-Controle_de_Versão-F05032?logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Pages_e_Actions-181717?logo=github)
![Publicação](https://img.shields.io/badge/GitHub_Pages-publicado-614AD3)
![Licença](https://img.shields.io/badge/conteúdo-CC_BY--SA_4.0-lightgrey)

Material público da capacitação introdutória de **Git e GitHub** da liga
acadêmica for_code, com duração de **2 horas**, sem pré-requisitos.

### 📖 **[Acessar o material](https://andradasdev.github.io/github/)**

| | |
|---|---|
| 📘 Guia completo, com exercícios | [`docs/guia.pdf`](docs/guia.pdf) |
| 🖥️ Slides da apresentação | [`docs/apresentacao.pdf`](docs/apresentacao.pdf) |
| 🎮 Site do exercício de GitHub Pages | [`materials/jogo-da-memoria.zip`](materials/jogo-da-memoria.zip) |
| 🐍 Script do exercício de GitHub Actions | [`materials/main.py`](materials/main.py) |
| ⚙️ Exemplo de workflow em Fortran | [`materials/modelo-actions.zip`](materials/modelo-actions.zip) |

---

## 🧭 Este repositório é só de publicação

Aqui ficam apenas os **artefatos prontos**. Eles não são editados neste
repositório: chegam por automação, compilados a partir das fontes LaTeX.

> ### 👉 Para ver o código-fonte, ir ao repositório de código:
> ## **[github.com/ronidomingues/github-training](https://github.com/ronidomingues/github-training)**
>
> É lá que estão as fontes `.tex` do guia e dos slides, a lista de presença
> por Pull Request e o histórico de desenvolvimento. **Correções e
> contribuições devem ser abertas lá** — qualquer alteração feita diretamente
> aqui será sobrescrita na próxima publicação.

### Como o material chega até aqui

```
  ronidomingues/github-training                   andradasdev/github
  ─────────────────────────────                   ──────────────────
   fontes .tex, presenças, materiais
            │
            │  push na main
            v
   ┌──────────────────────┐
   │ workflow: build.yml  │
   │  1. lista presenças  │
   │  2. compila LaTeX    │
   │  3. verifica os PDFs │
   │  4. commita lá       │
   │  5. envia para cá ───┼──────────────>  guia.pdf
   └──────────────────────┘                 apresentacao.pdf
                                            materiais
                                                  │
                                                  │ dispara
                                                  v
                                        ┌──────────────────────┐
                                        │ workflow: pages.yml  │
                                        │  publica o site      │
                                        └──────────┬───────────┘
                                                   v
                                     andradasdev.github.io/github
```

A autenticação entre os dois repositórios está documentada em
**[`documentacao/autenticacao-github-actions.md`](documentacao/autenticacao-github-actions.md)**.

---

## 🎯 O que a capacitação cobre

Ao final, o participante é capaz de:

1. Criar e proteger a conta no GitHub (2FA) e pedir os benefícios de estudante
2. Instalar e configurar o Git e o GitHub CLI no Windows, no Linux ou no macOS
3. Fazer commits, trabalhar com branches e resolver um conflito
4. Contribuir por fork e Pull Request, com mensagens de commit padronizadas
5. Publicar um site com o GitHub Pages e automatizar uma tarefa com o GitHub Actions
6. Versionar arquivos grandes com o Git LFS e assinar commits (GPG ou SSH)

### Os 120 minutos

| # | Bloco | Início | Duração |
|---|---|---|---|
| 0 | Abertura, objetivos e combinados | 00:00 | 5 min |
| 1 | A conta no GitHub, 2FA e benefícios de estudante | 00:05 | 15 min |
| 2 | Instalação, configuração e login | 00:20 | 20 min |
| 3 | Git no dia a dia: commits, branches, merge e conflito | 00:40 | 20 min |
| — | *Pausa* | 01:00 | 5 min |
| 4 | Colaboração: fork, Pull Request e padrões de commit | 01:05 | 20 min |
| 5 | GitHub Pages e GitHub Actions | 01:25 | 15 min |
| 6 | Git LFS e assinatura de commits | 01:40 | 15 min |
| 7 | Encerramento e próximos passos | 01:55 | 5 min |
| | **Total** | | **120 min** |

---

## 📂 Estrutura

```
github/
├── docs/
│   ├── guia.pdf              guia (gerado, não editar aqui)
│   └── apresentacao.pdf      slides (gerados, não editar aqui)
├── materials/
│   ├── jogo-da-memoria.zip   site do exercício de GitHub Pages
│   ├── main.py               script do exercício de GitHub Actions
│   └── modelo-actions.zip    exemplo de workflow em Fortran
├── documentacao/
│   └── autenticacao-github-actions.md
├── index.html                página publicada no GitHub Pages
├── LICENSE                   MIT, para o código
├── LICENSE-CONTENT           CC BY-SA 4.0, para o conteúdo didático
└── README.md
```

---

## ⚖️ Licença

- **Conteúdo didático** (guia, slides, textos, exercícios) — [CC BY-SA 4.0](LICENSE-CONTENT)
- **Código** (materiais, workflows, `index.html`) — [MIT](LICENSE)

Você pode usar, adaptar e reaplicar este material, inclusive comercialmente,
desde que dê o crédito e mantenha a mesma licença nas suas adaptações.

## 👨‍🏫 Autor

**Ronivaldo Domingues de Andrade**
LinkedIn: [ronidomingues](https://www.linkedin.com/in/ronidomingues/) ·
GitHub: [@ronidomingues](https://github.com/ronidomingues)
📍 Rio de Janeiro — RJ

### ⭐ Se este material foi útil, considere dar uma estrela no repositório!
