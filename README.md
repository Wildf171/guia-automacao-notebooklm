# Miniguia de Estudos: Automação Inteligente com Python e NotebookLM 🚀

Este repositório foi desenvolvido como parte do desafio de projeto da **DIO (Digital Innovation One)**. O objetivo é utilizar a Inteligência Artificial (NotebookLM) como uma ferramenta de aprendizagem ativa para aprofundar conhecimentos em automação de processos e ciência de dados.

## 🎯 Contexto e Objetivos
Como estudante de Ciência de Dados no 3º semestre e fundador da **Neo Desenvolver**, meu foco foi entender como escalar automações que utilizam Python, Docker e APIs de comunicação (como a Evolution API).

**Objetivos de Estudo:**
* Compreender as melhorias de performance do Python 3.11.
* Identificar boas práticas de containerização com Docker para projetos de automação.
* Explorar estratégias de manipulação de grandes volumes de dados com Pandas.

## 📚 Curadoria de Fontes
Para alimentar o NotebookLM, selecionei as seguintes fontes técnicas:
1. **Documentação Python 3.11 (What's New):** Foco em performance e novos recursos.
2. **Guia de Usuário Pandas:** Melhores práticas de manipulação de DataFrames.
3. **Docker Python Web Guide:** Estratégias para criar imagens leves e seguras.
4. **Documentação Evolution API:** Referência para integrações de mensagens.

## 🧠 Engenharia de Prompts e "Cicatrizes"
Nesta etapa, testei diferentes abordagens para extrair informações densas da IA.

* **Prompt de Teste:** "Quais as vantagens do Python para automação?"
    * *Resultado:* Resposta genérica.
* **Prompt Estratégico (O que funcionou):** "Com base nas fontes fornecidas, identifique as 3 principais dificuldades que um desenvolvedor de automação enfrenta ao escalar projetos com Python e Docker."
    * *Dificuldade Encontrada (Cicatriz):* A IA inicialmente não listava os problemas de forma direta. Precisei pedir que ela inferisse os desafios com base nas soluções (como o uso de *ExceptionGroups* e imagens *Alpine*) apresentadas nos documentos.

## 📖 Miniguia de Estudo (Entrega Final)

### Resumo Estruturado: Desafios de Escala
1. **Otimização Docker:** A necessidade de usar imagens `python:alpine` para segurança e performance, além da gestão de variáveis de ambiente com `python-dotenv`.
2. **Gargalos de Memória:** O uso de estratégias de *chunking* (processamento em partes) para grandes conjuntos de dados.
3. **Alta Simultaneidade:** A importância do `asyncio.TaskGroup` e dos novos `ExceptionGroups` do Python 3.11 para gerenciar múltiplas tarefas assíncronas sem travar o sistema.

### 📝 Glossário de Conceitos Chave
* **Faster CPython:** Iniciativa do Python 3.11 para tornar o interpretador entre 10-60% mais rápido.
* **Image Layering:** Conceito de construção de imagens Docker onde cada comando cria uma camada, exigindo rebuilds em mudanças de código.
* **ExceptionGroup:** Nova sintaxe (`except*`) para tratar várias falhas simultâneas em códigos assíncronos.

### 🛠️ Prompts Reutilizáveis para Revisão
* `"Explique como a nova funcionalidade de TaskGroup do Python 3.11 resolveria um problema de timeout em múltiplos webhooks."`
* `"Resuma as melhores práticas de segurança para Docker containers baseadas no documento enviado."`

---
Projeto desenvolvido por [William Gabriel Souza Vieira] para o Bootcamp Accenture - DIO.
