# 💻 Laboratório Prático: Criação e Configuração de Máquinas Virtuais no Microsoft Azure 

Este repositório documenta minha experiência prática com a criação e configuração de máquinas virtuais (VMs) na plataforma de nuvem Microsoft Azure. O objetivo é compartilhar o passo a passo, aprendizados, dicas e capturas de tela do processo.

---

## 🎯 Objetivo

- Criar uma máquina virtual no Azure
- Configurar suas propriedades básicas (tamanho, usuário, rede, etc.)
- Conectar-se à VM
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
- **Imagem:** optei por `Windows Server (2025 Datacenter Azure Edition)`
- **Tamanho da VM:** escolhi o tipo B1s (ideal para testes e ambientes de estudo)
- **Autenticação:** criei usuário e senha

### 3. Configurações de Rede
- Configurei IP público
- Adicionei regras de entrada para RDP (porta 3389) 

---

## 📸 Capturas de Tela

Durante o processo, capturei várias telas para registrar cada etapa da criação e configuração da máquina virtual. Todas as imagens estão organizadas na pasta [`/images`](./images), divididas conforme as fases do laboratório:

### 📂 `/images/vm-criacao/`
Contém **9 capturas de tela**, numeradas de `1.png` a `9.png`, que ilustram todas as etapas do processo de criação da VM no portal Azure — **desde a configuração básica até a revisão final e a criação da máquina virtual**.

### 📂 `/images/vm-parada/`
Contém as capturas de tela **1.png e 2.png**, que demonstram o processo de **parar/desligar a VM** após a conclusão do laboratório — uma etapa importante para evitar cobranças indevidas e liberar recursos após o uso.

Essas imagens documentam visualmente todas as etapas realizadas e servem como material de referência para futuras implementações ou revisões.

---

## 💡 Minhas Anotações e Dicas

### 🔧 Configurações
- Escolhi o tamanho **B1s**, uma opção de baixo custo (e elegível para uso gratuito), ideal para testes e estudos
- Criei um novo **grupo de recursos** chamado `lab-myVM_group`, o que facilita a organização e, principalmente, a **remoção de todos os recursos associados de forma centralizada** ao final do laboratório

### 🔐 Segurança
- Abri apenas as portas necessárias (no caso, a **porta 3389** para RDP)
- Usei **autenticação via usuário e senha**, conforme exigido pela imagem do Windows Server
- Recomendo restringir o acesso à porta RDP (3389) por faixa de IP sempre que possível, para aumentar a segurança da conexão

### 💸 Custo
- Após finalizar o laboratório, **parei a VM** para evitar cobranças
- Como boa prática, excluí todos os recursos criados para garantir que não haveria custos residuais

---

## 🔗 Recursos que Usei

- [Documentação oficial do Azure](https://learn.microsoft.com/pt-br/azure/)
- [Guia de criação de VMs](https://learn.microsoft.com/pt-br/azure/virtual-machines/)
- **ChatGPT** — usei ativamente para esclarecimento de dúvidas, estruturação e revisão do conteúdo do laboratório.
  
---

## ✅ Conclusão

Realizar esse laboratório foi essencial para consolidar meu entendimento sobre a criação e configuração de máquinas virtuais no Azure. Como sou novo nesse tema, utilizei também o apoio do **ChatGPT** para tirar dúvidas, estruturar o conteúdo e organizar as etapas do processo. Isso facilitou muito meu aprendizado e me ajudou a documentar tudo com clareza.

Este repositório servirá como material de apoio para futuras implementações em projetos mais robustos.

---

### 🔗 Link do Repositório

> [https://github.com/LidianeSouza/azure-lab-vm](https://github.com/LidianeSouza/azure-vm-lab/tree/main)
