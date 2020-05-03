
# RabbitMQ

[Azure](https://dev.azure.com/anyvent/RabbitMQ)

## Login GUI

[Link to RabbitMQ gui](http://10.3.56.9:15672/)
login: `guest`
password: `guest`
(login wordt later aangepast)

## RabbitMQ queues
[XML structuur](https://anyvent.github.io/docs/architecture/XML/)

## Master mapping queues
| Item| queue|
|----------------|------------|
| User | master-user-mapping-queue |
| Event | master-event-mapping-queue |


### Control room
| Item| queue|
|----------------|------------|
| User | control-room-user-queue |

### CRM
| Item| queue|
|----------------|------------|
| User | crm-user-queue |
| Event | crm-event-queue |

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
| Event | kassa-event-queue |

### Mailinglist
| Item| queue|
|----------------|------------|
| User | mailinglist-user-queue |
| Event | mailinglist-event-queue |

### Master UUID
| Item| queue|
|----------------|------------|
| User | master-uuid-user-queue |
| Event | master-uuid-event-queue |



