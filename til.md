# Things I Learned on This Project

I'd like to track as much of what I've learned as I can.

* How to install NVM
    
    - Use brew to install
    - mkdir ~/.nvm && export NVM_DIR=~/.nvm
    - add these to shell config file:
    
        - [ -s "/usr/local/opt/nvm/nvm.sh" ] && . "/usr/local/opt/nvm/nvm.sh"
        - [ -s "/usr/local/opt/nvm/etc/bash_completion" ] && . "/usr/local/opt/nvm/etc/bash_complete"
    - then `nvm install` the version of node you need

* Azure is very picky about the language versions it accepts.

    - Node has to be version 8 or 10, right now
    - Python has to be 3.6, not even 3.7 worked

* CircleCI doesn't support monorepos out of the box

* Netlify can host React apps that haven't been converted
to static websites

* VS Code can generate Azure Functions for you.
* Azure Functions only run locally with VS Code. Running the same commands from the command line will not get you a working Function
* Ignore the instructions on getting started with Azure and Python. The dependencies weren't installed, so nothing worked. Just use VS Code to create the Dunction instead.
* I was able to click around in the Azure portal and create a resource group, and a function app. Then, I deployed my function to that function app from VS Code. I don't see the option from the portal to connect the function app to a repository.