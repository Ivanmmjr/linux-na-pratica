# 📖 Resumos Estruturados: Linux na Prática

Este documento consolida os principais tópicos estudados durante a curadoria do caderno temático, servindo como referência rápida para o uso diário do Linux.

---

## 1. Fundamentos da Linha de Comando (CLI)
A interface de linha de comando (CLI) permite controle total sobre o sistema operacional através de interações baseadas em texto.
* **Estrutura de comandos:** `comando [opções] [argumentos]`
* **Navegação básica:**
  * `pwd`: Mostra o diretório atual (*Print Working Directory*).
  * `ls -la`: Lista todos os arquivos (incluindo ocultos) em formato detalhado.
  * `cd <diretório>`: Altera o diretório de trabalho.
* **Manipulação de Arquivos e Diretórios:**
  * `mkdir -p dir/subpasta`: Cria estruturas aninhadas de diretórios.
  * `cp` / `mv`: Copiam ou movem/renomeiam arquivos.
  * `rm -rf`: Remove diretórios e arquivos recursivamente (usar com cautela extrema).

---

## 2. Manipulação de Texto e Filtragem com `grep`
O Linux segue a filosofia Unix: ferramentas pequenas que fazem bem uma única tarefa e se comunicam através de *pipes* (`|`).
* **O operador Pipe (`|`):** Redireciona a saída padrão (*stdout*) de um comando para a entrada padrão (*stdin*) de outro.
  * *Exemplo:* `history | grep apt`
* **Domínio do `grep`:** Utilizado para buscar padrões de texto.
  * `grep "erro" /var/log/syslog`: Busca linhas contendo a palavra "erro".
  * `grep -i "erro" arquivo.txt`: Ignora diferenças entre maiúsculas e minúsculas (*case-insensitive*).
  * `grep -n "config" arquivo.txt`: Exibe o número das linhas correspondentes.
  * `grep -C 3 "falha" log.txt`: Exibe 3 linhas de contexto (antes e depois) do padrão encontrado.

---

## 3. Introdução ao Shell Scripting
Automatizar tarefas repetitivas é um dos maiores superpoderes de um administrador Linux.
* **Shebang (`#!/bin/bash`):** Linha inicial obrigatória que indica qual interpretador executar o script.
* **Variáveis e Atribuição:**
  ```bash
  NOME="Administrador"
  echo "Olá, $NOME!"
