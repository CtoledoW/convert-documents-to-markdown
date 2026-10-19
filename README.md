# convert-documents-to-markdown

Skill que ensina o Claude a converter documentos em Markdown com a ferramenta **anydoc**. Formatos aceitos: Word, PowerPoint, Excel, OpenDocument, RTF, EPUB, CSV e PDF.

> **Esta é uma cópia sem modificações** da skill publicada pela **Firecrawl** no repositório **[firecrawl/anydoc](https://github.com/firecrawl/anydoc)**. **Recomendamos instalar pela fonte oficial**, que recebe as atualizações.

## O que a skill faz

- Executa a anydoc pela linha de comando, sem instalação prévia: `npx -y @firecrawl/anydoc <arquivo>`.
- Grava documentos grandes em arquivo (`-o saida.md`) para ler só as partes necessárias.
- Explica os códigos de saída (0 sucesso, 1 falha, 2 erro de uso, 3 PDF precisa de OCR).

## Como instalar

### Pela fonte oficial (recomendado)

```bash
npx skills add firecrawl/anydoc
```

### Instalação manual a partir deste repositório

No **Claude Code**, clone o repositório na pasta de skills pessoais (vale para todos os projetos):

```bash
git clone https://github.com/CtoledoW/convert-documents-to-markdown.git ~/.claude/skills/convert-documents-to-markdown
```

Para usar em um único projeto, clone em `.claude/skills/convert-documents-to-markdown/`, dentro da pasta do projeto.

No **app Claude**, compacte a pasta da skill (com o `SKILL.md`) em um arquivo `.zip`. Depois, envie esse arquivo na área de skills das configurações.

## Como usar

```text
Converta o arquivo briefing-cliente.docx para Markdown, salve como
briefing-cliente.md e me dê um resumo dos requisitos em tópicos.
```

## Requisitos e limitações

- Requer **Node.js 20 ou superior** e acesso ao npm.
- A anydoc não faz OCR localmente. A opção `--ocr hosted` **envia o documento** a um serviço externo da Firecrawl; evite usá-la com arquivos confidenciais.

## Créditos

- **Autoria:** [Firecrawl](https://github.com/firecrawl) (Sideguide Technologies Inc.), no repositório [firecrawl/anydoc](https://github.com/firecrawl/anydoc/tree/main/skills/convert-documents-to-markdown).
- **Alterações nesta cópia:** nenhuma na skill. Foi adicionado apenas este `README.md` em português.

## Série *Do Planejamento ao Código*

Este repositório faz parte do material educacional gratuito *Do Planejamento ao Código — 5 Skills para Desenvolver Projetos com Inteligência Artificial*, da Brismarp Tecnologia.

| Capítulo | Repositório |
|---|---|
| 1. Planejamento e orquestração | [maestro](https://github.com/CtoledoW/maestro) |
| 2. Arquitetura e organização do ambiente | [claude-code-setup](https://github.com/CtoledoW/claude-code-setup) |
| 3. Desenvolvimento e implementação | [using-agent-skills](https://github.com/CtoledoW/using-agent-skills) |
| 4. Automação e produtividade | **convert-documents-to-markdown** (este) |
| 5. Qualidade e curadoria de ferramentas | [find-skills](https://github.com/CtoledoW/find-skills) |

## Licença

[MIT](LICENSE) © 2026 Sideguide Technologies Inc., conforme o repositório original.

---

**Brismarp Tecnologia** — Inovação que conecta ideias ao futuro

Material gratuito e educacional. Se este repositório ajudou você, dê os créditos aos autores originais citados acima.
