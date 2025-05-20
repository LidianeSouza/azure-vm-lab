# 💻 Laboratório Prático: Criação e Configuração de Máquinas Virtuais no Microsoft Azure

Este repositório documenta minha experiência prática com a criação e configuração de máquinas virtuais (VMs) na plataforma de nuvem Microsoft Azure. O objetivo é compartilhar o passo a passo, aprendizados, dicas e capturas de tela do processo.

## 🗂️ Índice

- [🎯 Objetivo](#-objetivo)  
- [🧱 Etapas Realizadas](#-etapas-realizadas)  
  - [1. Acesso ao Portal](#1-acesso-ao-portal)  
  - [2. Criação da Máquina Virtual](#2-criação-da-máquina-virtual)  
  - [3. Configurações de Rede](#3-configurações-de-rede)  
- [📸 Capturas de Tela](#-capturas-de-tela)  
  - [`/images/vm-criacao/`](#imagesvm-criacao)  
  - [`/images/vm-parada/`](#imagesvm-parada)  
- [💡 Minhas Anotações e Dicas](#-minhas-anotações-e-dicas)  
  - [🔧 Configurações](#-configurações)  
  - [🔐 Segurança](#-segurança)  
  - [💸 Custo](#-custo)  
- [🔗 Recursos que Utilizei](#-recursos-que-utilizei)  
- [✅ Conclusão](#-conclusão)  
- [🔗 Link do Repositório](#-link-do-repositório)

---

## 🎯 Objetivo

- Criar uma máquina virtual no Azure  
- Configurar suas propriedades básicas (tamanho, usuário, rede, etc.)  
- Documentar o processo, desafios e boas práticas para fins de estudo e referência futura  

---

## 🧱 Etapas Realizadas

### 1. Acesso ao Portal
Acessei o [portal do Azure](https://portal.azure.com) e, após fazer login, iniciei o processo de criação da VM clicando em **"Criar um recurso" > "Máquina Virtual"**.

### 2. Criação da Máquina Virtual
Durante o processo, configurei os seguintes parâmetros:

- **Grupo de Recursos:** criei um novo para organização  
- **Nome da VM:** `lab-myVM`  
- **Região:** selecionei `Brazil South`  
- **Imagem:** optei por `Windows Server 2025 Datacenter: Azure Edition - x64 Gen2`  
- **Tamanho da VM:** escolhi o tipo B1s (Standard_B1s)  
- **Autenticação:** criei usuário e senha (labuser - ****)  

### 3. Configurações de Rede
- Configurei IP público  (Permitir portas selecionadas)
- Adicionei regras de entrada para RDP (porta 3389)  

---

## 📸 Capturas de Tela

Durante o processo, capturei diversas telas para registrar cada etapa da criação e configuração da máquina virtual. Todas as imagens estão organizadas na pasta [`/images`](./images), divididas conforme as fases do laboratório:

### 📂 `/images/vm-criacao/`
Contém **9 capturas de tela**, numeradas de `1.png` a `9.png`, que ilustram todas as etapas do processo de criação da VM no portal Azure — **desde a configuração básica até a revisão final e a criação da máquina virtual**.

### 📂 `/images/vm-parada/`
Contém as capturas de tela **1.png** e **2.png**, que demonstram o processo de **parar/desligar a VM** após a conclusão do laboratório — uma etapa importante para evitar cobranças indevidas e liberar os recursos utilizados.

Essas imagens documentam visualmente todas as etapas realizadas e servem como material de referência para futuras implementações ou revisões.

---

## 💡 Minhas Anotações e Dicas

### 🔧 Configurações
- Escolhi o tamanho **B1s**, uma opção de baixo custo (e elegível para uso gratuito), ideal para testes e estudos  
- Criei um novo **grupo de recursos** chamado `laboratorio-myVM_group`, o que facilita a organização e, principalmente, a **remoção de todos os recursos associados de forma centralizada** ao final do laboratório  

### 🔐 Segurança
- Abri apenas as portas necessárias (no caso, a **porta 3389** para RDP)  
- Usei **autenticação via usuário e senha**, conforme exigido pela imagem do Windows Server   

### 💸 Custo
- Após finalizar o laboratório, **parei a VM** para evitar cobranças  
- Como boa prática, **excluí todos os recursos criados** para garantir que não haja custos residuais  

---

## 🔗 Recursos que Utilizei

- [Documentação oficial do Azure](https://learn.microsoft.com/pt-br/azure/)  
- [Guia de criação de VMs](https://learn.microsoft.com/pt-br/azure/virtual-machines/)  
- **ChatGPT** — usei para esclarecimento de dúvidas, estruturação e revisão do conteúdo do laboratório  

---

## ✅ Conclusão

Realizar esse laboratório foi essencial para consolidar meu entendimento sobre a criação e configuração de máquinas virtuais no Azure. Foi tudo muito novo para mim, então utilizei o apoio do **ChatGPT** para tirar dúvidas, estruturar o conteúdo e organizar as etapas do processo. Isso facilitou muito meu aprendizado e me ajudou a documentar tudo com clareza.

Estou animada para aplicar esse conhecimento em projetos reais e explorar ainda mais recursos da Azure em futuros laboratórios.

---

## 🔗 Link do Repositório

> [https://github.com/LidianeSouza/azure-vm-lab](https://github.com/LidianeSouza/azure-vm-lab)


