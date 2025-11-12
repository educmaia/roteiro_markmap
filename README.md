# 🎤 Roteiro de Entrevista - Markmap Interativo

## 📌 Sobre este Projeto

Este repositório contém o roteiro de entrevista semiestruturada transformado em **markmap interativo** para facilitar a condução de entrevistas em campo sobre adoção de IA no marketing por PMEs.

**Pesquisador:** Eduardo Camargo Maia
**Programa:** Mestrado MUST
**Tema:** Não-adotantes de IA Generativa no Marketing Digital

---

## 📁 Estrutura de Arquivos

```
roteiro_markmap/
├── entrevista_markmap.md          ← ARQUIVO PRINCIPAL (roteiro interativo)
├── PLANO_Markmap_Roteiro_Entrevista.md  ← Plano de arquitetura
├── _Roteiros/
│   └── Cheat_Sheet_1_Pagina.txt   ← Guia rápido de 1 página
├── Roteiro Entrevista.pdf         ← Roteiro acadêmico completo (21 páginas)
├── TCF - Eduardo Camargo Maia.pdf ← Termo de Consentimento
└── README.md                       ← Este arquivo
```

---

## 🚀 Como Usar o Markmap

### Opção 1: VSCode (Recomendado para Desenvolvimento)

1. **Instale a extensão Markmap:**
   - Abra VSCode
   - Vá em Extensions (Ctrl+Shift+X)
   - Busque: `markmap`
   - Instale: **Markmap** (by gera2ld)

2. **Visualize o markmap:**
   - Abra o arquivo `entrevista_markmap.md`
   - Clique com botão direito → **Open as Markmap**
   - Ou use o atalho: `Ctrl+Shift+P` → "Markmap: Open"

### Opção 2: Online (Rápido para Testar)

1. Acesse: https://markmap.js.org/repl
2. Copie todo o conteúdo de `entrevista_markmap.md`
3. Cole no editor online
4. Visualize o mapa interativo

### Opção 3: Exportar HTML (Uso em Campo - Offline)

1. No VSCode, com o markmap aberto:
   - `Ctrl+Shift+P` → "Markmap: Export"
   - Escolha formato: **HTML**
   - Salve em `exports/entrevista_markmap.html`

2. **Vantagem:** Arquivo HTML funciona offline em qualquer navegador ou tablet!

### Opção 4: CLI (Para Gerar Arquivos em Lote)

```bash
# Instalar markmap-cli
npm install -g markmap-cli

# Gerar HTML
markmap entrevista_markmap.md -o exports/entrevista_markmap.html

# Gerar SVG (backup estático)
markmap entrevista_markmap.md -o exports/entrevista_markmap.svg
```

---

## 🎯 Navegação no Markmap

### Elementos Sempre Visíveis (Não Colapsam)

- 🎯 **Regra de Ouro:** PROBLEMA → EXPLICAR IA → PERGUNTAR
- ⚡ **7 Perguntas Obrigatórias:** Núcleo da entrevista
- 💬 **Como Explicar IA:** Roteiro de 30 segundos
- 🔗 **Conectar Problema com IA:** Tabela de referência rápida
- ⏱️ **Timer da Entrevista:** Gestão de tempo por bloco
- ✓ **Checklist de Cobertura:** Marcar o que foi coberto

### Navegação por Perfil

O markmap se adapta ao perfil identificado:

- 🟢 **Adotante Pleno:** Seguir rota VERDE (Blocos 2.3-2.6, 3.1-3.5)
- 🔴 **Não-Adotante Consciente:** Seguir rota VERMELHA (Blocos 2.7-2.10, 3.6-3.10)
- 🟡 **Experimentador:** Seguir rota AMARELA (Blocos 2.11-2.13, 3.11-3.12)

### Controles Interativos

- **Clique em nó:** Expande/colapsa seção
- **Zoom:** Scroll do mouse ou pinça (tablet)
- **Pan:** Arrastar com mouse/dedo
- **Foco:** Clique duplo centraliza nó

---

## 📋 Estrutura do Roteiro (6 Blocos)

| Bloco | Tema | Tempo | Construtos UTAUT |
|-------|------|-------|------------------|
| **1** | Rapport e Caracterização | 10-15 min | Dados demográficos |
| **2** | Práticas de Marketing Digital | 15-20 min | Contexto |
| **3** | Impactos Percebidos | 15-20 min | PE + EE |
| **4** | Influências Sociais | 10-15 min | SI |
| **5** | Condições Facilitadoras e Barreiras | 15-20 min | FC |
| **6** | Reflexões Finais | 5-10 min | Categorias emergentes |

**Tempo total:** 50-70 minutos

---

## 🔑 Conceitos Importantes

### Construtos UTAUT

- **[PE] Performance Expectancy:** Benefícios percebidos/esperados
- **[EE] Effort Expectancy:** Facilidade ou dificuldade percebida
- **[SI] Social Influence:** Influência de pares, concorrentes, mercado
- **[FC] Facilitating Conditions:** Recursos disponíveis (tempo, dinheiro, suporte)

### Taxonomias Teóricas

**Davenport (Tarefas de IA):**
- Task Automation (automação)
- Context Awareness (adaptação)
- Decision Support (análise/decisão)

**Huang & Rust (Tipos de IA):**
- Mechanical AI (tarefas repetitivas)
- Thinking AI (análise de dados)
- Feeling AI (relacionamento/empatia)

---

## ✅ Checklist Pré-Entrevista

### Tecnologia
- [ ] Gravador de áudio testado e com bateria
- [ ] Backup de gravação (celular)
- [ ] Markmap acessível (tablet ou laptop)
- [ ] Termo de Consentimento impresso

### Preparação
- [ ] Revisar perfil da empresa (se disponível)
- [ ] Preparar explicação de IA de 30 segundos
- [ ] Ter ChatGPT aberto no celular (para demonstração)

### Postura
- [ ] Lembrar: objetivo é ENTENDER, não CONVENCER
- [ ] Não-adotantes são tão valiosos quanto adotantes
- [ ] Escuta ativa > seguir roteiro rigidamente

---

## 🎯 Dados Críticos a Capturar

### Essenciais
1. **Barreira Principal** (a número 1!)
2. Performance Expectancy (benefícios percebidos)
3. Effort Expectancy (facilidade percebida)
4. Social Influence (pressão de concorrentes)
5. Facilitating Conditions (recursos disponíveis)

### Complementares
- Estratégias sem IA (como faz hoje)
- Preocupação com autenticidade
- Intenção de uso futuro
- Categorias emergentes

---

## 📊 Pós-Entrevista

### Imediatamente Após
1. Verificar se gravação funcionou
2. Fazer anotações complementares (impressões, contexto)
3. Preencher checklist de cobertura
4. Classificar perfil do entrevistado
5. Identificar barreira principal

### Backup de Dados
- Transferir gravação para 2 locais diferentes
- Nomear arquivo: `Entrevista_[Empresa]_[Data]_[Perfil].mp3`
- Backup de anotações escritas

---

## 🔧 Troubleshooting Técnico

### Markmap não abre no VSCode
- Verificar se extensão está instalada e ativada
- Tentar recarregar janela: `Ctrl+Shift+P` → "Reload Window"
- Verificar se arquivo tem extensão `.md`

### Markmap está truncado
- Ajustar zoom (scroll do mouse)
- Usar pan (arrastar) para navegar
- Se necessário, ajustar `maxWidth` no frontmatter

### Ícones não aparecem
- Ícones emoji são universais, devem funcionar em qualquer sistema
- Se não aparecer, o conteúdo textual ainda é legível

### HTML offline não funciona
- Verificar se salvou com todas as dependências incorporadas
- Testar em navegador diferente (Chrome, Firefox, Edge)

---

## 📚 Referências

### Documentação Técnica
- [Markmap Official Docs](https://markmap.js.org/)
- [Markdown Guide](https://www.markdownguide.org/)

### Base Teórica
- Venkatesh et al. (2003) - UTAUT Model
- Huang & Rust (2018) - AI Service Types
- Davenport & Ronanki (2018) - AI Taxonomy

---

## 📝 Versão e Atualizações

**Versão atual:** 1.0
**Data:** 2025-11-12
**Changelog:**
- v1.0 (2025-11-12): Primeira versão do markmap interativo

---

## 📞 Contato

**Pesquisador:** Eduardo Camargo Maia
**Instituição:** Mestrado MUST
**Tema:** Adoção de IA Generativa no Marketing Digital por PMEs

---

## 📄 Licença

Este material é parte de pesquisa acadêmica de mestrado.
Uso permitido para fins educacionais e de pesquisa com devida citação.

---

**🎯 Boa entrevista!**
*Lembre-se: o objetivo é ENTENDER, não CONVENCER.*
