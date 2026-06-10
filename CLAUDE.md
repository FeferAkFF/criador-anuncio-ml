# CLAUDE.md — Marketplace Ad Creator

> Documento mestre do projeto.
> Última atualização: 2026-06-08

---

# VISÃO GERAL

Marketplace Ad Creator é uma aplicação web que gera anúncios completos para marketplaces.

Entrada:
- dados do produto
- medidas
- peso
- categoria
- imagens

Saída:
- título otimizado
- descrição otimizada
- imagens prontas para publicação

---

# CONTEXTO

Este é um produto independente da Tulele Ltda.
Não compartilha código nem repositório com outros projetos de Felipe.

Projetos paralelos existentes (não confundir):

| Projeto | Foco |
|---------|------|
| tulele-agencia- | Portal de operação de marketplace |
| felipe-automacao-sellers | Conteúdo de automação para sellers |
| **Este projeto** | Produto SaaS — gerador de anúncios |

---

# OBJETIVO PRINCIPAL

Reduzir drasticamente o tempo necessário para criar anúncios de marketplace.

---

# PROBLEMA

Sellers:
- gastam horas criando anúncios
- não dominam SEO de marketplace
- utilizam imagens ruins
- possuem baixa padronização

---

# SOLUÇÃO

Automação completa da criação de anúncios.

---

# HIERARQUIA DE DECISÃO

Ao tomar decisões técnicas:

1. Simplicidade
2. Baixo custo
3. Velocidade de entrega
4. Facilidade de manutenção
5. Escalabilidade

Nunca sacrificar simplicidade por sofisticação prematura.

---

# MVP

Escopo obrigatório:
- entrada de dados
- pesquisa de keywords
- geração de títulos
- geração de descrição
- geração de imagens
- exportação

Nada além disso sem aprovação.

---

# CONTROLE DE ESCOPO

Evitar:
- dashboards complexos
- autenticação avançada
- múltiplos planos
- analytics avançado
- integrações secundárias

Feature creep é proibido.

---

# STACK OFICIAL

Frontend:
- HTML
- CSS
- JavaScript puro

Backend:
- Vercel Functions
- Node.js

IA Texto:
- Gemini
- OpenRouter

IA Imagem:
- Pollinations (gratuito, MVP)
- Imagen 3 (qualidade superior, fase seguinte)

Keywords:
- Primeira opção: Mercado Livre Suggestions (scraping das sugestões do campo de busca)
- Segunda opção: Google Keyword Planner API
- Decisão final: pendente validação técnica — não implementar sem definir com Felipe

Hospedagem:
- Vercel

---

# EXPORTAÇÃO

Comportamento esperado ao final do fluxo:

- Título: botão copiar com um clique
- Descrição: botão copiar com um clique
- Imagens: download individual por imagem ou download em ZIP
- Nenhuma integração direta com marketplace no MVP
- O seller copia e sobe manualmente

---

# TEMPLATES DE IMAGEM (MVP)

| Template | Descrição | Prioridade |
|----------|-----------|-----------|
| Foto principal | Produto centralizado, fundo branco, sombra sutil | ⭐ MVP |
| Infográfico de medidas | Produto com setas e dimensões sobrepostas | ⭐ MVP |
| Destaque de benefícios | 3 bullets visuais ao lado do produto | Fase 2 |
| Comparativo de tamanho | Produto ao lado de objeto de referência | Fase 2 |

---

# TECNOLOGIAS PROIBIDAS

Não adicionar sem aprovação:
- React
- Next.js
- Vue
- Angular
- NestJS

---

# DEPENDÊNCIAS

Antes de instalar qualquer biblioteca:

1. Verificar se JS puro resolve.
2. Justificar necessidade.
3. Avaliar impacto futuro.

Preferir zero dependências.

---

# ARQUITETURA
