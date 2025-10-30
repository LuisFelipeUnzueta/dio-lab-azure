# 🧠 Desafio DIO: Máquinas Virtuais no Microsoft Azure

## 🧩 Etapas Realizadas

### 1️⃣ Criação do Grupo de Recursos
- Acesse o **Portal do Azure**: https://portal.azure.com  
- Crie um **Resource Group** para centralizar todos os recursos do projeto.  
- Nome sugerido: `rg-desafio-vm-azure`

### 2️⃣ Criação da Máquina Virtual
- Navegue até **Máquinas Virtuais** > **Criar** > **Máquina Virtual**.  
- Configurações utilizadas:
  - **Nome:** `vm-desafio-dio`
  - **Região:** `East US`
  - **Imagem:** `Windows Server 2022 Datacenter`
  - **Tamanho:** `Standard_B1s`
  - **Usuário administrador:** definido durante a criação  
  - **Portas abertas:** 3389 (RDP)
  - **Disco do SO:** SSD padrão  

### 3️⃣ Conexão com a VM
- Após o provisionamento, clique em **Conectar > RDP**.  
- Faça o download do arquivo `.rdp` e conecte-se via **Remote Desktop**.  
- Teste o acesso utilizando as credenciais definidas.  

### 4️⃣ Testes de Configuração
- Verifique a conectividade de rede (ping, ipconfig).  
- Acesse o **Gerenciador do Servidor** e valide os recursos provisionados.  
- (Opcional) Instale e teste serviços adicionais, como IIS.

---

## 🧾 Considerações Técnicas

- O provisionamento foi realizado utilizando o modelo **IaaS**, permitindo controle total sobre o sistema operacional.  
- A escolha da **região** impacta diretamente em **latência e custo**.  
- O uso de **Resource Groups** facilita o gerenciamento e a exclusão de recursos em massa.  
- O acesso **RDP (Remote Desktop Protocol)** foi essencial para validar a conectividade e o funcionamento da VM.  

---

## 💡 Conclusão

Este desafio proporcionou uma experiência prática completa sobre o uso de **máquinas virtuais na nuvem Azure**, consolidando conceitos de:
- Infraestrutura como Serviço (IaaS);
- Elasticidade e escalabilidade de recursos;
- Gerenciamento via portal e boas práticas de segurança.
