# Zabbix
A explicação abaixo demonstra como em MEU ambiente eu consegui integrar o Zabbix 5.0 com o ServiceNow fazendo com que a abertura, atualização e fechamento dos chamados abertos sejam feitos de forma automática. Pode ser que eu seu ambiente também necessite estes ajustes, por isso estarei demonstrando aqui.

O Media Type padrão apenas abre e atualiza o chamado, não fazendo o fechamento.

# Procedimento

1 - Primeiramente exporte o media type padrão no Zabbix.
    (Adminstration -> Media Type -> Import)
2 - Crie ou use um usuário para que ele possa utilizar este media type.
    (Administration -> User -> Create User)
    (Administration -> User -> Select User)
3 - Com o usuário selecionado, na sessão Midia dele, cadastre o media type do ServiceNow.
    (Media -> Add -> Type: ServiceNow -> Send To: URL da sua instância Service Now)


