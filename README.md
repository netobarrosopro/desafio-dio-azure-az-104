# desafio-dio-azure-az-104
Navegando no Azure - Dicas e Resumo Essencial para Iniciantes

Introdução: O que é o Azure?

O Microsoft Azure é uma plataforma de computação em nuvem abrangente que oferece mais de 200 produtos e serviços. Ele permite que você construa, gerencie e implante aplicações e serviços em uma rede global usando ferramentas e estruturas de sua escolha. Em vez de comprar e manter servidores físicos em seu próprio data center, você "aluga" recursos de computação, armazenamento e rede diretamente da Microsoft.

Mas, com tanta coisa disponível, por onde começar? Este guia didático foi criado para resumir os conceitos mais importantes e dar dicas práticas para você começar a usar o Azure de forma eficiente e segura.

Parte 1: Resumo dos Conceitos-Chave do Azure

Para entender o Azure, você precisa dominar alguns conceitos fundamentais:

1. Assinatura (Subscription):
Pense na sua assinatura como a sua conta bancária no Azure. Ela é um contêiner lógico para os seus recursos, e é a ela que as cobranças são associadas. Você pode ter várias assinaturas para organizar seus projetos, equipes ou departamentos.

2. Grupo de Recursos (Resource Group):
Um Grupo de Recursos é um contêiner lógico para agrupar recursos relacionados a uma aplicação ou projeto. Por exemplo, você pode criar um Grupo de Recursos chamado app-web-producao e colocar nele sua máquina virtual, seu disco, sua rede virtual e seu banco de dados. Isso facilita o gerenciamento, o monitoramento e a exclusão conjunta dos recursos. Dica: Sempre agrupe recursos que têm o mesmo ciclo de vida.

3. Região (Region):
Uma Região do Azure é um conjunto de data centers físicos localizados em uma área geográfica. Exemplos são "Leste dos EUA", "Europa Ocidental" ou "Sul do Brasil". A latência, a conformidade de dados e a redundância dependem de onde seus recursos são implantados. Dica: Escolha a região mais próxima dos seus usuários para reduzir a latência e verifique a disponibilidade de serviços na região antes de implantar.

4. Recurso (Resource):
Um recurso é uma instância de um serviço do Azure. Exemplos incluem uma Máquina Virtual (VM), uma conta de armazenamento, um banco de dados SQL, uma rede virtual, entre outros. Tudo o que você cria no Azure é um recurso.

5. Modelo de Responsabilidade Compartilhada:
Este é um dos conceitos mais importantes para a segurança. Na nuvem, a responsabilidade pela segurança e manutenção é compartilhada entre você (o cliente) e a Microsoft (o provedor).

    Microsoft é responsável por: A segurança da nuvem em si (data centers físicos, infraestrutura, hardware).

    Você é responsável por: A segurança na nuvem (seus dados, aplicativos, sistemas operacionais, configurações de rede). A sua responsabilidade varia dependendo do modelo de serviço:

        IaaS (Infraestrutura como Serviço): Você gerencia o sistema operacional, os aplicativos e os dados. A Microsoft gerencia a infraestrutura física. Exemplo: Máquinas Virtuais (VMs).

        PaaS (Plataforma como Serviço): Você gerencia seus dados e aplicativos. A Microsoft gerencia a infraestrutura, o sistema operacional e o middleware. Exemplo: Azure SQL Database.

        SaaS (Software como Serviço): Você apenas usa o software. A Microsoft gerencia tudo. Exemplo: Microsoft 365.

Parte 2: Dicas Práticas para o Dia a Dia no Azure

Dica 1: Otimize Custos com Monitoramento e Orçamentos
O maior desafio para iniciantes é controlar os custos.

    Use a Calculadora de Custos do Azure: Antes de criar qualquer recurso, use a calculadora para estimar o custo mensal.

    Configure Orçamentos e Alertas: No portal do Azure, na seção de Gerenciamento de Custos e Cobrança, crie orçamentos para suas assinaturas e grupos de recursos. O Azure enviará alertas quando você atingir 50%, 75% ou 90% do seu limite.

    Use Máquinas Virtuais de Baixo Custo (B-series): Para ambientes de desenvolvimento/teste, as VMs da série B (burstable) são uma ótima opção econômica.

    Desligue Recursos Inativos: Máquinas virtuais, por exemplo, continuam a ser cobradas mesmo quando ociosas. Use a funcionalidade de desligamento automático ou automação para desligá-las fora do horário comercial.

Dica 2: Priorize a Segurança Desde o Início
Não deixe a segurança para depois.

    Use Grupos de Segurança de Rede (NSGs): Configure NSGs para controlar o tráfego de entrada e saída de suas redes virtuais. Bloqueie todas as portas de que você não precisa.

    Habilite o Azure Defender for Cloud: Este serviço oferece uma visão centralizada da postura de segurança, recomendações e proteção contra ameaças para seus recursos.

    Implemente o Acesso Just-in-Time (JIT): Para VMs, em vez de deixar a porta de acesso remoto (como a porta 22 para SSH ou 3389 para RDP) aberta permanentemente, use o JIT para abrir a porta apenas quando necessário e por um tempo limitado.

Dica 3: Monitore o Desempenho e a Saúde dos Recursos
O Azure Monitor é seu melhor amigo para isso.

    Configure Alertas: Defina alertas para métricas importantes, como utilização de CPU, memória ou disco em suas VMs. Seja notificado por e-mail ou SMS quando um limite for atingido.

    Analise Logs com o Log Analytics: Use o Log Analytics para consultar e analisar logs de recursos. A Linguagem de Consulta Kusto (KQL) é a chave para extrair informações valiosas.

    Use a Topologia do Network Watcher: Para visualizar a estrutura da sua rede e as conexões entre os recursos.

Dica 4: Simplifique a Gestão com Automação e Ferramentas
Não faça tudo manualmente!

    Use o Azure CLI ou o Azure PowerShell: Para gerenciar recursos via linha de comando e automatizar tarefas.

    Aproveite o Azure Resource Manager (ARM): Use templates ARM ou Terraform para implantar sua infraestrutura de forma consistente e repetível.

    Implemente Rotinas de Backup Automáticas: Use o Azure Backup para agendar backups automáticos e garantir a recuperação dos seus dados. Lembre-se de criar um Recovery Services Vault na mesma região dos seus recursos.

Conclusão: O Azure é uma Jornada Contínua

Começar com o Azure pode parecer assustador, mas entendendo os conceitos básicos (Assinaturas, Grupos de Recursos, Regiões, Recursos) e aplicando as dicas práticas de custo, segurança e monitoramento, você estará no caminho certo. Lembre-se, o aprendizado na nuvem é uma jornada contínua. Mantenha-se atualizado com as novidades e explore os serviços conforme a necessidade. A flexibilidade e o poder do Azure estão ao seu alcance!
