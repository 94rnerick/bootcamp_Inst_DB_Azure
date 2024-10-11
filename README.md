# Bootcamp_Inst_DB_Azure
Este repositório fala um pouco sobre o que aprendi durante o modulo instância de Banco de Dados na Azure do Bootcamp Microsoft Azure Essentials da Dio.

## Resumo dos Recursos Necessários:

Antes de criar uma instância de banco de dados na Azure, é importante configurar alguns recursos essenciais. Esses recursos fornecem a infraestrutura, segurança e conectividade necessárias para o correto funcionamento da instância de banco de dados.

1. **Grupo de Recursos**: Contêiner lógico para agrupar recursos.
2. **Rede Virtual (VNet) e Sub-rede** (opcional): Isolamento e controle de tráfego de rede.
3. **Endereço IP Público ou Regras de Firewall**: Controlar o acesso ao banco de dados.
4. **Servidor de Banco de Dados**: Hospeda e gerencia as instâncias de banco de dados.
5. **Armazenamento**: Definir o tipo e tamanho do disco para performance.
6. **Backup e Recuperação** (opcional): Estratégias de retenção e recuperação de dados.
7. **Credenciais Administrativas**: Definir usuários com permissões de administrador.
8. **Alta Disponibilidade e Réplicas** (opcional): Garantir disponibilidade e escalabilidade.
9. **Monitoramento e Logs** (opcional): Acompanhar a saúde e a segurança do banco de dados.



# Criando um instancia de DB no Azure:

##  Crie um Novo Recurso
- No menu lateral esquerdo, clique em **Criar um recurso**.
##  Selecione o Tipo de Banco de Dados
- Escolha o tipo de banco de dados que deseja criar, como **Azure SQL Database**, **Azure Database for MySQL**, **PostgreSQL**, ou **MariaDB**.
##  Configuração Básica
- Na primeira aba de **Básico**, insira as seguintes informações:
    - **Assinatura**: Selecione a assinatura de Azure.
    - **Grupo de Recursos**: Selecione um grupo de recursos existente ou crie um novo.
    - **Nome do Servidor ou Instância**: Dê um nome ao servidor ou instância do banco de dados.
    - **Região**: Escolha a localização onde o banco de dados será hospedado (ex.: East US, West Europe).
    - **Versão do Banco de Dados**: Selecione a versão do banco de dados (ex.: MySQL 5.7, PostgreSQL 12, etc.).
    - **Método de Autenticação**: Defina as credenciais do administrador do banco de dados (usuário e senha).

##  Configuração de Compute e Armazenamento
- Na aba **Compute + Storage**, configure os parâmetros de desempenho e armazenamento:
    - **Tamanho do Compute**: Escolha a quantidade de vCores e memória para a instância.
    - **Espaço de Armazenamento**: Defina o espaço em disco (SSD ou HDD) e o tamanho máximo de armazenamento.
    - **Escalabilidade**: Configure a escalabilidade de desempenho, se necessário (auto-escalonamento).

##  Configuração de Rede
- Na aba **Rede**, configure as opções de rede:
    - **Conectividade Pública/Privada**: Escolha se a instância será acessível pela internet (IP público) ou somente dentro de uma rede virtual (VNet).
    - **Firewall**: Defina as regras de firewall para controlar quais endereços IP podem acessar o banco de dados.
    - **Rede Virtual**: Caso opte por conectividade privada, associe a instância a uma rede virtual (VNet) existente.

##  Configurações de Segurança (opcional)
- Na aba **Segurança**, configure as opções de segurança:
    - **Auditoria e Logs**: Habilite a auditoria e o monitoramento de logs.
    - **Encriptação de Dados**: Escolha as opções de encriptação de dados em repouso e em trânsito.

##  Backup e Recuperação
- Na aba **Backup**, configure as políticas de backup e recuperação:
    - **Backups Automáticos**: Defina o período de retenção de backups automáticos (ex.: 7 dias, 35 dias, etc.).
    - **Restauração Georredundante**: Escolha se os backups serão replicados para outra região geográfica para recuperação de desastres.

##  Revisar e Criar
- Clique em **Revisar + Criar** para revisar as configurações.
- **Descrição**: O Azure validará todas as suas configurações. Se estiver tudo correto, uma tela de resumo será exibida.
- **Ação**: Clique em **Criar** para iniciar o processo de implantação da instância de banco de dados.

---

