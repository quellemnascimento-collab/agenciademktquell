# Como Usar os Agentes GPT — Quellnodigital

---

## O Que Sao Estes Arquivos

Cada arquivo nesta pasta e uma instrucao completa para criar um GPT Custom Agent especializado em uma area da Quellnodigital.

---

## Como Criar um GPT Customizado

1. Acesse: chat.openai.com → Explorar GPTs → Criar
2. Clique em "Configurar"
3. Preencha:
   - **Nome:** ex. "Social Media Quellnodigital"
   - **Descricao:** ex. "Especialista em social media estrategico da Quellnodigital"
   - **Instrucoes:** cole o conteudo COMPLETO do arquivo correspondente
4. Em "Conhecimento": voce pode fazer upload dos arquivos SKILL.md de cada pilar como contexto adicional
5. Salve e comece a usar

---

## Agentes Disponíveis

| Arquivo | Especialidade | Quando Usar |
|---------|-------------|------------|
| agente-master-gpt.md | Agente completo da agencia | Para tarefas gerais e estrategicas |
| agente-social-media-gpt.md | Social media e conteudo | Calendarios, copys, roteiros |
| agente-performance-gpt.md | Trafego pago e conversao | Campanhas, anuncios, analise de performance |
| agente-branding-gpt.md | Branding e posicionamento | Diagnostico de marca, identidade verbal |
| agente-ia-automacao-gpt.md | IA e automacoes | Fluxos, bots, integrações |
| agente-mentoria-gpt.md | Mentoria e consultoria | Sessoes com clientes, diagnostico de negocio |

---

## Como Usar no Claude (Cowork e Projetos)

No inicio de cada sessao de projeto de cliente, cole o conteudo de SKILL-MASTER.md como contexto inicial.

Para tarefas especificas, adicione tambem o SKILL.md do pilar correspondente.

Exemplo: para criar o calendario editorial de um cliente, cole:
1. SKILL-MASTER.md (contexto da agencia)
2. 01-social-media-inteligente/SKILL.md (expertise especifica)
3. Informacoes do cliente (briefing, ICP, tom)

---

## Como Usar no Lovable

Cole o conteudo de SKILL-MASTER.md como "System Prompt" do projeto.
Adicione informacoes especificas do produto que esta sendo construido.
O agente vai atuar como tech lead + copywriter + estrategista integrado.

---

## Como Usar no Manus

Configure o agente com o SKILL-MASTER.md como instrucao base.
Para tarefas autonomas, especifique o pilar ativo e o objetivo da tarefa.
O Manus vai executar em loop com checkpoints — configure aprovacao humana para publicacoes.

---

## Dica de Ouro

Quanto mais contexto do cliente voce der ao agente, melhor a entrega.
Nunca peca "crie um post" — peca "crie um post de aquisicao para uma clinica de estetica em Serra/ES, publico feminino 30-50 anos, objetivo: agendar avaliacao gratuita, tom: profissional e acolhedor."
