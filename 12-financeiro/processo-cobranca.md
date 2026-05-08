# Processo de Cobranca e Gestao Financeira - Quellnodigital
## @quellnodigital

---

## 1. CICLO DE COBRANCA MENSAL

### Para Servicos Recorrentes (MRR)

| Dia | Acao |
|-----|------|
| Dia 25 do mes anterior | Enviar aviso de cobranca + NF (quando possivel) |
| Dia 1-5 (vencimento padrao) | Verificar pagamentos recebidos |
| Dia 6 | Listar inadimplentes |
| Dia 7-8 | Primeiro contato amigavel (WhatsApp) |
| Dia 10 | Segundo contato + link de pagamento |
| Dia 15 | Terceiro contato + aviso de suspensao |
| Dia 20 | Suspender servicos se nao houver pagamento |
| Dia 30 | Iniciar processo de encerramento se necessario |

### Script de Cobranca

**Dia 6 (amigavel):**
Oi [Nome]! Passando para avisar que a mensalidade de [mes] vence amanha. Se precisar, e so me avisar para ajustarmos. Pix/Boleto: [link]

**Dia 10 (segundo contato):**
Oi [Nome], vi que a mensalidade de [valor] ainda esta em aberto. Pode verificar? Segue o link para pagamento: [link]. Qualquer duvida, so falar!

**Dia 15 (aviso formal):**
[Nome], estou precisando que regularize o pagamento de [valor] referente a [mes]. Em caso de nao quitacao ate [data], precisarei pausar os servicos conforme nosso contrato. Segue link: [link]

---

## 2. FERRAMENTAS DE COBRANCA

### Asaas (Recomendado)

**Por que Asaas:**
- Emite boleto, Pix e cartao de credito
- Cobra automaticamente por recorrencia
- Envia lembretes automaticos
- Integra com NFS-e em alguns municipios
- Relatorio de inadimplencia automatico

**Configuracao de cobranca recorrente:**
1. Cadastrar cliente
2. Criar assinatura com valor e vencimento
3. Ativar envio automatico de cobranca (7 dias antes)
4. Ativar lembrete automatico no dia do vencimento
5. Ativar aviso automatico de atraso

**Custo:** 0,99% por transacao Pix / 1,99% boleto / 2,49%+ cartao

### Alternativas:
- Stripe: melhor para cobrar em dolar (clientes internacionais)
- PagSeguro: boa para cartao, porem taxas maiores
- Transferencia Pix direto: zero custo, porem sem automacao

---

## 3. PROCESSO DE EMISSAO DE NOTA FISCAL

### Quando emitir:
- **Servicos recorrentes:** emitir no inicio do mes de competencia (dia 1-5)
- **Projetos:** emitir em cada parcela recebida

### Informacoes obrigatorias na NF:
- CNPJ e razao social do cliente (ou CPF e nome se pessoa fisica)
- Descricao detalhada do servico
- Competencia do servico
- Valor bruto
- ISS retido (se aplicavel)
- Dados da empresa emissora

### Arquivamento:
- Salvar PDF da NF em: Drive > Financeiro > Notas Fiscais > [ANO] > [MES]
- Nomear como: NF_[Numero]_[Cliente]_[MesAno].pdf

---

## 4. GESTAO DE CONTRATOS E RENOVACOES

### Dashboard de Contratos

Manter planilha atualizada com:

| Campo | Descricao |
|-------|-----------|
| Cliente | Nome e empresa |
| Servico | Tipo de servico |
| Plano | Starter/Growth/Authority etc |
| Valor | R [valor]/mes |
| Inicio | Data inicio do contrato |
| Vigencia | Duracao contratada |
| Proxima renovacao | Data |
| Status | Ativo/Em risco/Cancelado |
| Responsavel CS | Nome do CS responsavel |

### Alerta de Renovacao:
- Sistema deve alertar 30 dias antes do vencimento
- CS deve entrar em contato com cliente 15 dias antes
- Proposta de renovacao enviada 10 dias antes

---

## 5. POLITICA DE DEVOLUCAO

**Servicos recorrentes:**
- Nao ha devolucao de mensalidades ja pagas
- Cancelamento com 30 dias de aviso: mes corrente e pago integralmente, sem cobranca adicional
- Cancelamento sem aviso: multa conforme contrato

**Projetos:**
- Sinal (30-50%): nao devolvido em caso de desistencia apos inicio
- Parcelas intermediarias: nao devolvidas apos entrega da fase correspondente
- Entrega final: nao devolvida apos aprovacao do cliente

---

## 6. COMISSOES E REMUNERACAO VARIAVEL

### Estrutura de Comissao para SDR/Vendedor

| Tipo de Receita | Comissao |
|----------------|---------|
| Novo cliente recorrente (MRR) | 10% do primeiro mes |
| Renovacao com upgrade | 5% da diferenca |
| Indicacao que fecha | 5% do primeiro mes |
| Projeto avulso | 5% do valor total |

**Pagamento:** No mes subsequente ao fechamento confirmado e com pagamento realizado

### Comissao por Retencao (CS)

- Cliente retido no mes: R 100 bonus por cliente acima de 6 meses
- NPS medio acima de 9: bonus mensal de R 300

---

## 7. RESERVA FINANCEIRA

### Meta de reserva:
- Manutencao: 3 meses de custos fixos em caixa
- Crescimento: adicionar 10% de cada mes recorrente

### Distribuicao do faturamento:
- 40% pro-labore (Marcia)
- 30% reinvestimento (equipe, ferramentas, marketing)
- 20% reserva de emergencia
- 10% impostos e contador

---

*Quellnodigital - Saude financeira e base de crescimento.*
