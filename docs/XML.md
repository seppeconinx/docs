#XMl structure Anyvent
## User
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message>
	<Header>
		<Sender>{Module}</Sender> //Module vanwaar het komt
		<Timestamp>hh:mm:ss</Timestamp> //Wanneer het verzonden is
		<Type>Create</Type> //Create, Update, Delete
	</Header>
	<User>
		<UUID>315685156</UUID>
		<Firstname>Jonas</Firstname>
		<Lastname>Van den Cruyce</Lastname>
		<Email>jonas.van.den.cruyce@student.ehb.be</Email>
		<Address>
			<Street>Steenweg</Street>
			<Housenmuber>15</Housenmuber>
			<City>Opwijk</City>
			<Zip>1745</Zip>
		</Address>
		<Tags>
			<Tag>Data</Tag>
			<Tag>Networks</Tag>
		</Tags>
	</User>
</Message>
```

## Event
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message>
	<Header>
		<Sender>{Module}</Sender> //Module van waar het komt
		<Timestamp>hh:mm:ss</Timestamp> //Wanneer het verzonden is
		<Type>Create</Type> //Create, Update, Delete
	</Header>
	<event>
		<UUID>315685156</UUID>
		<Name>Final Work Presentatie</Name>
		<Date>dd-mm-yyyy</Date>
		<Time>hh:mm</Time>
		<Address>
			<Street>Steenweg</Street>
			<Housenmuber>15</Housenmuber>
			<City>Opwijk</City>
			<Zip>1745</Zip>
		</Address>
		<Organiser>
			<Firstname>Jonas</Firstname>
			<Lastname>Van den Cruyce</Lastname>
			<Email>jonas.van.den.cruyce@student.ehb.be</Email>
		</Organiser>
		<Tags>
			<Tag>IT</Tag>
			<Tag>Nerd</Tag>
		</Tags>
	</event>
</Message>
```

## Heartbeat
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Heartbeat>
	<Sender>{Module}</Sender> //Module van waar het komt
	<Timestamp>hh:mm:ss</Timestamp> //Wanneer het verzonden is
</Heartbeat>
```

## Error
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message>
	<Header>
		<Sender>{Module}</Sender> //Module van waar het komt
		<Timestamp>hh:mm:ss</Timestamp> //Wanneer het verzonden is
	</Header>
	<Log>
		<Type>Error</Type> //Warning, Error, Info, ...
		<Msg>explanation error</Msg>
	</Log>
</Message>
```
