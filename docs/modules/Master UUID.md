# Master UUID
[azure](https://dev.azure.com/anyvent/Master UUID)

## Information page
[information page](http://10.3.45.4)

## Services

### Master UUID applicatie
Taal: C#

Type: console app

#### User registration from Frontend
Send [user XML](https://anyvent.github.io/docs/architecture/XML/#user) to `master-uuid-user-queue`

Master UUID will send the [XML](https://anyvent.github.io/docs/architecture/XML/#user) to the topic exchange and the topic exchange `user-exchange` will send the message to every other module.


#### Mapping user in master uuid after saving user in own system

Send [mapping XML](https://anyvent.github.io/docs/architecture/XML/#mapping) to `master-user-mapping-queue` 


### PHPMyAdmin
[Link](http://10.3.56.4:8080/)

Credentials:

- username: root
- password: password

### MySql
`http://10.3.56./3306`

