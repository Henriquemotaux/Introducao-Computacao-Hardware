# Arquitetura de Redes

Henrique Mota Monteiro  


---

# 1. Linha do Tempo: Evolução da Escala

A evolução das redes partiu de sistemas isolados para a conectividade global que conhecemos hoje.

## 1950s - 1960s (Mainframes)
Computadores isolados, centralizados e de altíssimo custo, sem qualquer comunicação externa.

## 1969 (O Marco Inicial)
Criação da ARPANET, financiada pelo Departamento de Defesa dos EUA, com o objetivo de compartilhar recursos entre universidades.

## Evolução Atual (A Rede Global)
Transição para a Internet moderna, com a padronização da comunicação através de protocolos como o TCP/IP.

---

# 2. Elementos Fundamentais da Rede

Para que ocorra a comunicação, são necessários quatro componentes básicos:

| Elemento | Descrição | Exemplo Prático |
|---|---|---|
| **Emissor** | Dispositivo que transmite a informação inicial. | Um computador enviando um e-mail. |
| **Receptor** | Dispositivo de destino que recebe a informação. | Um smartphone recebendo uma mensagem. |
| **Meio de Transmissão** | Caminho físico (cabos) ou sem fio (ondas de rádio) que carrega o dado. | Cabos Ethernet ou sinal Wi-Fi. |
| **Protocolo** | Regras universais que definem como a comunicação ocorre e é compreendida. | Protocolo TCP/IP. |

---

# 3. Classificação de Redes (Abrangência Geográfica)

As redes são categorizadas conforme a área física que cobrem.

## PAN (Personal Area Network)
Dispositivos muito próximos (alguns metros).  
**Exemplo:** Bluetooth entre celular e fone.

## LAN (Local Area Network)
Rede local que ocupa uma sala, escritório ou prédio.  
**Exemplo:** Ethernet (IEEE 802.3).

## CAN (Campus Area Network)
Abrange múltiplos prédios.  
**Exemplo:** Universidades ou hospitais.

## MAN (Metropolitan Area Network)
Abrange uma cidade.  
**Exemplo:** Redes de concessionárias como Telefônica ou Embratel.

## WAN (Wide Area Network)
Rede de longa distância, conectando países.  
**Exemplo:** A própria Internet.

## Variações e Modelos

- **WLAN:** LAN sem fio via radiofrequência.
- **VLAN:** Rede configurável por software, independente da estrutura física.
- **Intranet:** Rede privada restrita ao acesso interno de uma organização.

---

# 4. Modelos Computacionais

Define como os dados são processados e administrados:

## Computação Centralizada
Um computador central atende a diversos "terminais burros" (sem poder de processamento próprio).

## Cliente/Servidor
Um servidor central de alto desempenho fornece serviços e diretórios para máquinas clientes.

## Ponto-a-Ponto (P2P)
Modelo descentralizado onde qualquer máquina pode atuar como cliente e servidor simultaneamente.
