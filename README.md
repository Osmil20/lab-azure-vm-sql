# Lab Azure - Máquina Virtual e Banco de Dados SQL

Este repositório contém o resumo das lições aprendidas durante o desenvolvimento em nuvem na DIO, incluindo a criação de uma Máquina Virtual no Azure e de um Banco de Dados SQL.

---

## 1. Criação da Máquina Virtual (VM)

- **Objetivo:** Praticar a criação e configuração de uma máquina virtual no Azure.
- **Passos realizados:**
  1. Acesse o portal do Azure e vá em **Máquinas Virtuais**.
  2. Clique em **Criar > Máquina Virtual**.
  3. Configure:
     - Sistema operacional: Windows Server 2019 Datacenter – Gen2
     - Tipo de VM: B1s (gratuita, teste) ou outro disponível
     - Usuário administrador: `azureuser`
     - Rede: IP público habilitado para teste
  4. Conclua a criação e aguarde a **implantação**.
  5. Conecte à VM usando o botão **Conectar** do portal.
  
- **Conceitos aprendidos:**
  - Diferença entre CapEx e OpEx.
  - Diferença entre nuvem pública, privada e híbrida.
  - Garantias de SLA (Service Level Agreement).
  - Importância de configurar acesso seguro e rede pública limitada.

---

## 2. Criação do Banco de Dados SQL

- **Objetivo:** Configurar e acessar um banco de dados SQL no Azure.
- **Passos realizados:**
  1. No portal do Azure, vá em **Banco de Dados SQL**.
  2. Clique em **Criar > SQL Database**.
  3. Configure:
     - Nome do banco: `MeuBancoSQL`
     - Servidor: `meusqlserver` (novo servidor lógico)
     - Camada de serviço: **Uso Geral - Sem servidor**
     - Armazenamento: 32 GB
     - Backup: redundância geográfica
     - Admin SQL: usuário criado pelo Azure (`CloudSA3f56fae8`)
  4. Conecte-se ao banco usando **Query Editor**, **VS Code** ou outro cliente.
  5. Criou-se tabela de teste e dados de exemplo usando SQL (opcional para aprendizado).

- **Conceitos aprendidos:**
  - Diferença entre autenticação SQL e Azure AD.
  - Camadas de serviço e computação (Provisionado vs Sem Servidor).
  - Redundância de backups e importância da alta disponibilidade.
  - Conexão de aplicativos ao banco de dados via cadeias de conexão.

---

## 3. Aprendizados Gerais

- Criar e gerenciar recursos na nuvem exige atenção às **configurações de rede e segurança**.
- O portal do Azure facilita o provisionamento rápido de recursos.
- Conhecer os tipos de autenticação é essencial para conectar clientes externos.
- A documentação oficial e as cadeias de conexão ajudam a integrar bancos de dados com aplicações.


**Autor:** Osmil Dias  
**Curso:** Desenvolvimento em Nuvem - DIO
