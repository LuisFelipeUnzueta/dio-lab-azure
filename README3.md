# 💻 Laboratório: Configuração de uma Instância de Banco de Dados no Microsoft Azure

## 🧩 Descrição do Desafio

Este laboratório teve como objetivo **praticar o processo de criação e configuração de uma instância de Banco de Dados na plataforma Microsoft Azure**.  
Como entregável, foi desenvolvido este repositório contendo **resumos, anotações e dicas práticas** sobre o uso do Azure, servindo como **material de apoio para estudos e futuras implementações**.

---

## 🎯 Objetivos de Aprendizagem

Ao concluir este desafio, fui capaz de:

- ✅ Aplicar os conceitos aprendidos sobre o ecossistema Azure em um ambiente real;  
- 🧠 Documentar processos técnicos de forma clara, estruturada e reutilizável;  
- 🌐 Utilizar o **GitHub** como ferramenta de documentação e compartilhamento técnico.

---

## ⚙️ Tecnologias Utilizadas

- **Microsoft Azure Portal**
- **Azure SQL Database**
- **Azure Resource Group**
- **Azure Data Studio**
- **Git e GitHub**

---

## 🚀 Passo a Passo Realizado

### 1️⃣ Criação do Banco de Dados no Azure

1. Acessei o [Portal do Azure](https://portal.azure.com);
2. Criei um novo **Recurso do tipo Azure SQL Database**;
3. Configurei os parâmetros principais:
   - **Assinatura:** Visual Studio Enterprise Subscription  
   - **Grupo de Recursos:** `rg-lab-azure-sql`  
   - **Nome do Banco de Dados:** `db-lab-azure`  
   - **Servidor:** `server-lab-sql.database.windows.net`  
   - **Usuário Administrador:** `admin_lab`  
   - **Camada de Desempenho:** Basic (DTU-based)  
   - **Região:** Brazil South  

---

### 2️⃣ Configuração de Acesso Seguro

- Criei uma regra de **firewall** para permitir acesso do meu IP local;
- Desativei o acesso público após a configuração inicial;
- Testei a conexão através do **Azure Data Studio**, utilizando a string de conexão gerada automaticamente pelo portal.

```sql
SELECT DB_NAME() AS DatabaseName, SUSER_NAME() AS UserName, GETDATE() AS DateTimeConnected;
