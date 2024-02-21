# Warehouse-Tool
Curio Internship: 6 februari t/m 7 juli.

***
## Usage:
*(Not useable anymore, no access to API etc.)*
Console-based tool that can be used through the commandline, it can load a JSON setting file that sends the data to the API, 
then sets up a test-warehouse and can be used to save alternate settings that were changed later on. 
I made the JSON setting files myself from the already existent templates I recieved.

## Development:
The API used here was specifically created for the company where my intership was. I used Docker to develop and test the API/app.
The development started as a menu type of console app but later on i added the option to use it as a commandline so its faster and more efficient to use.

## Documentation:
#### Commands
There are multiple commands or menu-options that can be used, I put in a help command to let the user know what commands there are and what options you have so it is more accessible for people. 
All commands are: `help`, `json.read`, `json.write`, `item.read`, `item.write`.
*(There are checks so the user is send to the `help` command when a wrong string is entered.)*
You can choose to use the menu, there it is just some switch cases that lets the user choose which option they want to use.

#### Options
##### help
Gives the user a list of commands they can use, they are listed underneath here.
##### json.read
Lets the user read out a JSON file, it asks which JSON it wants to read and then puts it inside the API, there it creates a testing environment for the programmers working on the warehouse software, so its easy and quick to test the thing they make.
It is used because every warehouse is a little different but has the same setup, so with settings it can be set up for testing.
##### json.write
This lets the user write the created JSON that they maybe changed/edited so it can later be used to test another time, so you can switch between warehouses and back up the warehouse for later.
When a JSON is written it save it at `bin\Debug\net6.0\Jsons`, here all JSON files are stored.
##### item.read

##### item.write
This lets the user write the created JSON for the item list they made or edited so it can later be used to test another time, so you can back up the items stored in that warehouse and use it for later or put it inside another warehouse.
When a JSON is written it save it at `bin\Debug\net6.0\ItemJsons`, here all JSON files are stored.
