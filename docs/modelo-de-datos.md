"""

   Column    |           Type           | Collation | Nullable |      Default      
-------------+--------------------------+-----------+----------+-------------------
 id          | uuid                     |           | not null | gen_random_uuid()
 routing_key | text                     |           | not null | 
 payload     | jsonb                    |           | not null | 
 recibido_en | timestamp with time zone |           | not null | now()
Indexes:
    "mensajes_taller_pkey" PRIMARY KEY, btree (id)

 """