# A WebAdmin based CLI for Apache James

## Development

Webadmin command-line interface is an upcoming replacement for the outdated, security-vulnerable JMX command-line interface. It also aims at providing a more modern and intuitive interface.

## Run the script

## Syntax

General syntax to run the script

        
        $ ./james_cli [OPTION] ENTITY ACTION {ARGUMENT}
        
where

    OPTION: optional parameter when running the script,
  
    ENTITY: represents the route performing actions,
  
    ACTION: name of the action to perform,
  
    ARGUMENT: arguments needed for the action.

Example: 
```
$ ./james_cli --url http://127.0.0.1 --port 9999 domain list
```

The above command lists all domain names available on domain route at address http://127.0.0.1:9999. 
It does not require any argument to execute. Options --url and --port are optional. Without them, the default value is http://127.0.0.0:8000.
As for other commands, arguments might be required after the sub-command (ACTION such as list, add and remove).

Note: the command line ```$ ./james_cli``` will be documente as {cli}.

## Navigation menu

- [Manage Domains]()
   - [Create a domain]()
   - [Delete a domain]()
   - [Check if a domain exists]()
   - [Get the list of domains]()
- [Manage Users]() 
   - [Create a user]()
   - [Test a user existence]()
   - [Delete a user]()
   - [Get users list]()
   - [Update a user password]()

## Manage Domains

### Create a domain

```
{cli} domain create <domainToBeCreated>
```

### Delete a domain

```
{cli} domain delete <domainToBeDeleted>
```

### Check if a domain exists

```
{cli} domain exist <domainToBeChecked>
```

### Get the list of domains

```
{cli} domain list
```

// Domain Alias

## Manage Users

### Create a user

```
{cli} user create <username> <password>
```

### Test a user existence

```
{cli} user exist <username>
```

### Delete a user

```
{cli} user delete <username>
```

### Get users list

```
{cli} user list
```

### Update a user password
Same than Create, but a user need to exist.

If the user do not exist, then it will be created.


