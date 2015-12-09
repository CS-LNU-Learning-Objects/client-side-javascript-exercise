# Autocomplete
In this exercise we will write an autocompleting input field. 

[TODO] Detailed instructions

## The server
To have something to contact we need a server up and running. You find the server in the "server"-folder. 

### Install
Install the required packages by writing `npm install --no-bin-links` when you are in the folder `exercise/autocomplete`.

You will need to add the followin line to your `/vagrant/Vagrantfile`:

```
config.vm.network "forwarded_port", guest: 3001, host: 3001
```

### Start server
Start the server in a seperate terminal window by writing `npm run server`
The server will listen on port 3001 (see app.js for config). 

API:
* POST http://localhost:3001/teams
* require header "Content-Type: application/json"
* post data as example:
    {
        query: "MAN"
    }
