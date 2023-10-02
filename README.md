# Zabuino: O Poder da Precisão, a Inteligência da Integração
**Alunos: João Savaris, Tiago Mohr e Wagner Holleweger**

No universo em constante movimento da tecnologia, o controle preciso da temperatura é essencial para manter ambientes seguros e operando com eficiência máxima. Apresentamos o Zabuino, uma solução de monitoramento de temperatura que vai além das expectativas, integrando perfeitamente dois gigantes da gestão de dados: Zabbix e Grafana.

Por que Escolher o Zabuino?

**Precisão Inigualável**: O Zabuino é equipado com sensores de ponta que proporcionam leituras de temperatura excepcionalmente precisas, garantindo dados confiáveis para tomadas de decisão precisas.

**Integração Zabbix e Grafana**: O Zabuino une o poder do Zabbix, um dos sistemas de monitoramento mais robustos do mundo, com a flexibilidade e visualizações impressionantes do Grafana. Isso significa que você tem acesso a dados em tempo real e visualizações personalizadas em um único painel intuitivo.

**Histórico Detalhado e Análise Preditiva**: O Zabuino mantém registros meticulosos de dados de temperatura, permitindo análises de tendências e a implementação de estratégias proativas para otimizar o ambiente.

**Fácil Instalação e Configuração**: Com um design intuitivo e guias claros, a instalação do Zabuino é rápida e descomplicada. Em questão de minutos, você estará protegido.



**Acompanhe abaixo o nosso diagrama de classes do projeto**
![2023-08-28_21h09_18](https://github.com/Holleweger/ProjetoRegionalidade/assets/65625548/c20d282c-12d6-4855-85d6-565ab4fa8580)

**Requisitos funcionais e nao funcionais**
![2023-08-28_21h22_29](https://github.com/Holleweger/ProjetoRegionalidade/assets/65625548/e571d3a0-53f6-42e9-8937-cf0554f3db1e)


**Título:** _"Asas da Inovação: Zabuino Eleva a Avicultura"_

Na comunidade de avicultores, Lucas, um engenheiro agrícola, trouxe uma reviravolta. Ao combinar sua paixão por aves com seu conhecimento tecnológico, ele criou o "Zabuino" - um sistema que revolucionou os aviários. Equipado com sensores precisos e uma interface intuitiva, o Zabuino permitiu que os avicultores monitorassem a temperatura e umidade dentro dos aviários em tempo real. Com alertas imediatos e dados históricos disponíveis no "AviaryHub", as aves passaram a viver em ambientes ideais, e os avicultores abraçaram um novo nível de eficiência e planejamento. A história de Lucas e do Zabuino destaca como a fusão da tecnologia com a natureza pode conduzir a um futuro próspero para a avicultura.


**Ambiente Desenvolvimento**

Sensor de Temperatura:
- Arduino

Sistema Operacional:
- Almalinux

Interface de Obetenção de Dados:
- Zabbix

Interface de Usuário:
- Grafana

Banco de Dados:
- Mysql (Zabbix)


# Documentação de Integração entre Zabbix e Grafana
**Resumo**
Esta documentação descreve os passos necessários para integrar o Zabbix e o Grafana, permitindo a visualização de dados de monitoramento do Zabbix em painéis do Grafana. Essa integração proporciona uma interface gráfica avançada para análise e monitoramento de sistemas, redes e serviços.

**Índice**
Requisitos
Instalação do Zabbix
Configuração do Zabbix
Instalação do Grafana
Configuração do Grafana
Integração entre Zabbix e Grafana
Criação de Dashboards

**1. Requisitos**
Antes de iniciar a integração, certifique-se de ter:

Servidor Linux com acesso à internet.
Permissões de administrador no servidor.
Zabbix e Grafana instalados no mesmo servidor ou em servidores diferentes.

**2. Instalação do Zabbix**
Siga a documentação oficial do Zabbix para instalação do servidor Zabbix e do agente em: Link para Documentação Oficial do Zabbix

**3. Configuração do Zabbix**
Após a instalação do Zabbix, certifique-se de que os hosts que deseja monitorar estejam configurados e funcionando corretamente.

**4. Instalação do Grafana**
Siga a documentação oficial do Grafana para instalação em: Link para Documentação Oficial do Grafana

**5. Configuração do Grafana**
Acesse a interface do Grafana pelo navegador.
Faça login com suas credenciais.

**6. Integração entre Zabbix e Grafana**
No Grafana, clique no ícone de engrenagem no menu lateral esquerdo e selecione "Data Sources".
Clique em "Add your first data source".
No campo de busca, digite "Zabbix" e selecione o plugin do Zabbix.
Preencha os campos conforme a configuração do seu servidor Zabbix:
HTTP: Endereço do servidor Zabbix (ex: http://seu_servidor_zabbix/zabbix).
Name: Um nome para a fonte de dados.
Access: Selecione o tipo de acesso (direct ou proxy).
User e Password: Credenciais de um usuário do Zabbix com permissões suficientes.
Clique em "Save & Test" para verificar a conexão.

**7. Criação de Dashboards**
No Grafana, clique no "+" no menu lateral esquerdo e selecione "Dashboard".
Clique em "Add new panel".
No painel de configuração, em "Query", selecione "Zabbix" no menu suspenso.
Escolha a fonte de dados Zabbix configurada anteriormente.
Configure as métricas e o host desejados.
Personalize o painel conforme suas necessidades, adicionando gráficos, tabelas, etc.
Clique em "Apply" para salvar o painel.
Com esta integração, você poderá visualizar e analisar os dados de monitoramento do Zabbix em painéis dinâmicos e customizáveis no Grafana. Aproveite as vantagens dessa combinação poderosa para otimizar o monitoramento de seus sistemas e serviços.

# Visualizacao Dos dados coletados pelos sensores(EM DESENVOLVIMENTO)
![2023-08-28_21h09_04](https://github.com/Holleweger/ProjetoRegionalidade/assets/65625548/1f609f0c-c628-4d83-b9b3-1969d10d44c6)
