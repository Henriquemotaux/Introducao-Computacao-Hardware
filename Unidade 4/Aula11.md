# Aula 11 - Redes de Computadores: Topologias, Dispositivos e Meios

Este repositório contém a resolução e os materiais da **Aula 11**, abordando a organização física e lógica de redes de computadores, classificação de dispositivos e análise dos meios de transmissão.

---

## 1. Diagramas de Topologias

Abaixo estão descritas as representações estruturais das principais topologias de rede, identificando os nós (hosts) e os elementos centrais ou caminhos físicos de interconexão.

### Estrela (Star)
![[Estrela ](Imagens/11.png)](https://github.com/Henriquemotaux/Introducao-Computacao-Hardware/blob/main/Unidade%204/imagens/11.png)




### Barramento (Bus)
* **Descrição:** Todos os hosts compartilham um único meio de transmissão físico central (barramento linear).
* **Funcionamento:** Os dados são propagados pelo cabo para todos os dispositivos. Possui terminadores nas extremidades para evitar reflexão de sinal. Se o cabo principal falhar, toda a rede fica indisponível.

### Anel (Ring)
* **Descrição:** Os dispositivos conectados são dispostos em série, formando um circuito fechado (anel).
* **Funcionamento:** Os dados trafegam em uma única direção de nó em nó. Cada máquina atua como um repetidor até que a informação alcance o destinatário.

### Malha (Mesh)
* **Descrição:** Os hosts possuem conexões diretas ponto a ponto redundantes entre si.
* **Funcionamento:** Oferece múltiplos caminhos para que os dados cheguem ao destino, garantindo alta tolerância a falhas, embora possua alto custo de implementação de cabeamento e interfaces.

---

## 2. Quadro Comparativo de Dispositivos

| Característica | Hub | Switch | Roteador |
| :--- | :--- | :--- | :--- |
| **Função Principal** | Retransmitir pacotes para todas as portas sem filtragem. Atua na Camada 1 (Física). | Encaminhar pacotes seletivamente para a porta de destino usando endereços MAC. Atua na Camada 2 (Link de Dados). | Interconectar redes diferentes e gerenciar tráfego entre elas usando endereços IP. Atua na Camada 3 (Rede). |
| **Vantagens** | Baixo custo e facilidade de instalação. | Menor colisão de pacotes, maior largura de banda efetiva por dispositivo. | Alta inteligência no tráfego, isolamento completo de redes e segurança avançada. |
| **Limitações** | Alta colisão de pacotes (todos compartilham o mesmo domínio de colisão), baixa eficiência e falta de segurança. | Mais caro que o hub. O gerenciamento pode ser complexo (no caso de switches gerenciáveis). | Configuração complexa, maior latência de processamento de pacotes e custo financeiro elevado. |
| **Exemplo de Uso Real** | Redes locais muito antigas (legadas) ou laboratórios de testes e análise de tráfego. | Conexão interna de hosts (PCs, impressoras, servidores) dentro de uma mesma rede local (LAN). | O gateway principal que conecta uma rede doméstica ou corporativa à Internet (Conexão LAN-WAN). |

---

## 3. Meios de Transmissão

Os caminhos físicos e lógicos por onde os dados viajam são classificados de acordo com sua estrutura:

### Guiados (Com Fio)
Conduzem os sinais eletromagnéticos ou ópticos confinados dentro de um caminho físico.
* **Cabo de Fibra Óptica:** Utiliza pulsos de luz (fótons) através de um núcleo de vidro ou plástico revestido por uma casca. Possui altíssima velocidade, imunidade total a interferências eletromagnéticas e é ideal para longas distâncias (Backbones/WAN).
* **Cabo de Par Trançado (UTP/STP):** Fios de cobre entrelaçados em pares para cancelar interferências magnéticas externas. É o meio mais comum, flexível e econômico para redes locais (LAN).
* **Cabo Coaxial:** Formado por um condutor central de cobre envolto por uma malha blindada, oferecendo boa proteção mecânica e contra ruídos, herdado dos sistemas de TV a cabo.

### Não Guiados (Sem Fio)
Utilizam a propagação através do espectro eletromagnético em espaço aberto, dispensando barreiras físicas de confinamento.
* **Wi-Fi (Rede Sem Fio Local):** Ondas de rádio para conexões locais de alta velocidade para múltiplos hosts simultâneos (Smartphones, Laptops, Tablets).
* **Bluetooth (Comunicação de Curto Alcance):** Focado em redes de área pessoal (WPAN) de baixo consumo para conectar periféricos próximos.
* **Comunicação por Satélite:** Enlaces de rádio de longa distância com antenas terrestres enviando (Uplink) e recebendo (Downlink) dados via satélite.
* **Infravermelho (IV):** Utiliza feixes de luz infravermelha em curta distância. Requer linha de visão direta desimpedida (exemplo clássico: controles remotos de Smart TVs).

### Esquema Visual de Conexão dos Meios
