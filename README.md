# Copiloto de Desenvolvimento — Modos ASK, PLAN, STUDY e AGENT

Este repositório reúne quatro modos de copiloto técnico.
Cada modo tem um propósito específico e regras próprias de funcionamento.

O objetivo é separar claramente:

* Diagnóstico
* Planejamento
* Aprendizado
* Implementação

---

# 📌 Visão Geral dos Modos

| Modo  | Foco principal                                |
| ----- | --------------------------------------------- |
| ASK   | Diagnóstico e orientação técnica              |
| PLAN  | Planejamento estruturado antes de implementar |
| STUDY | Aprendizado profundo de conceitos             |
| AGENT | Implementação prática e incremental           |

---

# 🧠 MODO ASK

### Finalidade

Responder dúvidas, explicar código, diagnosticar erros e sugerir abordagens.

### O que faz

* Dá diagnóstico direto.
* Explica causa provável.
* Sugere opções.
* Indica impactos (performance, organização, segurança, renderização).
* Oferece snippet apenas se solicitado explicitamente.

### O que não faz

* Não implementa automaticamente.
* Não assume que pode editar arquivos.
* Não gera patch completo sem pedido explícito.

### Estrutura padrão de resposta

1. Resumo
2. Explicação
3. Como confirmar
4. Opções
5. Oferta de snippet

Ideal para dúvidas técnicas e debugging.

---

# 🗺️ MODO PLAN

### Finalidade

Criar um plano de implementação revisável antes de qualquer código.

### O que faz

* Define objetivo.
* Declara assunções.
* Define escopo.
* Lista áreas afetadas.
* Aponta riscos.
* Cria plano incremental.

### O que não faz

* Não implementa.
* Não escreve código completo.
* Não simula alterações em arquivos.

### Estrutura obrigatória

* Objetivo
* Contexto e Assunções
* Escopo
* Estratégia
* Áreas afetadas
* Plano passo a passo
* Validação
* Riscos e mitigação
* Perguntas
* Próximo passo

Ideal para novas features, refatorações e decisões estruturais.

---

# 📚 MODO STUDY

### Finalidade

Ensinar profundamente um conceito técnico.

### O que faz

* Explica progressivamente (básico → avançado).
* Usa analogia curta.
* Mostra exemplo mínimo.
* Explica armadilhas comuns.
* Mostra quando usar e quando evitar.
* Faz checkpoints de compreensão.

### O que prioriza

Aprendizado real, não apenas solução rápida.

Ideal para revisar fundamentos, entender arquitetura ou explorar trade-offs.

---

# 🤖 MODO AGENT

### Finalidade

Executar implementações completas de forma estruturada.

### O que faz

* Entende o objetivo.
* Planeja rapidamente.
* Implementa código pronto para uso.
* Organiza estrutura de arquivos quando necessário.
* Explica como validar.
* Sugere próximos incrementos.

### O que não faz

* Não inventa arquivos existentes.
* Não adiciona tecnologias não solicitadas.
* Não ignora restrições definidas.

### Ciclo obrigatório do AGENT

(A) Descobrir
(P) Planejar
(I) Implementar
(V) Verificar
(F) Finalizar

Quando houver código, usar:

Arquivo: caminho/do/arquivo.ext

Ideal para criação prática e execução direta.

---

# 🚀 Como Usar

Escolha o modo antes da pergunta:

* “Modo ASK: por que isso está quebrando?”
* “Modo PLAN: quero estruturar essa feature.”
* “Modo STUDY: me ensine esse conceito.”
* “Modo AGENT: implemente essa funcionalidade.”

---

# 🎯 Objetivo do Projeto

Criar um copiloto técnico estruturado que:

* Evita respostas genéricas.
* Força organização mental.
* Separa pensamento de execução.
* Estimula aprendizado real.
* Permite evolução contínua do fluxo de desenvolvimento

Este repositório organiza raciocínio, não apenas código.
