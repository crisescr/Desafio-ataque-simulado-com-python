# Projeto: Simulação de Ransomware e Keylogger em Ambiente Controlado

## 🧩 Sobre o Desafio

Este repositório foi criado como parte de um desafio prático para aplicar os conhecimentos estudados sobre o funcionamento de malwares simulados (Ransomware e Keylogger) utilizando **Python**, sempre em um ambiente **100% seguro e controlado**.

O objetivo é demonstrar, de forma educativa, como essas ameaças operam, como podem afetar sistemas e quais medidas são essenciais para mitigá-las no mundo real.

---

## 📌 Estrutura do Repositório

```
/
├── ransomware_simulado/
│   ├── codigo_ransomware.py
│   ├── codigo_decriptacao.py
│   ├── arquivos_de_teste/
│   └── imagens/
│
├── keylogger_simulado/
│   ├── keylogger.py
│   ├── envio_email.py
│   └── imagens/
│
└── README.md
```

Cada pasta contém:

* **Códigos completos** das simulações.
* **Imagens (prints)** mostrando a execução real.
* **Arquivos utilizados nos testes**, quando aplicável.

---

## 🧪 Ambiente Utilizado

Todas as simulações foram executadas em um ambiente isolado para evitar qualquer impacto no sistema principal:

* 💻 **Máquina Virtual:** Windows 10
* 📦 **Hipervisor:** VirtualBox
* 🔐 **Ambiente controlado e sem acesso a sistemas reais**

Este tipo de estudo *nunca* deve ser realizado no computador principal ou em máquinas de produção.

---

## 🕵️‍♂️ Simulação 1: Ransomware

Na pasta **/ransomware_simulado**, você encontrará:

* Script que **cripta arquivos** utilizando Python e a biblioteca `cryptography.fernet`.
* Script para **descriptografar** os arquivos.
* Arquivos de teste utilizados durante a simulação.
* Prints mostrando criptografia, descriptografia e mensagem de "resgate".

### Objetivos atingidos:

* Compreender o funcionamento básico de um ransomware.
* Simular sequestro de arquivos.
* Documentar comportamento e etapas.

---

## 🎹 Simulação 2: Keylogger

Na pasta **/keylogger_simulado**, você encontrará:

* Script que captura teclas pressionadas e salva em `.txt`.
* Versão mais "furtiva" do keylogger.
* Script opcional para **envio automático por e-mail**.
* Prints mostrando o log sendo gerado.

### Objetivos atingidos:

* Entender o funcionamento técnico de keyloggers.
* Registrar e analisar capturas de teclado.
* Documentar funcionamento e medidas defensivas.

---

## 🛡️ Medidas de Defesa e Prevenção

Além das simulações, o projeto inclui uma reflexão sobre defesa contra malwares, abordando:

* 🔒 Antivírus e detecção comportamental
* 🧱 Firewall e controle de tráfego suspeito
* 📦 Sandboxing e análise isolada
* 🧠 Conscientização e boas práticas do usuário

Essas recomendações estão descritas de forma clara dentro de cada seção de simulação.

---

## 🎯 Objetivos de Aprendizagem Alcançados

Ao concluir o desafio, foram consolidados conhecimentos como:

* Funcionamento interno de malwares simples.
* Criação de scripts educacionais em Python.
* Análise de impacto e riscos.
* Boas práticas de defesa cibernética.
* Documentação e organização de projetos no GitHub.

---

## 📂 Considerações Finais

Este projeto tem **fins exclusivamente educativos** e foi realizado **inteiramente em ambiente seguro**.
Seu propósito é compreender para defender, nunca para prejudicar.

Fique à vontade para explorar o código, estudar o comportamento e aprimorar as soluções! 🚀

