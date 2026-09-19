# 🐧 Linux na Pratica

<p align="center">
  <b>Caderno temático e guia prático de comandos Linux, terminal, grep e shell script.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen?style=flat-square" alt="Status">
  <img src="https://img.shields.io/badge/Platform-Linux-orange?style=flat-square&logo=linux" alt="Platform">
  <img src="https://img.shields.io/badge/Shell-Bash-blue?style=flat-square&logo=gnu-bash" alt="Bash">
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=flat-square" alt="License">
</p>

---

## 📋 Contexto e Objetivos

O ecossistema Linux é o alicerce da infraestrutura moderna de tecnologia — sustentando servidores em nuvem, ambientes de containers, ferramentas DevOps e sistemas corporativos de missão crítica. 

O objetivo principal deste projeto é transpor a barreira entre a teoria de sistemas operacionais e a execução prática no dia a dia, servindo como um caderno de estudos estruturado.

### Objetivos Específicos de Estudo:
1. **Domínio da Linha de Comando (CLI):** Navegação eficiente no sistema de arquivos, manipulação de fluxos de dados e busca avançada de padrões com `grep`.
2. **Conectividade e Acesso Remoto:** Práticas seguras de conexão via `ssh` e diagnósticos iniciais de rede.
3. **Automação com Shell Scripting:** Criação de scripts básicos e intermediários para otimização de tarefas repetitivas e rotinas de sistema.
4. **Administração e Referência Técnica:** Utilização de documentações oficiais de distribuições corporativas e comunitárias (Ubuntu e Red Hat).

---

## 📚 Curadoria de Fontes (NotebookLM)

Para o embasamento teórico e prático deste caderno, foram cadastradas e indexadas **14 fontes abertas** no workspace do NotebookLM, divididas entre guias definitivos, folhas de consulta e documentações oficiais:

1. **Guias Didáticos e Manuais de Referência:**
   * *Guia Foca Linux* & *GuiaFoca — Site Oficial*
   * *Bash Linux - Guia Básico de Comandos e Exemplos de Uso*
   * *Os comandos Linux mais usados*
2. **Busca, Filtragem e Conectividade:**
   * *Como usar o comando grep no Linux? Exemplos de uso*
   * *Folha de Consulta de Comandos Linux - Arquivos, grep e ssh*
3. **Shell Scripting e Automação:**
   * *Guia de sobrevivência Bash e Shell Script (Sério!) – Otávio Miranda*
   * *Research report: Comandos Práticos e Shell Scripting no Linux*
   * *Shell script: um guia básico – Diego Mariano*
   * *Tutorial de Shell Script | Lucas Possatti*
4. **Visão Institucional e Enterprise:**
   * *O que é Linux? | IBM*
   * *O que é Linux? | Oracle Brasil*
   * *Official Ubuntu Documentation*
   * *Red Hat Enterprise Linux*

---

## ⚙️ Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

O mercado valoriza o raciocínio por trás dos resultados. Abaixo está documentado um exemplo de refinamento de prompt utilizado durante a extração de conhecimento:

* **Tentativa 1 (Prompt Inicial):** 
  > *"Como filtrar textos no Linux?"*
* **Resultado Obtido:** Uma explicação superficial sobre o comando `grep`, sem exemplos práticos de expressões regulares ou casos de uso em logs do sistema.
* **A Cicatriz / Dificuldade:** O prompt inicial não trazia o contexto de troubleshooting necessário para buscar padrões complexos em arquivos de log extensos.
* **Prompt Refinado (Estratégico):**
  > *"Atue como um Administrador de Sistemas Sênior. Utilizando as referências de manipulação de texto e grep, explique como estruturar uma busca avançada ignorando maiúsculas/minúsculas, exibindo o número da linha e extraindo contexto (linhas antes e depois) em logs de erro. Forneça exemplos práticos de sintaxe."*
* **Aprendizado Consolidado:** O uso de parâmetros como `-i`, `-n`, `-C` e o entendimento de pipes (`|`) tornaram a extração de informações de logs muito mais ágil e precisa.

*(Mais detalhes sobre o histórico de interações e troubleshooting encontram-se na pasta [`/prompts`](./prompts))*

---

## 📂 Estrutura do Repositório

```text
/
├── README.md               # Contexto, objetivos e visão geral do projeto
├── fontes/                 # Referências e links das fontes abertas indexadas
├── prompts/                # Registro de engenharia de prompts e cicatrizes
└── miniguia/               # Entrega final consolidada
    ├── resumos.md          # Resumos estruturados do assunto
    ├── glossario.md        # Glossário com os principais conceitos aprendidos
    └── prompts_uteis.md    # Conjunto de prompts reutilizáveis para revisões
