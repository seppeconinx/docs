# XML structure Anyvent
[generate radnom](https://genxml)
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
[schema](https://raw.githubusercontent.com/Anyvent/XSD/master/event.xsd)
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message version="1.0">
	<Header>
		<Sender>TestModule</Sender> 
		<Timestamp>5444</Timestamp> 
		<Type>Create</Type>
	</Header>
	<Event>
		<UUID>315685156</UUID>
		<Name>Final Work Presentatie</Name>
		<StartDateTime>1207</StartDateTime>
		<EndDateTime>3308</EndDateTime>
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
	</Event>
</Message>
```

## Event Registration
[schema](https://raw.githubusercontent.com/Anyvent/XSD/master/event_registration.xsd)
```xml
<?xml version="1.0" encoding="UTF-8"?>
<Message version="1.0">
    <Header>
        <Sender>TestModule</Sender> 
        <Timestamp>5444</Timestamp> 
        <Type>Register</Type> 
    </Header>
    <EventRegistration>
        <UserId>789456</UserId>
        <EventId>1234548</EventId>
    </EventRegistration>
</Message>
```
Type can be `Register` or `Unregister`

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
[schema](https://raw.githubusercontent.com/Anyvent/XSD/master/logging.xsd)
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
