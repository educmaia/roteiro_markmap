# PLANO DE ARQUITETURA: ROTEIRO → MARKMAP INTERATIVO

**Projeto:** Transformação do Roteiro de Entrevista Semiestruturada em Markmap Navegável
**Autor:** Eduardo Maia | Mestrado MUST
**Data:** 2025-11-12
**Arquivos Base:**
- `Roteiro Entrevista.pdf` (21 páginas - roteiro acadêmico completo)
- `Cheat_Sheet_1_Pagina.txt` (guia rápido de campo)
- `markmap_manual.md` (documentação técnica)

---

## 1. VISÃO GERAL DO PLANO

### Objetivo
Criar um markmap navegável que transforme o roteiro acadêmico de 21 páginas em uma ferramenta visual e prática para condução de entrevistas em campo.

### Princípios de Design
- **Dual-layer**: Camada simplificada (cheat sheet) + camada completa (roteiro detalhado)
- **Perfil-adaptável**: Navegação condicional baseada no perfil do entrevistado
- **7 Perguntas Core**: Sempre visíveis e destacadas
- **Teoria incorporada**: Construtos UTAUT e taxonomias visíveis mas não intrusivas

---

## 2. ARQUITETURA HIERÁRQUICA (5-6 NÍVEIS)

### Estrutura de Níveis
```
# NÍVEL 1: Âncora Principal
## NÍVEL 2: Blocos Temáticos (6 blocos)
### NÍVEL 3: Seções dentro dos blocos
#### NÍVEL 4: Perguntas principais
##### NÍVEL 5: Probes e variações
###### NÍVEL 6 (limitado): Notas metodológicas
```

### Estrutura de Navegação Principal

```
ENTREVISTA NÃO-ADOTANTES IA
├── 🎯 REGRA DE OURO
├── ⚡ 7 PERGUNTAS OBRIGATÓRIAS (sempre visível)
├── 📊 SELETOR DE PERFIL
│   ├── Adotante Pleno
│   ├── Não-Adotante Consciente
│   └── Experimentador
├── ⏱️ CHECKLIST TEMPORAL (50-70 min)
└── 📋 ROTEIRO COMPLETO
    ├── Bloco 1: Rapport (10-15 min)
    ├── Bloco 2: Práticas (15-20 min)
    ├── Bloco 3: Impactos (15-20 min)
    ├── Bloco 4: Influências Sociais (10-15 min)
    ├── Bloco 5: Barreiras (15-20 min)
    └── Bloco 6: Reflexões Finais (5-10 min)
```

---

## 3. ELEMENTOS ESTRATÉGICOS DO CHEAT SHEET

### A integrar no topo (sempre visíveis - fold: false)

#### 1. Regra de Ouro Box
```markdown
## 🎯 REGRA DE OURO
**PROBLEMA → EXPLICAR IA → PERGUNTAR**
```

#### 2. Explicação IA em 30seg (colapsável)
```markdown
### 💬 Como Explicar IA (se necessário)
"ChatGPT é tipo um assistente que escreve pra você. Você fala:
'Escreve legenda sobre blusa florida, algo divertido'. Em 10 seg
ele dá 3 opções prontas. Você escolhe, ajusta, posta. É tipo ter
estagiário de graça. Saca?"
<!-- markmap: fold -->
```

#### 3. 7 Perguntas Núcleo (destaque visual)
```markdown
## ⚡ 7 PERGUNTAS OBRIGATÓRIAS
### 1️⃣ Barreira Principal
"Qual o PRINCIPAL obstáculo que te impede de usar IA?"

### 2️⃣ Benefícios Esperados (PE)
"Você acha que IA te ajudaria com [PROBLEMA QUE ELA RELATOU]?"

### 3️⃣ Facilidade (EE)
"Seria FÁCIL ou DIFÍCIL pra você aprender? Por quê?"

### 4️⃣ Pressão Social (SI)
"Seus CONCORRENTES usam IA? Você sente que precisa usar?"

### 5️⃣ Recursos (FC)
"Teria TEMPO/DINHEIRO/AJUDA pra aprender?"

### 6️⃣ Estratégias sem IA
"Como você faz HOJE sem IA? Essas estratégias FUNCIONAM BEM?"

### 7️⃣ Autenticidade
"Você tem MEDO de perder a essência da marca ao usar IA?"
```

#### 4. Conectores Problema-IA (tabela visual)
```markdown
## 🔗 CONECTAR PROBLEMA COM IA

| Problema Relatado | Pergunta de Conexão |
|-------------------|---------------------|
| "Falta tempo" | "IA economizaria tempo pra você?" |
| "Faz tudo sozinha" | "IA seria tipo ter ajudante?" |
| "Difícil criar conteúdo" | "IA te dando ideias ajudaria?" |
| "Não sei se dá retorno" | "IA analisando dados ajudaria?" |
```

#### 5. Checklist de Cobertura (interativo)
```markdown
## ✓ CHECKLIST: COBRI TUDO?

- ☐ Por que NÃO usa? (Barreira principal)
- ☐ Performance Expectancy (Vê benefícios?)
- ☐ Effort Expectancy (Acha fácil/difícil?)
- ☐ Social Influence (Pressão de concorrentes?)
- ☐ Facilitating Conditions (Tem recursos?)
- ☐ Estratégias SEM IA (Como faz hoje?)
- ☐ Autenticidade (Medo de perder identidade?)
- ☐ Futuro (Vai usar daqui X anos?)
```

---

## 4. NAVEGAÇÃO POR PERFIL DO ENTREVISTADO

### Mecanismo de Ramificação Condicional

```markdown
## 📊 SELECIONE O PERFIL DO ENTREVISTADO

### 🟢 ADOTANTE PLENO
**Usa IA regularmente no marketing**

#### Perguntas Específicas
- Bloco 2: Perguntas 2.3-2.6
  - Primeiro contato com IA
  - Ferramentas utilizadas
  - Tarefas delegadas
  - Mudanças observadas
- Bloco 3: Perguntas 3.1-3.5
  - Benefícios realizados
  - Exemplos concretos
  - Facilidade/Dificuldade
  - Desafios e limitações

#### ⚠️ PULAR
- 2.7-2.10 (Não-adotantes)
- 3.6-3.10 (Expectativas projetadas)
<!-- markmap: fold -->

### 🔴 NÃO-ADOTANTE CONSCIENTE
**Conhece IA mas optou por não usar**

#### Perguntas Específicas
- Bloco 2: Perguntas 2.7-2.10
  - Conhecimento sobre IA
  - Razões para não-adoção
  - Estratégias alternativas
  - Pressão ou urgência
- Bloco 3: Perguntas 3.6-3.10
  - Expectativa projetada de desempenho
  - Complexidade percebida
  - Impactos negativos evitados
  - Comparação com estratégias atuais

#### ⚠️ PULAR
- 2.3-2.6 (Adotantes)
- 3.1-3.5 (Benefícios realizados)
<!-- markmap: fold -->

### 🟡 EXPERIMENTADOR / USUÁRIO LIMITADO
**Testou mas não incorporou ou usa ocasionalmente**

#### Perguntas Específicas
- Bloco 2: Perguntas 2.11-2.13
  - Experiência de experimentação
  - Razões para descontinuidade
  - Intenções futuras
- Bloco 3: Perguntas 3.11-3.12
  - Benefícios percebidos
  - Por que não foram suficientes

#### ⚠️ USAR
- Questões intermediárias de ambos os perfis
<!-- markmap: fold -->
```

---

## 5. ESTRUTURA DETALHADA DOS BLOCOS

### Template Padrão para Cada Bloco

```markdown
## 📋 BLOCO X: [NOME] (XX-XX min)

**Objetivo Específico:** [OE1/OE2/OE3]
**Construtos UTAUT:** [PE/EE/SI/FC]
**Teoria Base:** [Huang & Rust / Davenport / UTAUT]

---

### [TODOS] Perguntas para Todos os Perfis

#### X.X [Título da Pergunta]
"[Texto da pergunta principal]"

##### Probes
- Probe 1
- Probe 2
- Probe 3

##### Capturar
[Indicação do que observar/anotar - ex: maturidade digital, moderador UTAUT]

---

### 🟢 [ADOTANTES] Perguntas Específicas
<!-- markmap: fold -->

#### X.X [Título]
"[Pergunta específica para quem usa IA]"

##### Probes Estruturados
- **Task Automation**: "[probe focado em automação]"
- **Context Awareness**: "[probe focado em adaptação]"
- **Decision Support**: "[probe focado em análise]"

---

### 🔴 [NÃO-ADOTANTES] Perguntas Específicas
<!-- markmap: fold -->

#### X.X [Título]
"[Pergunta específica para quem NÃO usa IA]"

##### Se SIM
"[Follow-up para resposta positiva]"

##### Se NÃO
"[Follow-up para resposta negativa]"

##### Probes Específicos
- Custo?
- Aplicabilidade ao negócio?
- Qualidade/Autenticidade?
- Tempo/Conhecimento?

---

### 🟡 [EXPERIMENTADORES] Perguntas Específicas
<!-- markmap: fold -->

#### X.X [Título]
"[Pergunta específica para quem testou mas não continuou]"

---

### 📐 VARIAÇÕES POR PORTE
<!-- markmap: foldAll -->

#### Microempresas (< 10 funcionários)
"[Pergunta adicional após X.X] [texto adaptado para contexto de micro]"

#### Médias Empresas (50-249 funcionários)
"[Pergunta adicional após X.X] [texto adaptado para contexto de média]"

---

### 🏭 VARIAÇÕES POR SETOR
<!-- markmap: foldAll -->

#### Setor de Serviços
"[Pergunta adicional após X.X] [foco em relacionamento B2C/Feeling AI]"

#### Setor Industrial
"[Pergunta adicional após X.X] [foco em B2B/análise de dados]"
```

---

## 6. FEATURES TÉCNICAS DO MARKMAP

### Frontmatter Configuration

```yaml
---
markmap:
  colorFreezeLevel: 2
  initialExpandLevel: 2
  maxWidth: 300
  zoom: true
  pan: true
  spacingHorizontal: 100
  spacingVertical: 10
  color:
    - '#FF6B6B'  # Vermelho - Não-adotantes
    - '#4ECDC4'  # Azul - Adotantes
    - '#FFE66D'  # Amarelo - Experimentadores
    - '#95E1D3'  # Verde claro - Geral
    - '#A8E6CF'  # Verde água - Moderadores
    - '#F38181'  # Rosa - Alertas
  duration: 500
  activeNode:
    placement: 'visible'
---
```

### Magic Comments Estratégicos

| Localização | Magic Comment | Razão |
|-------------|---------------|-------|
| Blocos de variações por perfil | `<!-- markmap: foldAll -->` | Evitar poluição visual durante navegação |
| Seções de probes extensos | `<!-- markmap: fold -->` | Mostrar só quando necessário |
| Regra de Ouro | Nenhum (sempre aberto) | Máxima visibilidade |
| 7 Perguntas | Nenhum (sempre aberto) | Acesso constante |
| Seletor de Perfil | Nenhum (sempre aberto) | Navegação principal |
| Variações por porte/setor | `<!-- markmap: fold -->` | Mostrar só se aplicável |

---

## 7. SISTEMA DE NOTAÇÃO VISUAL

### Ícones para Navegação Rápida

```
🎯 Regra de Ouro / Objetivo
⚡ Perguntas Obrigatórias
📊 Perfil do Entrevistado
⏱️ Tempo / Checklist
📋 Bloco Temático
🟢 Adotante Pleno
🔴 Não-Adotante Consciente
🟡 Experimentador / Usuário Limitado
💬 Explicação para Entrevistado
🏢 Variação por Porte
🏭 Variação por Setor
⚠️ Alerta / Atenção / Pular
✓ Item Coberto
☐ Pendente de Verificação
🔗 Conexão / Link
📐 Adaptação / Customização
```

### Tags de Construtos UTAUT

```
[PE] Performance Expectancy (Benefícios percebidos)
[EE] Effort Expectancy (Facilidade/Dificuldade)
[SI] Social Influence (Influência Social)
[FC] Facilitating Conditions (Condições Facilitadoras)
[OE1] Objetivo Específico 1 (Práticas)
[OE2] Objetivo Específico 2 (Impactos)
[OE3] Objetivo Específico 3 (Fatores Determinantes)
```

### Código de Cores (Visual)

```markdown
- 🔴 **Crítico/Obrigatório**: Perguntas que não podem ser puladas
- 🟡 **Condicional**: Usar apenas se condição X for atendida
- 🟢 **Recomendado**: Explorar se tempo permitir
- ⚪ **Opcional**: Aprofundamento para categorias emergentes
```

---

## 8. MÓDULOS ESPECIAIS

### 8.1 Troubleshooting Rápido (Sidebar)

```markdown
## ⚠️ SE ALGO DER ERRADO

### Ela não entende IA?
**Ação:** Mostrar no celular
- Abrir ChatGPT
- Pedir pra escrever sobre produto dela
- Mostrar resultado

### Ela desvia pra outro assunto (ex: tráfego pago)?
**Ação:** Refocar
- "Entendi, mas queria focar em IA pra criar conteúdo. Tipo ChatGPT. Conhece?"

### Ela responde "não sei" sempre?
**Ação:** Usar cenário concreto
- "Segunda de manhã, sem ideia pro post. Se ferramenta te desse 3 ideias em 10 seg, usaria?"

### Entrevista desviou muito?
**Ação:** Consultar checklist
- Olhar checklist das 7 perguntas
- Identificar o que falta
- "Agora queria fazer perguntas específicas sobre..."

### Resposta vaga?
**Ação:** Aprofundar
- "Por quê?"
- "Me dá um exemplo?"
```

### 8.2 Lembretes Importantes

```markdown
## 💡 LEMBRE-SE!

- ✓ LIMITE Rapport a 15 min, depois siga roteiro
- ✓ Se ela menciona PROBLEMA → ANOTE e conecte com IA
- ✓ Se resposta VAGA → "Por quê?" ou "Me dá exemplo?"
- ✓ GRAVE ÁUDIO (não confie só em anotações)
- ✓ Não-adotantes são TÃO valiosos quanto adotantes
- ✓ Objetivo: ENTENDER, não CONVENCER
```

### 8.3 Timer Visual

```markdown
## ⏱️ TEMPO IDEAL (50-70 min total)

### Bloco 1: Rapport
- ⏰ 10-15 min
- 🎯 Estabelecer confiança
- 📊 Capturar dados demográficos

### Bloco 2: Práticas
- ⏰ 15-20 min
- 🎯 Mapear uso atual de IA

### Bloco 3: Impactos
- ⏰ 15-20 min
- 🎯 PE + EE (UTAUT)

### Bloco 4: Influências
- ⏰ 10-15 min
- 🎯 SI (UTAUT)

### Bloco 5: Barreiras
- ⏰ 15-20 min
- 🎯 FC (UTAUT)

### Bloco 6: Reflexões
- ⏰ 5-10 min
- 🎯 Categorias emergentes

### Margem de Manobra
- 🔄 10-15 min para aprofundamento
```

---

## 9. ESTRUTURA DE ARQUIVOS RECOMENDADA

```
📁 Markmap_Entrevista/
│
├── 📄 entrevista_markmap.md
│   └── Arquivo principal com estrutura completa
│
├── 📄 cheat_sheet_layer.md (opcional)
│   └── Versão ultra-simplificada (apenas 7 perguntas + troubleshooting)
│
├── 📄 README.md
│   └── Instruções de uso e navegação
│
├── 📁 exports/
│   ├── entrevista_markmap.html
│   │   └── Versão interativa para navegador (offline-ready)
│   ├── entrevista_markmap.svg
│   │   └── Backup estático visual
│   └── entrevista_markmap.pdf
│       └── Versão imprimível de emergência
│
└── 📁 docs/
    ├── PLANO_Markmap_Roteiro_Entrevista.md
    │   └── Este documento
    └── markmap_manual.md
        └── Documentação técnica do Markmap
```

---

## 10. WORKFLOW DE CONSTRUÇÃO (Passo a Passo)

### FASE 1: Estrutura Base (1-2h)

**Entregável:** Skeleton navegável com cabeçalho e árvore principal

1. ✓ Criar arquivo `entrevista_markmap.md`
2. ✓ Adicionar frontmatter com configurações
3. ✓ Criar cabeçalho H1 principal
4. ✓ Inserir Regra de Ouro (sempre visível)
5. ✓ Inserir 7 Perguntas Obrigatórias (sempre visível)
6. ✓ Criar Seletor de Perfil com 3 ramos
7. ✓ Criar esqueleto dos 6 blocos (apenas títulos)
8. ✓ Adicionar Timer Visual
9. ✓ Adicionar Checklist
10. ✓ Testar visualização básica

### FASE 2: População de Conteúdo (3-4h)

**Entregável:** Roteiro completo transcrito e estruturado

#### Bloco 1: Rapport e Caracterização
11. ✓ Transcrever perguntas 1.1-1.3 (universais)
12. ✓ Adicionar variações por porte (micro/média)
13. ✓ Aplicar `<!-- markmap: fold -->` nas variações

#### Bloco 2: Práticas de Marketing Digital
14. ✓ Transcrever perguntas 2.1-2.2 (universais)
15. ✓ Criar ramo 🟢 Adotantes (2.3-2.6)
16. ✓ Criar ramo 🔴 Não-Adotantes (2.7-2.10)
17. ✓ Criar ramo 🟡 Experimentadores (2.11-2.13)
18. ✓ Adicionar variações por setor
19. ✓ Aplicar `<!-- markmap: foldAll -->` nos ramos específicos

#### Bloco 3: Impactos Percebidos
20. ✓ Criar ramo 🟢 Adotantes (3.1-3.5) - PE/EE realizados
21. ✓ Criar ramo 🔴 Não-Adotantes (3.6-3.10) - PE/EE projetados
22. ✓ Criar ramo 🟡 Experimentadores (3.11-3.12)
23. ✓ Adicionar probes estruturados (Huang & Rust)
24. ✓ Aplicar magic comments

#### Bloco 4: Influências Sociais e do Ambiente
25. ✓ Transcrever perguntas 4.1-4.4 (universais - SI)
26. ✓ Adicionar probes sobre concorrentes/pares
27. ✓ Marcar construto [SI] explicitamente

#### Bloco 5: Condições Facilitadoras e Barreiras
28. ✓ Transcrever perguntas 5.1-5.4 (universais - FC)
29. ✓ Adicionar pergunta 5.5 (cultura organizacional)
30. ✓ Criar seção 5.6 (barreiras específicas não-adotantes)
31. ✓ Adicionar variações por porte
32. ✓ Marcar construto [FC] explicitamente

#### Bloco 6: Reflexões Finais
33. ✓ Transcrever perguntas 6.1-6.4 (universais)
34. ✓ Marcar como abertura para categorias emergentes

### FASE 3: Adaptações e Variações (2h)

**Entregável:** Customizações por contexto implementadas

#### Variações por Porte
35. ✓ Revisar todas as variações para microempresas
36. ✓ Revisar todas as variações para médias empresas
37. ✓ Garantir que estão marcadas com 🏢 e `<!-- markmap: fold -->`

#### Variações por Setor
38. ✓ Revisar todas as variações para setor de serviços
39. ✓ Revisar todas as variações para setor industrial
40. ✓ Garantir que estão marcadas com 🏭 e `<!-- markmap: fold -->`

#### Probes Estruturados
41. ✓ Inserir taxonomia Davenport (Task Automation, Context Awareness, Decision Support)
42. ✓ Inserir taxonomia Huang & Rust (Mechanical/Thinking/Feeling AI)
43. ✓ Adicionar [Capturar: ...] em cada pergunta relevante

### FASE 4: Elementos de Usabilidade (1-2h)

**Entregável:** Ferramentas de apoio durante entrevista

44. ✓ Criar módulo de Troubleshooting (⚠️ SE ALGO DER ERRADO)
45. ✓ Criar tabela de Conexões Problema-IA (🔗)
46. ✓ Criar Checklist interativo das 7 perguntas (☐/✓)
47. ✓ Criar seção "Como Explicar IA em 30seg" (💬)
48. ✓ Criar seção "Lembretes Importantes" (💡)
49. ✓ Adicionar Timer Visual detalhado (⏱️)

### FASE 5: Refinamento (1h)

**Entregável:** Markmap otimizado e testado

50. ✓ Revisar hierarquia (máximo 6 níveis)
51. ✓ Aplicar magic comments estrategicamente
   - `<!-- markmap: foldAll -->` em variações por perfil
   - `<!-- markmap: fold -->` em probes extensos
   - Nenhum comment em: Regra de Ouro, 7 Perguntas, Seletor
52. ✓ Testar navegação por perfil (3 cenários)
   - Cenário 1: Adotante Pleno de microempresa de serviços
   - Cenário 2: Não-Adotante de média empresa industrial
   - Cenário 3: Experimentador de pequena empresa
53. ✓ Validar completude contra roteiro PDF original (21 páginas)
54. ✓ Verificar que todos os construtos UTAUT estão mapeados
55. ✓ Ajustar `colorFreezeLevel` e `initialExpandLevel` para usabilidade
56. ✓ Exportar para HTML (funcional offline)
57. ✓ Exportar para SVG (backup estático)

### FASE 6: Documentação e Entrega (30min)

**Entregável:** Pacote completo pronto para uso

58. ✓ Criar README.md com instruções de uso
59. ✓ Documentar atalhos de navegação
60. ✓ Criar guia rápido de símbolos e cores
61. ✓ Preparar checklist de pré-entrevista

### FASE 7: Validação em Campo (pós-criação)

**Entregável:** Markmap validado empiricamente

62. ☐ Testar em 1-2 entrevistas piloto
63. ☐ Anotar pontos de fricção na navegação
64. ☐ Identificar perguntas que ficaram "escondidas"
65. ☐ Ajustar profundidade de fold baseado em uso real
66. ☐ Otimizar ordem das perguntas se necessário
67. ☐ Versão 2.0 com ajustes de campo

---

## 11. BENEFÍCIOS ESPERADOS

### Para a Condução da Entrevista

✅ **Redução de tempo de consulta**
- De folhear 21 páginas → 3 cliques no markmap
- Tempo economizado: ~30-40 segundos por consulta
- Em 10 consultas/entrevista: 5-7 minutos economizados

✅ **Garantia de cobertura**
- 7 perguntas obrigatórias sempre visíveis
- Checklist interativo para marcar progresso
- Impossível esquecer construtos UTAUT

✅ **Adaptação dinâmica ao perfil**
- Identificou Adotante? → Ramo verde se expande
- Identificou Não-Adotante? → Ramo vermelho se expande
- Sem perda de tempo com perguntas não aplicáveis

✅ **Visualização de progresso**
- Checklist mostra o que falta cobrir
- Timer visual indica se está no ritmo
- Fácil identificar se algum bloco foi negligenciado

### Para o Rigor Acadêmico

✅ **Alinhamento teórico mantido**
- Construtos UTAUT [PE][EE][SI][FC] marcados explicitamente
- Taxonomias (Huang & Rust, Davenport) integradas nos probes
- Rastreabilidade com numeração original (2.3, 3.7, etc.)

✅ **Facilitação de análise pós-entrevista**
- "Na pergunta 3.7 [EE], o entrevistado mencionou..."
- Fácil mapear respostas para framework teórico
- Categorias emergentes capturadas no Bloco 6

### Para a Experiência do Pesquisador

✅ **Recuperação rápida de desvios**
- Módulo de troubleshooting acessível a qualquer momento
- Tabela de conexões problema-IA para pivôs naturais
- Lembretes de boas práticas sempre visíveis

✅ **Portabilidade e confiabilidade**
- HTML funciona offline (importante se conexão instável em Capivari)
- Visualização em tablet durante entrevista presencial
- SVG imprimível como backup de emergência

✅ **Redução de carga cognitiva**
- Não precisa memorizar sequência de 6 blocos
- Não precisa lembrar de todas as variações por perfil/porte/setor
- Foco na escuta ativa, não na gestão do roteiro

---

## 12. CONSIDERAÇÕES ESPECIAIS PARA SEU CONTEXTO

### Contexto de Pesquisa Acadêmica (Mestrado MUST)

**Rastreabilidade Metodológica**
- Manter numeração original do roteiro (2.3, 3.4, etc.)
- Facilitar citação nas transcrições: "Em 3.7 [EE], Entrevistado A relatou..."
- Permitir cruzamento direto com tabela de operacionalização UTAUT

**Rigor Teórico**
- Construtos UTAUT visíveis mas não intrusivos para o entrevistado
- Notas sobre taxonomias (Huang & Rust / Davenport) em tooltips colapsáveis
- Justificativa de cada pergunta acessível via probes estruturados

**Replicação e Transparência**
- Roteiro completo exportável para auditoria
- Estrutura permite replicação por outros pesquisadores
- Markdown versionável (controle de mudanças via Git)

### Contexto de Campo (Capivari - Pequenos Empresários)

**Linguagem Acessível**
- Preservar coloquialismo do cheat sheet: "saca?", "tipo estagiário de graça"
- Evitar jargão acadêmico nas perguntas diretas
- Explicação de IA em linguagem simples sempre disponível (💬)

**Troubleshooting Prático**
- Adaptado para realidade de pequenos empresários
- Cenários concretos ("Segunda sem ideia de post...")
- Demonstração visual via celular se necessário

**Sensibilidade ao Tempo**
- Empresários têm agenda apertada
- Timer visual ajuda a respeitar compromisso de 50-70 min
- Opção de "fast-track" se entrevista precisa ser encurtada

### Versatilidade de Uso

**Multiplataforma**
- VSCode (desenvolvimento)
- Navegador web (uso em campo - HTML export)
- Tablet/iPad (visualização durante entrevista presencial)
- Impressão (SVG/PDF como backup absoluto)

**Offline-Ready**
- HTML exportado funciona sem internet
- Crucial para entrevistas em locais com conexão instável
- Todos os recursos (fold/unfold, zoom, pan) funcionam offline

**Adaptável**
- Fácil adicionar novas perguntas emergentes
- Possível criar versões customizadas por setor específico
- Markdown permite edição sem ferramentas especiais

---

## 13. MÉTRICAS DE SUCESSO DO MARKMAP

### Quantitativas

| Métrica | Meta | Como Medir |
|---------|------|------------|
| Tempo de consulta ao roteiro | < 30 seg por consulta | Cronometrar durante piloto |
| Cobertura das 7 perguntas | 100% | Checklist ao final |
| Cobertura dos 4 construtos UTAUT | 100% | Revisão de transcrição |
| Duração total da entrevista | 50-70 min | Gravação de áudio |
| Desvios do roteiro | < 3 por entrevista | Anotação do pesquisador |

### Qualitativas

| Aspecto | Critério de Sucesso |
|---------|---------------------|
| Navegabilidade | Pesquisador encontra perguntas sem hesitação |
| Adaptabilidade | Transição entre perfis é fluida |
| Completude | Nenhuma pergunta do PDF original foi perdida |
| Usabilidade | Não atrapalha rapport com entrevistado |
| Confiabilidade | Zero falhas técnicas (offline-ready) |

---

## 14. PRÓXIMOS PASSOS RECOMENDADOS

### Opção A: Implementação Completa Imediata
**Tempo estimado:** 6-8 horas
**Entrega:** Markmap 100% funcional com todos os 6 blocos

**Quando escolher:**
- Você tem tempo disponível nas próximas 1-2 semanas
- Quer ferramenta completa antes da primeira entrevista
- Prefere fazer 1 grande sprint de trabalho

### Opção B: Implementação em Fases (Recomendado)
**Fase 1 - Protótipo (2h):** Estrutura + 7 perguntas + Bloco 1
**Fase 2 - MVP (4h):** Adicionar Blocos 2-3 (mais complexos)
**Fase 3 - Completo (2h):** Adicionar Blocos 4-6
**Fase 4 - Polish (1h):** Troubleshooting + Refinamentos

**Quando escolher:**
- Quer validar abordagem antes de investir tempo total
- Prefere feedback incremental
- Tem disponibilidade espaçada ao longo de várias semanas

### Opção C: Exemplo Funcional Primeiro
**Tempo estimado:** 1 hora
**Entrega:** Bloco 2 ou 3 completamente implementado (demonstração)

**Quando escolher:**
- Quer "sentir" como ficará antes de decidir
- Precisa apresentar para orientador/banca
- Quer avaliar viabilidade técnica

---

## 15. DECISÃO NECESSÁRIA

**Para prosseguir, você precisa escolher:**

1. **Qual opção de implementação?** (A, B ou C acima)

2. **Prioridade de features?**
   - [ ] Todas as features do plano
   - [ ] Focar em navegação por perfil (core)
   - [ ] Focar em troubleshooting (usabilidade campo)
   - [ ] Versão minimalista primeiro

3. **Formato de entrega preferencial?**
   - [ ] Apenas `.md` (você exporta depois)
   - [ ] `.md` + `.html` (pronto para usar offline)
   - [ ] Pacote completo com README e documentação

4. **Quer alguma customização adicional?**
   - [ ] Esquema de cores diferente
   - [ ] Níveis de expansão inicial diferentes
   - [ ] Módulos adicionais não previstos

---

## 16. RECURSOS ADICIONAIS

### Documentação Técnica
- [Markmap Official Docs](https://markmap.js.org/)
- [Markdown Guide](https://www.markdownguide.org/)
- VSCode Extension: `gera2ld.markmap-vscode`

### Exemplos Inspiradores
- [Markmap React Demo](https://stackblitz.com/edit/markmap-react)
- [Markmap Vue Demo](https://stackblitz.com/edit/markmap-vue)

### Ferramentas Complementares
- **Obsidian**: Editor Markdown com preview de markmap
- **Typora**: Editor WYSIWYG para Markdown
- **Markmap CLI**: Para export automatizado em batch

---

## RESUMO EXECUTIVO

Este plano transforma seu roteiro acadêmico de 21 páginas em um **markmap hierárquico e interativo** que:

1. **Prioriza** as 7 perguntas obrigatórias do cheat sheet (sempre visíveis)
2. **Adapta-se** dinamicamente ao perfil do entrevistado (Adotante/Não-Adotante/Experimentador)
3. **Organiza** os 6 blocos temáticos com navegação intuitiva e fold estratégico
4. **Integra** troubleshooting prático e ferramentas de conexão problema-IA
5. **Garante** cobertura completa dos construtos UTAUT (PE/EE/SI/FC)
6. **Mantém** rigor acadêmico sem sacrificar usabilidade de campo
7. **Funciona** offline em múltiplas plataformas (HTML, tablet, impresso)

**Resultado esperado:**
Ferramenta que reduz tempo de consulta em 80%, garante cobertura teórica de 100%, e melhora experiência tanto do pesquisador quanto do entrevistado.

---

**Status:** Plano aprovado. Aguardando decisão de implementação.
**Próximo passo:** Escolher Opção A, B ou C e iniciar construção.

---

*Documento criado em 2025-11-12 por Eduardo Maia | Mestrado MUST*
*Versão: 1.0*
