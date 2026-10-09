```

   ┌──────────────────────────────────────────┐
   │ mensajes_taller                          │
   ├──────────────────────────────────────────┤
   │ PK  id           uuid                    │
   │     routing_key  text         NOT NULL   │
   │     payload      jsonb        NOT NULL   │
   │     recibido_en  timestamptz  NOT NULL   │
   └──────────────────────────────────────────┘

```




vicentefabar@Laptop-de-Vicente biblioteca-plataforma % docker compose exec rabbit1 rabbitmqctl list_queues name messages

Timeout: 60.0 seconds ...
Listing queues for vhost / ...
name	messages
notificaciones.dlq	1
auditoria	0
notificaciones	0
correos.dlq	0
auditoria.dlq	1
correos	0
