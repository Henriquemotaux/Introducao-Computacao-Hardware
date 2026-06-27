# 3. Estudo de Cenário: O Ataque Global do Ransomware WannaCry (Opção A)

## Contexto do Ataque
Em maio de 2017, o mundo testemunhou um dos ataques cibernéticos mais devastadores e velozes da história da computação: o surto do ransomware **WannaCry**. Este código malicioso espalhou-se de forma epidêmica por mais de 150 países, infectando mais de 200 mil computadores em poucas horas. O ataque paralisou empresas globais de logística, gigantes do setor automobilístico e, de forma crítica, o Serviço Nacional de Saúde (NHS) do Reino Unido, forçando o cancelamento de cirurgias, exames e o redirecionamento emergencial de ambulâncias.

## Vulnerabilidade Explorada
O WannaCry utilizou uma abordagem híbrida altamente perigosa. Ele combinava a natureza destrutiva de um ransomware com a capacidade de replicação autônoma de um *worm* . A brecha explorada foi uma **vulnerabilidade técnica** crítica de execução remota de código localizada no protocolo de compartilhamento de arquivos *Server Message Block (SMBv1)* de sistemas operacionais Microsoft Windows. 

A exploração utilizou um exploit conhecido como *EternalBlue* (alegadamente desenvolvido pela NSA e vazado por hackers). Embora a Microsoft tivesse lançado uma atualização de segurança (*patch*) dois meses antes do ataque , milhares de instituições ao redor do globo falharam na aplicação correta da política de gerenciamento e correção de atualizações, deixando as suas infraestruturas completamente expostas e desprotegidas .

## Atributos de Segurança Violados e Impactos
O ataque desferiu um golpe direto contra os pilares fundamentais da Segurança da Informação:
* **Disponibilidade (Violada de Forma Crítica):** Ao invadir uma máquina, o WannaCry realizava a criptografia em massa dos arquivos locais e exibia uma tela exigindo o pagamento de um resgate em Bitcoins . O bloqueio completo dos dados e servidores resultou em indisponibilidade absoluta dos sistemas . Hospitais ficaram cegos sem acesso aos prontuários dos pacientes e linhas de montagem industriais pararam por completo devido à falta de dados operacionais.
* **Integridade (Violada):** Os dados originais foram modificados e corrompidos coercitivamente de sua forma natural para uma forma codificada e inacessível sem a chave do invasor, quebrando a garantia de completude e exatidão da informação .

## Medidas de Mitigação (Aplicadas e Recomendadas)
Com base nas lições do WannaCry e alinhando-as com as práticas recomendadas na nossa literatura base, as medidas cruciais para conter e prevenir cenários análogos incluem:

1.  **Políticas Rígidas de Atualização e Correção (Patching):** Garantir o monitoramento contínuo e a instalação automatizada e imediata de atualizações críticas em sistemas operacionais e softwares a fim de fechar brechas conhecidas antes que sejam exploradas .
2.  **Estratégia de Backups Offline Resilientes:** Manter rotinas automatizadas de cópias de segurança (backups) que permaneçam desconectadas da rede principal (offline), assegurando que os dados possam ser restaurados prontamente em sua integridade caso ocorra um incidente de criptografia forçada .
3.  **Segmentação de Redes e Firewalls Ativos:** Implementar firewalls de rede robustos para bloquear o tráfego de protocolos vulneráveis (como o SMB) a partir de conexões externas e isolar sub-redes internas para evitar a propagação lateral de códigos maliciosos .
