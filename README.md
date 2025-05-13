# Meu-Projeto-SQL-MI
# 💡 Projeto: Configuração de Instância Gerenciada SQL no Azure

Este repositório foi criado como parte de um laboratório prático com o objetivo de **configurar uma Instância Gerenciada de SQL no Microsoft Azure**.  
O projeto serve como material de apoio para estudos e futuras implementações na plataforma.


## 🛠️ Configuração da Instância Gerenciada

### 🔹 Etapa 1: Dados básicos da Instância SQL MI
- Informações sobre assinatura, recurso, vCores, armazenamento, custo mensal e autenticação.

![Dados básicos]![Image](https://github.com/user-attachments/assets/95c13969-b035-44d1-bfd6-6dcb364b67f1)

---

### 🔹 Etapa 2: Configuração de Rede e TLS
- Sub-rede virtual, tipo de conexão Proxy, versão mínima TLS, e ponto público de dados.

![Rede e TLS]![Image](https://github.com/user-attachments/assets/92cb69de-3959-4553-8a60-c45886d80352)

---

### 🔹 Etapa 3: Segurança
- Criptografia, identidade gerenciada, chaves e dados avançados.

![Segurança](imagens/instancia_sql_mi_segurança.png)

---

### 🔹 Etapa 4: Tela de Criação Final da Instância
- Janela de manutenção, política de atualização e informações do projeto.

![Criação da instância](imagens/instancia_sql_mi_criacao.png)

---

## 🆚 Comparativo: Azure SQL Database vs SQL Managed Instance

| Característica                     | Azure SQL Database                   | Azure SQL Managed Instance          |
|-----------------------------------|--------------------------------------|-------------------------------------|
| Tipo de serviço                   | PaaS (Banco individual)              | PaaS (instância completa)           |
| Suporte a SQL Agent               | ❌ Não                                | ✅ Sim                               |
| Linked Servers                    | ❌ Não                                | ✅ Sim                               |
| Suporte a VNET                    | Parcial (com endpoints privados)     | ✅ Total                             |
| Autenticação integrada (AD)       | Limitada                             | ✅ Sim                               |
| Backup/Restore com .bak           | ❌ Não                                | ✅ Sim                               |
| Tempo de migração                 | Rápido                               | Mais demorado                       |
| Casos de uso                      | Apps modernos e simples              | Migração de ambientes locais (on-premises) |

---

## 🧠 Observações

- A instância foi criada na região **West US 3** com **8 vCores**, **256 GB de armazenamento** e **sem redundância de zona**.
- Utilizou-se autenticação mista (SQL + Microsoft Entra).
- A versão do SQL Server utilizada foi a **2022**.
- Custos estimados: cerca de **US$ 1.472,75/mês para computação** + **US$ 29,44/mês para armazenamento**.

---

## 🔗 Recursos úteis

- [Documentação oficial do Azure SQL MI](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/)
- [Comparação entre modelos do Azure SQL](https://learn.microsoft.com/pt-br/azure/azure-sql/database/features-comparison)
