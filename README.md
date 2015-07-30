# keepalived_rabbitmq
HA configs of rabbitmq cluster with keepalived

+rabbitmq policy
rabbitmqctl set_policy ha-all "" '{"ha-mode":"all","ha-sync-mode":"automatic"}'`

+hostname
/etc/hostname
/etc/sysconfig/network

+commands
rabbitmqctl add_user teiron teiron
rabbitmqctl set_permissions teiron
rabbitmq-plugins enable rabbitmq_management
++lua support:stomp
rabbitmq-plugins enable rabbitmq_stomp


