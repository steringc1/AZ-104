
# AZ-104 - Máquinas Virtuais no Microsoft Azure

_**O que é?**_ 
É o serviço de computação do Azure que permite criar e executar máquinas virtuais na nuvem.

**_Para que serve?_** 
Serve para hospedar sistemas operacionais, aplicações, bancos de dados, ambientes de teste, laboratórios e qualquer workload que você executaria em um servidor físico.

**_Qual cenário se aplica?_** 
Quando você precisa de servidores sob demanda, com flexibilidade de tamanho, performance, sistema operacional e alta disponibilidade sem manter infraestrutura física.

🟦 _**Regiões**_


_**O que é?**_
Locais que possuem datacenters do Azure. Cada região possui seu próprio preço ao criar VMs.

_**Para que serve?**_
Permite escolher onde os recursos serão criados fisicamente.

_**Qual cenário se aplica?**_
Quando você precisa selecionar uma região por preço, latência ou requisitos de conformidade.

🟦 _**Availability Zone**_
_**O que é**_
Forma de distribuir a disponibilidade entre 3 zonas diferentes. As VMs são replicadas no mesmo datacenter e também para outro datacenter. SLA de 99,99%.

_**Para que serve**_
Aumentar a resiliência das VMs contra falhas físicas.

_**Qual cenário se aplica**_
Sistemas que não podem parar mesmo se um datacenter inteiro falhar.

🟦 _**Availability Set**_

_**O que é**_
Replica a VM dentro do mesmo datacenter (entre os racks). SLA de 99,95%.

_**Para que serve**_
Evitar que várias VMs caiam ao mesmo tempo devido a falha de rack ou manutenção.

**_Qual cenário se aplica_**

Ambientes onde você precisa garantir que pelo menos uma VM continue rodando durante falhas ou atualizações.

🟦 **Virtual Machine Scale Set**
_**O que é**_
Aumenta ou diminui a quantidade de VMs de acordo com a demanda (mesmo tamanho de VM).

_**Para que serve**_
Escalonar automaticamente a capacidade conforme uso.

_**Qual cenário se aplica**_

Aplicações que recebem picos de acesso e precisam escalar de forma automática.

🟦 **Update Domain**
_**O que é**_

Domínio de atualização. Usado quando é necessário realizar manutenções no rack.

_**Para que serve**_

Evitar que todas as VMs fiquem indisponíveis durante atualizações.

_**Qual cenário se aplica**_

Ambientes que fazem parte de um Availability Set.

🟦**Fault Domain**
_**O que é**_

Representa a falha de um rack.

_**Para que serve**_

Garantir que as VMs sejam distribuídas entre racks diferentes para evitar queda total.

_**Qual cenário se aplica**_

Infraestruturas que precisam de tolerância a falhas físicas.

🟦 **Conceito de Escala**
**Escala Vertical**
_**O que é**_

Aumentar ou diminuir a capacidade de uma única VM/workload.

_**Para que serve**_

Melhorar o desempenho de uma VM específica.

_**Qual cenário se aplica**_

Quando o sistema depende de uma VM única e você precisa mais CPU, memória ou disco.

**Escala Horizontal**
_**O que é**_

Aumentar ou diminuir a quantidade de VMs (scale set).

_**Para que serve**_

Distribuir carga entre várias VMs.

_**Qual cenário se aplica**_

Aplicações que rodam melhor em múltiplas instâncias iguais.

🟦 **Spot Instance**
_**O que é**_

Modelo de precificação onde o recurso que seria desperdiçado pelo Azure pode ser usado posteriormente.

_**Para que serve**_

Economizar usando VMs com preço reduzido.

_**Qual cenário se aplica**_

Workloads que podem ser interrompidos sem problema.

🟦**Tamanhos de VM**
_**O que é**_

Cada tamanho possui uma finalidade diferente.

_**Para que serve**_

Escolher a VM ideal para cada necessidade.

_**Qual cenário se aplica**_

Quando você define a VM de acordo com o tipo de workload.
**Exemplos:**

H → Computação de alto desempenho

B → Uso geral

E → Otimizado para memória

F → Otimizado para computação

L → Otimizado para storage




# Monitoramento e Gerenciamento de Máquinas Virtuais no Microsoft Azure

**_1. O que é_**: Monitoramento de recursos no Azure é o processo de acompanhar em tempo real a saúde, desempenho e disponibilidade dos serviços e máquinas virtuais na plataforma. Ele utiliza ferramentas como Azure Monitor, Log Analytics, Application Insights e Alerts para centralizar informações e permitir decisões rápidas.

_**2. Para que serve**_: Serve para garantir que os recursos funcionem dentro do esperado, detectar problemas antes que causem impacto, otimizar custos, registrar eventos e fornecer visibilidade total do ambiente.

_**3. Cenário de uso**_: Usei o monitoramento para acompanhar o estado de máquinas virtuais criadas durante o laboratório, verificando métricas de CPU, disco, rede, criando alertas para eventos críticos e registrando tudo em um Log Analytics Workspace para posterior análise.

_**4. Recursos criados no laboratório**_
Máquina Virtual de teste:
- Log Analytics Workspace
- Configuração do Azure Monitor
- Alertas customizados
- Dashboards com métricas

_**5. Aprendizados principais**_**
- Habilitar métricas e logs em uma VM
- Consulta de logs com KQL
- Como criar alertas baseados em condições específicas
- Como montar visualizações e dashboards
- Como o monitoramento ajuda na prevenção de incidentes




