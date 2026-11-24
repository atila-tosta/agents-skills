# agents-skills

Minha base pessoal de skills para o Claude, organizada como um **marketplace de plugins**.

## Estrutura

```
.claude-plugin/marketplace.json   # catálogo do marketplace
plugins/
├── pessoal/    # skills de uso pessoal
├── trabalho/   # skills de Arquiteto de IA
└── conteudo/   # texto, áudio, vídeo etc.
    ├── .claude-plugin/plugin.json
    └── skills/<nome-da-skill>/SKILL.md
template/skill-template/          # ponto de partida para novas skills
```

Cada plugin = uma categoria. Dentro de `skills/`, cada skill é uma pasta com um `SKILL.md`
(frontmatter `name` + `description`) e, opcionalmente, `references/`, `scripts/` e `assets/`.

## Criar uma skill

```bash
cp -r template/skill-template plugins/<categoria>/skills/<nome-da-skill>
# edite o SKILL.md
```

## Usar

```
/plugin marketplace add /Users/atilatosta/Documents/projetos/pessoal/agents-skills
/plugin install pessoal@agents-skills
/plugin install trabalho@agents-skills
/plugin install conteudo@agents-skills
```

Para testar sem instalar: `claude --plugin-dir plugins/trabalho`.

## Convenções
- Nomes de skill em `kebab-case`, descritivos (`proposta-tecnica-ia`, `roteiro-video`).
- A `description` diz o que faz **e quando acionar** — é o que dispara a skill.
- `SKILL.md` enxuto; detalhes longos vão para `references/`.
