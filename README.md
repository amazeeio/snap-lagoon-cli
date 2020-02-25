# Lagoon CLI
GoLang CLI tool for interacting with a Lagoon API

https://github.com/amazeeio/lagoon-cli

# How to install

`sudo lagoon install lagoon-cli`

Be sure you have `/snap/bin` in your path.  
At that point the command will be `lagoon-cli.lagoon`.  
I've created a request for settings an auto-alias to `lagoon` but you can set it with `sudo snap alias lagoon-cli.lagoon lagoon`.   

Because `lagoon` needs to access user's ssh-keys, you need to connect the first time you run the snap (that's due to the isolation by default snap packages provide)

`sudo snap connect lagoon-cli:ssh-keys`

At that point you can run the first command by passing the full path of your ssh key:   

`lagoon login -i ~/.ssh/id_rsa`