# XML structure Anyvent
## User
[schema](https://raw.githubusercontent.com/Anyvent/XSD/master/general_user.xsd)
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message version="1.0">
	<Header>
		<Sender>TestModule</Sender> 
		<Timestamp>5444</Timestamp> 
		<Type>Create</Type> 
	</Header>
	<User>
		<UUID>315685156</UUID>
		<Firstname>Jonas</Firstname>
		<Lastname>Van den Cruyce</Lastname>
		<Email>jonas.van.den.cruyce@student.ehb.be</Email>
		<Address>
			<Street>Steenweg</Street>
			<Housenumber>15</Housenumber>
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

## Mapping
[schema](https://raw.githubusercontent.com/Anyvent/XSD/master/mapping.xsd)
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message version="1.0">
	<Header>
		<Sender>TestModule</Sender> 
		<Timestamp>5444</Timestamp> 
	</Header>
	<Mapping>
		<UUID>315685156</UUID>
		<ID>5</ID>
	</Mapping>
</Message>
```

## Event
❌ [schema](https://raw.githubusercontent.com/Anyvent/XSD/master/event.xsd)
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message version="1.0">
	<Header>
		<Sender>TestModule</Sender> 
		<Timestamp>5444</Timestamp> 
		<Type>Create</Type>
	</Header>
	<event>
		<UUID>315685156</UUID>
		<Name>Final Work Presentatie</Name>
		<Date>dd-mm-yyyy</Date>
		<Time>hh:mm</Time>
		<Address>
			<Street>Steenweg</Street>
			<Housenumber>15</Housenumber>
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
[schema](https://raw.githubusercontent.com/Anyvent/XSD/master/heartbeat.xsd)
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Heartbeat version="1.0">
	<Sender>TestModule</Sender> 
	<Timestamp>5444</Timestamp> 
</Heartbeat>
```

## Log
❌ [schema]()
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message version="1.0">
	<Header>
		<Sender>TestModule</Sender> 
		<Timestamp>5444</Timestamp>
	</Header>
	<Log>
		<Type>Error</Type> 
		<Msg>explanation error</Msg>
	</Log>
</Message>
```
