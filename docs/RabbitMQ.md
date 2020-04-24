
# RabbitMQ

[Azure](https://dev.azure.com/anyvent/RabbitMQ)

## Login GUI

[Link to RabbitMQ gui]([http://10.3.56.9:15672/)
login: `guest`
password: `guest`
(login wordt later aangepast)

## Master queue

master-queue

## Master user mapping queue

master-user-mapping-queue

## RabbitMQ queues

[XML structuur](https://anyvent.github.io/docs/XML/)

### Control room
| Item| queue|
|----------------|------------|
| User | control-room-user-queue |

### CRM
| Item| queue|
|----------------|------------|
| User | crm-user-queue |

### Facturatie
| Item| queue|
|----------------|------------|
| User | facturatie-user-queue |

### Frontend
| Item| queue|
|----------------|------------|
| User | frontend-user-queue |

### Kassa
| Item| queue|
|----------------|------------|
| User | kassa-user-queue |

### Mailinglist
| Item| queue|
|----------------|------------|
| User | mailinglist-user-queue |

### Master UUID
| Item| queue|
|----------------|------------|
| User | master-uuid-user-queue |



