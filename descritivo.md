Servidores on premise em cluster com os servidores ( AD, PrintServer, FileServer e Adconect), reduzindo custos de licenciamento, tendo resiliência de dados;
Rede roteada no galpão, para poder crar regras de segurança nos firewall para acesso somente dessa rede para o backoffice, onde tem um private endpoint, para ter ip da rede interna criada na azure.
Colocado um WAF com load balancer, com isso temos a segurança de acesso pelo SSO e redirecionando para aplicação externa, tendo um NSG que ajuda na segurança entre as conexões do app externo e o MySql na rede interna.
App Service Plan, temos a observabilidade do sistema.
