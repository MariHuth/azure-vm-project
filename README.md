#Projeto: Criação de uma Máquina Virtual no Microsoft Azure
Este projeto documenta o processo de criação de uma Máquina Virtual (VM) utilizando a plataforma de cloud computing Microsoft Azure. O objetivo principal foi adquirir experiência prática na implantação e configuração de recursos computacionais na nuvem, especificamente uma VM Linux.

## Visão Geral da VM

Aqui estão algumas capturas de tela das configurações e detalhes da VM que foi criada:

### Detalhes Iniciais da VM
![Detalhes Iniciais da VM] https://github.com/MariHuth/azure-vm-project/blob/main/images/09e1ab8c-23fc-47cc-9268-290e2dd21fc8.jpg

### Configurações de Hardware e Sistema Operacional
![Configurações de Hardware e Sistema Operacional] https://github.com/MariHuth/azure-vm-project/blob/main/images/239df854-7adc-4afa-b62f-1905a96df8db.jpg

### Disponibilidade e Dimensionamento
![Disponibilidade e Dimensionamento] https://github.com/MariHuth/azure-vm-project/blob/main/images/6d35e646-9eff-40c9-863d-ef63c281c7d3.jpg

### Configurações de Rede e Extensões
![Configurações de Rede e Extensões] https://github.com/MariHuth/azure-vm-project/blob/main/images/6d4cfcb2-2208-4530-9509-28ddaf34cd9a.jpg

### Configurações de Disco e Desligamento Automático
![Configurações de Disco e Desligamento Automático] https://github.com/MariHuth/azure-vm-project/blob/main/images/cb036535-a74a-45fa-8805-32b8e6ec55f3.jpg

##Objetivos do Projeto
O objetivo principal deste projeto foi implantar uma máquina virtual do zero, configurando-a para atender a requisitos básicos de computação. As metas específicas incluíram:

*Criar uma VM Linux na plataforma Azure.

*Configurar os recursos computacionais (vCPUs e RAM) e o armazenamento.

*Garantir que a VM estivesse em execução e acessível.

##Tecnologias Utilizadas
Microsoft Azure: Plataforma de nuvem utilizada para hospedar a máquina virtual.

Linux (Ubuntu 24.04): Sistema operacional escolhido para a VM.

AzureVM (Máquina Virtual): Recurso principal do projeto.

Passos para a Criação da VM
O processo de criação da VM seguiu os seguintes passos detalhados na plataforma Azure:

Escolha do Sistema Operacional: O sistema operacional selecionado foi o Ubuntu 24.04-LTS, uma versão estável e de longo prazo do Linux.

##Definição do Tamanho e Recursos:

Tamanho (SKU): Standard_D2alds_v6 foi o tamanho escolhido para a VM.

vCPUs: 2 vCPUs.

RAM: 4 GiB de memória RAM.

Configuração de Rede: Uma rede virtual (vnet-eastus2) e uma sub-rede (snet-eastus2-1) foram criadas para a VM. Um endereço IP público (68.154.3.112) foi atribuído para permitir acesso externo.

Configuração de Disco: Um disco de SO (AzureVM_OSDisk_1) foi configurado para hospedar o sistema operacional.

Configurações de Segurança: A inicialização confiável foi habilitada, juntamente com o vTPM, para aumentar a segurança da VM.

Extensões e Aplicativos: A extensão AADSSHLoginForLinux foi adicionada para facilitar o login via Azure Active Directory.

Desligamento Automático: O desligamento automático da VM foi agendado para as 19:00 (Horário Oficial do Brasil) para otimizar custos, garantindo que o recurso não ficasse em execução desnecessariamente.

##Resultados
A máquina virtual, nomeada AzureVM, foi criada com sucesso e está em execução no momento. A configuração escolhida atendeu aos requisitos do projeto, e todos os componentes (rede, disco, segurança) foram implementados conforme planejado. O status Em execução e o endereço IP público são evidências do sucesso da implantação.

##Aprendizados e Desafios
Este projeto proporcionou uma valiosa experiência com a plataforma Azure. Alguns dos principais aprendizados e desafios foram:

##Aprendizados:

Entendimento da estrutura de recursos do Azure, como grupos de recursos, redes virtuais e VMs.

Conhecimento prático sobre como configurar o tamanho (SKU) da VM e suas implicações em desempenho e custo.

O uso de extensões como o AADSSHLoginForLinux para simplificar a autenticação e a segurança.

#Desafios:

Garantir a correta configuração de rede, especialmente a atribuição do IP público e a sub-rede, para que a VM fosse acessível.

Compreender e aplicar as configurações de segurança, como a inicialização confiável e o vTPM.
