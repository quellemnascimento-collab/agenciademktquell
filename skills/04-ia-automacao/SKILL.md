# Skill: IA e Automacao Aplicada — Quellnodigital

Especialista em implementar inteligencia artificial e automacoes nos processos de marketing, atendimento e vendas. Transforma tarefas manuais em sistemas que funcionam enquanto o cliente dorme.

---

## Quando Usar Esta Skill

- Mapear oportunidades de automacao no negocio do cliente
- Criar fluxos de automacao (WhatsApp, e-mail, CRM)
- Desenhar agentes IA para atendimento e qualificacao de leads
- Usar IA para producao de conteudo com curadoria estrategica
- Analisar dados de marketing com IA
- Configurar nutricao automatica de leads

---

## Principio Central

IA nao substitui estrategia humana — potencializa execucao.
Cada automacao deve servir a um objetivo de negocio claro.
Nunca automatize o que precisa ser humano (relacionamento de alto valor, decisoes criticas, atendimento em crise).

---

## Fluxo de Trabalho

### PASSO 1 — MAPEAMENTO DE OPORTUNIDADES

Faca as perguntas:
- Quais tarefas repetitivas o cliente ou o time faz todo dia?
- Onde leads estao "caindo" no funil sem nutricao?
- Quanto tempo e gasto respondendo as mesmas perguntas?
- O cliente tem CRM? Usa? Qual?
- Como e o atendimento via WhatsApp hoje?

**Mapa de priorizacao de automacoes:**

| Automacao | Impacto (1-5) | Esforco (1-5) | Prioridade |
|-----------|--------------|--------------|-----------|
| Resposta automatica WhatsApp | 5 | 2 | ALTA |
| Sequencia de boas-vindas (email) | 4 | 2 | ALTA |
| Nutricao de leads (email) | 5 | 3 | ALTA |
| Agendamento automatico | 4 | 2 | MEDIA |
| Relatorio automatico | 3 | 3 | MEDIA |
| Recuperacao de abandono | 5 | 4 | MEDIA |

### PASSO 2 — DESIGN DO FLUXO DE AUTOMACAO

Para cada automacao, documente:

```
FLUXO: [Nome da automacao]
OBJETIVO: [O que resolve]
GATILHO: [O que inicia o fluxo]
PLATAFORMA: [WhatsApp / E-mail / CRM / Site]

PASSOS DO FLUXO:
1. [Evento/acao que dispara]
2. [Mensagem ou acao automatica]
3. [Condicao: SE [X] ENTAO [Y]]
4. [Proximo passo]
...
N. [Saida do fluxo ou handoff humano]

HANDOFF HUMANO:
Quando um atendente real assume: [criterio]
```

### PASSO 3 — FLUXOS ESSENCIAIS (Templates)

**Fluxo 1: Boas-Vindas WhatsApp (novo lead)**
```
GATILHO: Lead preenche formulario no site
FERRAMENTA: Make + WhatsApp Business API

Passo 1 — Imediato (0 min):
  "Oi [Nome]! 👋 Sou a assistente da [Empresa].
   Recebi seu contato e ja avisei o time.
   Em ate [X horas] alguem fala com voce.
   Enquanto isso, posso te ajudar com algo?"

Passo 2 — Menu de opcoes (bot):
  1. Quero saber os precos
  2. Quero agendar uma conversa
  3. Tenho outra duvida

Passo 3A (escolheu preco):
  "Claro! Temos [X opcoes]. Posso te mandar um resumo?"
  [envia tabela de servicos]
  "Quer agendar uma conversa para eu detalhar o que faz mais sentido para voce?"

Passo 3B (escolheu agendar):
  "Perfeito! [Link Calendly] — escolha o melhor horario."

HANDOFF: Quando mencionar concorrente, preco especifico ou reclamacao → notificar humano
```

**Fluxo 2: Nutricao de Leads (sequencia de e-mail)**
```
GATILHO: Lead baixa lead magnet
FERRAMENTA: RD Station / ActiveCampaign

Email 1 — Imediato: Entrega do material + apresentacao
Email 2 — Dia 2: Dica relacionada ao problema (valor)
Email 3 — Dia 4: Case de resultado (prova social)
Email 4 — Dia 7: Oferta de diagnostico gratuito (CTA)
Email 5 — Dia 14: Ultimo contato (urgencia suave)

CADA EMAIL TEM:
- Assunto: maximo 50 caracteres, curiosidade ou beneficio
- Preview: complementa o assunto
- Body: menos de 200 palavras
- 1 CTA por email (nao mais)
```

**Fluxo 3: Agente IA para Qualificacao de Leads**
```
OBJETIVO: Qualificar leads antes de chegar ao comercial humano

PERGUNTAS DO AGENTE:
1. "Qual e o seu negocio?" (segmento)
2. "Voce ja investe em marketing digital hoje?" (maturidade)
3. "Qual e o principal desafio que quer resolver?" (dor)
4. "Qual orcamento mensal voce considera para marketing?" (ticket fit)

CRITERIOS DE QUALIFICACAO:
Lead Quente: responde tudo, orcamento alinhado → notificar comercial imediatamente
Lead Morno: responde parcialmente → nutricao por email por 7 dias
Lead Frio: orcamento incompativel → sequencia educativa longa

ENTREGA: Ficha do lead qualificado para o comercial com score (1-10)
```

### PASSO 4 — IA NA PRODUCAO DE CONTEUDO

**Fluxo de criacao assistida por IA (para o time):**

1. **Briefing humano:** estrategista define objetivo, publico e mensagem-chave
2. **Draft IA:** IA gera 3 versoes de copy para o formato
3. **Curadoria humana:** copywriter ou estrategista seleciona e ajusta
4. **Aprovacao:** cliente aprova versao final
5. **Publicacao:** social media manager agenda

**Prompts padrao para producao de conteudo:**

```
PROMPT — REEL (roteiro):
"Crie um roteiro para reel de [X segundos] para [cliente/segmento].
Objetivo: [aquisicao/consideracao/retencao].
Hook: deve parar o scroll em 3 segundos.
Tema: [tema especifico].
Tom: [descricao do tom da marca].
Terminar com CTA: [acao especifica].
Formato: fala direta para camera, sem texto na tela exceto no hook."

PROMPT — CAROUSEL:
"Crie um carousel de [X slides] sobre [tema] para [cliente].
Slide 1 (capa): titulo que gera curiosidade
Slides 2 a [X-1]: conteudo com progressao logica
Ultimo slide: CTA claro
Tom: [descricao]
Nao use bullet points — escreva frases completas e simples."

PROMPT — COPY DE ANUNCIO:
"Crie 3 versoes de copy para anuncio Meta Ads.
Produto/servico: [descricao]
Publico: [descricao do ICP]
Objetivo do anuncio: [lead / venda / trafego]
Inclua: hook de 1 linha, desenvolvimento de 2-3 linhas, CTA especifico.
Tom: [descricao]"
```

---

## Stack de Ferramentas Recomendado

| Caso de Uso | Ferramenta Principal | Alternativa |
|-------------|---------------------|------------|
| Automacao de WhatsApp | Make + WA Business API | Manychat |
| E-mail marketing + CRM | RD Station | ActiveCampaign |
| Integracao entre sistemas | Make (Integromat) | Zapier |
| Agente IA conversacional | Claude API | ChatGPT API |
| Geracao de conteudo IA | Claude + Midjourney | ChatGPT + DALL-E |
| Agendamento automatico | Calendly | Cal.com |
| Formularios inteligentes | Typeform | Tally |

---

## Referencias

- `references/agencia-dna.md` — proposito e valores
- `07-protocolo-q/SKILL.md` — fases de implementacao com o cliente
- `06-estrutura-operacional/ferramentas-stack.md` — stack completo da agencia
