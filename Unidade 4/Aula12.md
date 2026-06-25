

# Aula 12 – Internet: História, Conceitos, Protocolos e Navegadores

Este repositório contém a atividade prática desenvolvida para a matéria de Introdução à Computação do 1º semestre de Engenharia de Software.

---

## 1. História da Internet

### Linha do Tempo e Evolução
* **ARPANET (Décadas de 1960/1970):** Criada pelo Departamento de Defesa dos EUA (DARPA) durante a Guerra Fria. Foi a pioneira na tecnologia de **comutação de pacotes**, estabelecendo uma rede descentralizada que resistiria a falhas parciais de infraestrutura.
* **Expansão Acadêmica e Militar:** Nos anos 80, a rede ramificou-se. A parte militar formou a MILNET, enquanto universidades norte-americanas e europeias interconectaram-se para o compartilhamento de pesquisas acadêmicas e correio eletrônico.
* **Comercialização (Anos 90):** A infraestrutura deixou de ser restrita ao governo e à academia. Provedores de acesso privados surgiram, permitindo a conexão de empresas e residências em escala global.
* **Criação da WWW:** Em 1989, o cientista **Tim Berners-Lee**, no CERN, idealizou a *World Wide Web*. Com a criação dos conceitos de HTTP, HTML e URL, a internet transformou-se em um ecossistema visual e navegável por hiperlinks.

---

## 2. Conceitos Fundamentais

### Internet vs. Web
* **Internet:** É a **infraestrutura física e global**. Composta por servidores, cabos de fibra óptica submarinos, roteadores e satélites que interconectam redes de computadores no mundo todo.
* **Web (World Wide Web):** É um **serviço virtual** que opera *sobre* a internet. Trata-se do sistema de páginas interconectadas que acessamos via navegadores. Outros serviços que utilizam a internet, mas não são a Web, incluem jogos online, e-mail (protocolo SMTP) e redes de mensagens (como WhatsApp).

### Arquitetura Cliente-Servidor
É o modelo de computação distribuída padrão da Web:
* **Cliente:** O dispositivo ou aplicação (ex: navegador web) que inicia uma requisição solicitando dados ou serviços.
* **Servidor:** Computadores de alta performance conectados continuamente à rede, responsáveis por processar as requisições, armazenar dados e devolver as respostas adequadas aos clientes.

### Endereços IP (Internet Protocol)
O IP funciona como a identidade e localização única de cada dispositivo conectado à rede.
* **Exemplo Prático:** Para acessar o motor de busca do Google, o navegador precisa localizar o IP do servidor correspondente (ex: `142.250.74.46`). Como decorar números é complexo para humanos, utilizamos o sistema de nomes de domínio (DNS) para digitar apenas `google.com`.

---

## 3. Protocolos de Comunicação

Os protocolos são o conjunto de regras padronizadas que permitem a comunicação homogênea entre sistemas heterogêneos.

| Protocolo | Significado | Função Principal | Exemplo Prático |
| :--- | :--- | :--- | :--- |
| **TCP/IP** | *Transmission Control Protocol / Internet Protocol* | O TCP fraciona os dados em pacotes, garante que cheguem sem erros e na ordem correta. O IP realiza o roteamento desses pacotes do ponto de origem ao destino. | Download de um instalador (.exe): o TCP garante que nenhum byte seja corrompido no caminho. |
| **HTTP / HTTPS** | *Hypertext Transfer Protocol (Secure)* | Protocolo de transferência de hipertexto. O **HTTPS** adiciona criptografia via SSL/TLS, garantindo a confidencialidade dos dados trafegados. | Navegação segura em plataformas de e-commerce e internet banking. |
| **DNS** | *Domain Name System* | Serviço de resolução de nomes que traduz URLs legíveis por humanos em endereços IP legíveis por máquinas. | Digitar `github.com` e o navegador descobrir automaticamente qual servidor hospeda o site. |
| **FTP** | *File Transfer Protocol* | Protocolo otimizado exclusivamente para a transferência rápida e direta de arquivos entre um cliente e um servidor. | Desenvolvedor enviando arquivos de mídia pesados diretamente para o servidor de hospedagem do site. |

---

## 4. Navegadores (Browsers)

Os navegadores são softwares encarregados de interpretar linguagens de programação e marcação baseadas em texto e renderizá-las em uma interface gráfica inteligível para o usuário.

* **HTML (HyperText Markup Language):** Define a estrutura física, os blocos de texto, formulários e elementos da página.
* **CSS (Cascading Style Sheets):** Controla a estética, estilização, cores, tipografia e o layout visual.
* **JavaScript:** Camada lógica que adiciona interatividade dinâmica, manipulação de dados em tempo real e comportamento à página.

### Motores de Renderização (Rendering Engines)
O motor é o componente interno do navegador que processa o código e desenha os pixels na tela:
* **Blink:** Desenvolvido pelo Google (fork do WebKit). Utilizado no Google Chrome, Microsoft Edge, Opera e Brave.
* **Gecko:** Desenvolvido pela Mozilla. Utilizado no Firefox, com forte foco em padrões abertos e privacidade.
* **WebKit:** Desenvolvido pela Apple. Motor nativo do Safari. Nota: devido a restrições de ecossistema, todos os navegadores rodando no iOS são obrigados a utilizar o WebKit.

### 6. Reflexão Individual 
A análise da história e dos protocolos da internet me fez refletir sobre a robustez da infraestrutura que sustenta a sociedade moderna. Compreender o modelo cliente-servidor e o papel desempenhado pelo TCP/IP e pelo DNS deixa claro que o desenvolvimento de software não acontece no vácuo; ele depende de uma rede complexa de regras e padrões. Além disso, estudar os motores de renderização (Blink, Gecko, WebKit) me deu uma nova perspectiva sobre a importância da compatibilidade de código e padrões web (W3C), um desafio real que enfrentarei como engenheiro de software no mercado. 

