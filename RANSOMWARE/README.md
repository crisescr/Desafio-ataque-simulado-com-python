# Simulação Educacional: Ransomware & Descriptografador (Python)

**Resumo**  
Este repositório contém uma simulação educacional de ransomware e seu descriptografador correspondente, implementados em Python. Tudo foi desenvolvido para ser executado **apenas** em um ambiente de teste controlado (pasta `test_files` dentro do repositório, em máquina virtual isolada).

---

## ⚠️ Aviso de Segurança
- **Executar apenas em ambiente isolado (VM) e com backups.**  
- **Não execute em máquinas de produção, redes corporativas ou com dados reais.**  
- Estes scripts são educativos e não incluem técnicas furtivas de propagação. Use-os apenas para aprendizado.

---

## O que o Ransomware faz (visão geral)
- Gera uma chave de criptografia (`chave.key`) usando `cryptography.Fernet`.
- Procura por arquivos **dentro da pasta `test_files`** e ignora arquivos essenciais do projeto.
- Criptografa cada arquivo encontrado (sobrescrevendo ou gerando `.enc`, dependendo da versão usada).
- Cria um arquivo de aviso `LEIA ISSO.txt` indicando que os arquivos foram criptografados (simulação).

**Objetivo pedagógico:** demonstrar o fluxo de ataque (geração de chave → criptografia de arquivos → nota de resgate) e permitir estudar detecção e resposta.

---

## O que o Descriptografador faz
- Lê a chave gerada (`chave.key`).
- Percorre `test_files` e descriptografa os arquivos criptografados, restaurando o conteúdo original.
- Registra erros caso a chave esteja ausente ou arquivos estejam corrompidos.

---

## Como testar (ambiente seguro)
1. Crie uma pasta com o nome ex: Simulacao_Ransomware e dentro cole os arquivos codigo ransomware.py e descriptografar.py
2. Dentro crie/prepare a pasta `test_files` com alguns arquivos de exemplo:
   ```bash
   mkdir test_files
   echo "teste" > test_files/arquivo1.txt
