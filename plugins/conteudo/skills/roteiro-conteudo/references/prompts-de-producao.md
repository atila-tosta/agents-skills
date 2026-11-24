# Prompts de produção (opcional)

Use este guia só quando o usuário disser no briefing que quer gerar assets (imagem, áudio/trilha, vídeo/animação ou personagem). Se ele só vai gravar com a própria voz e câmera, não gere nada daqui.

## Índice
- Ficha de personagem
- Prompt de imagem
- Prompt de vídeo/animação
- Prompt de áudio, voz e trilha
- Como encaixar nos blocos
- Princípios gerais

## Ficha de personagem
Crie **uma vez**, no início do roteiro, quando houver personagem recorrente (mascote, apresentador virtual, protagonista de animação). Depois, **copie o texto da descrição fixa literalmente** em cada prompt de imagem e vídeo. É a forma mais confiável de manter a aparência consistente entre cenas, porque cada geração começa do zero e só "lembra" do que está escrito no prompt.

Campos:
- **Nome / papel** (ex.: "Léo, apresentador do canal")
- **Descrição fixa** (um parágrafo curto e concreto): idade aparente, rosto, cabelo, cor da pele, corpo, roupa e acessórios fixos, paleta de cores. Evite adjetivos vagos ("bonito", "legal").
- **Estilo visual** (realista, 2D, 3D estilo desenho, pixel art etc.), igual em todas as cenas.
- **Personalidade e voz** (como se move, expressões típicas, tom da voz), útil para direção de cena e para escolher a voz.
- **Referência** (imagem de referência gerada ou enviada pelo usuário), se houver. Sugira gerar primeiro uma imagem-base do personagem e usá-la como referência nas cenas seguintes.

## Prompt de imagem
Estrutura sugerida, em uma ou duas frases por item e sem enrolação:
`[sujeito + ação] · [cenário] · [enquadramento/ângulo] · [iluminação] · [estilo e paleta] · [emoção/atmosfera] · [proporção, ex.: 9:16]`
- Para personagem: inclua a descrição fixa da ficha.
- Diga o que quer, não o que não quer (negativos só se a ferramenta usar campo próprio).
- Texto dentro da imagem costuma sair errado: prefira colocar o texto na edição.
- Adapte a proporção à plataforma (9:16 Reels/TikTok/Shorts, 16:9 YouTube, 1:1 feed).

## Prompt de vídeo/animação
Descreva **um plano por prompt**, com uma ação principal:
`[personagem/sujeito + ação única] · [cenário] · [movimento de câmera: parada, travelling, zoom in, panorâmica, câmera na mão] · [iluminação] · [estilo] · [emoção] · [duração: 3–8 s] · [proporção]`
- Clipes curtos: uma ideia, um movimento de câmera, poucas palavras. Excesso de instruções gera resultados confusos.
- Indique se o ponto de partida é uma imagem (imagem → vídeo) e qual.
- Se o personagem fala, avise (lip sync) e diga qual é a fala do bloco.
- Para continuidade, repita cenário, iluminação e estilo entre planos da mesma sequência.

## Prompt de áudio, voz e trilha
Separe em três tipos, conforme o que o bloco precisa:
1. **Voz/locução** (texto-para-fala): entregue o **texto exato** com as marcações de pausa e ênfase, mais a direção de voz: gênero/idade aparente, timbre, ritmo, emoção, sotaque/idioma. Se for um personagem, derive da ficha.
2. **Trilha musical**: gênero, andamento (BPM aproximado ou "lento/médio/rápido"), instrumentos, clima, energia ao longo do tempo (ex.: "começa suave, cresce no gancho"), duração, se é loop e se deve ter ou não vocais (quase sempre "instrumental, sem vocais" para não competir com a fala).
3. **Efeitos sonoros**: o som, a duração e o momento (ex.: "whoosh curto na transição, 0,5 s").
Indique o mix de forma simples: trilha baixa sob a fala, efeitos nos cortes.

## Como encaixar nos blocos
Abaixo da tabela `Fala | Visual` de cada bloco, acrescente **só os prompts que o usuário pediu**:

```
Bloco 2 — Desenvolvimento (0:08–0:25)
| Fala | Visual |
| ... | ... |
🎨 Prompt de imagem: ...
🎬 Prompt de vídeo: ...
🔊 Prompt de áudio/trilha: ...
```

Mantenha os prompts em um bloco separado e curto, para o usuário copiar e colar. Os prompts podem ficar no idioma que a ferramenta rende melhor (muitas funcionam melhor em inglês); se mudar o idioma, avise e ofereça a versão no idioma do usuário.

## Princípios gerais
- Os prompts nascem do roteiro: devem ser coerentes com a fala, o tom e a duração do bloco.
- Não prometa resultado exato: ferramentas de geração variam. Sugira gerar 2 ou 3 opções e escolher.
- Se o usuário tiver uma ferramenta específica (ex.: Runway, ElevenLabs), adapte o formato dos prompts a ela e respeite os limites de duração e proporção que ela aceita.
