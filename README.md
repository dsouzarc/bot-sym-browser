## SymBrowser

### Created by Ryan D'souza
A Software Engineering Intern on Symphony's Core Services team in the New York City office from 05/2016 - 08/2016.


#### Purpose
This bot was built in July of 2016 during Symphony's first 'bot-athon' as a fun/lighthearted project that won the 'Best Intern Bot' prize and was added to the Symphony Foundation as one of the first open-source bots created.

This bot allows you to browse the Internet and certain “Contexts”, while making it look like you’re doing work.
Right now, only the Reddit context is implemented, but one can get the text from any website in a format that looks like it is a long message from another Symphony user.
Other contexts can be implemented fairly easily through the bot’s modular design.

This project serves as an example of how to use contexts and can be modified to utilize new, user-created contexts that implement [this interface](https://github.com/symphonyoss/bot-sym-browser/blob/master/src/com/symphony/contexts/ServiceContext.java).

In a Financial Services environment, such contexts can, for example, include a "Wall Street Journal" context where a command like "@SymBrowser WSJ top" would return the top articles from The Wall Street Journal in a Symphony-esque message chat form or a command like "@SymBrowser WSJ Symphony" that would return articles from The Wall Street Journal that contain the text 'Symphony'. 


#### Modification Instructions

Navigate to [symbrowser.properties](https://github.com/symphonyoss/bot-sym-browser/blob/master/src/resources/symbrowser.properties) under `bot-sym-browser/src/resources` and modify all custom fields that are indicated with capital letters inside "[]". 

Add your Symphony-specific ".p12" certificate file to this "resources" directory as well.


#### Run Instructions

- Download this ZIP 

- Uncompress this ZIP 

- Open project folder in IntelliJ 

- Install Maven dependencies from the `pom.xml`

- Modify [symbrowser.properties](https://github.com/symphonyoss/bot-sym-browser/blob/master/src/resources/symbrowser.properties) (filepath: `bot-sym-browser/src/resources/symbrowser.properties`) with custom URLs and API Keys) 

- Make sure to add your Symphony certificate file inside the "resources" directory (`bot-symbrowser/src/resources/`) with "symphony-bot-user.p12" as the file name

- Run the main method of 'SymBrowserBot.java'

