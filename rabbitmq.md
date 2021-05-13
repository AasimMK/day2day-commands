### Create User
```
rabbitmqctl add_user RabbitUser YOURPASSORDHERE
rabbitmqctl add_vhost rabbit
rabbitmqctl set_user_tags RabbitUser administrator
rabbitmqctl set_permissions -p rabbit RabbitUser ".*" ".*" ".*"
```

### Delete User
```
rabbitmqctl delete_user guest
```
