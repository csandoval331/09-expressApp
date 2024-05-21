# Notes
- created project by running **$ express --view=pug**

# Setting system environment
- ```$ printenv # will print system environment variables```
- ```$ export PORT=3000 # will set the variable PORT to 3000. Not recommended for local development```
- ```$ unset PORT=3000 # will remove variable PORT from environment variables```
- For this project, you will need to set **NODE_ENV=dev** and **DEBUG=\*** in order for ./bin/www > **require('debug')** to run
    - **DEBUG=\*** is a wildcard for package 'debug' that will get all errors
- You can print system environment in nodejs by running **console.log(process.env)**
- Consider using npm 'dotenv'
    - you will need a '.env' file in the root of your project
    - you will need to import package into project **require('dotenv').config()**
        - variables from .env will not be imported without this
        - once imported at the root of your project, they can be obtained from any file
        - 'dotenv' will overrider system variables
        - look at this about importing json objects into your project [link](https://stackoverflow.com/questions/58684642/should-i-call-dotenv-in-every-node-js-file)
    - you will need to read in variables into your project with **const PORT = process.env.PORT**





# Links:
- [npm debug](https://www.npmjs.com/package/debug)
- [npm dotenv](https://www.npmjs.com/package/dotenv)
- [in depth explanation of express app](https://www.reddit.com/r/node/comments/h0b1uh/can_anyone_explain_to_me_what_this_code_does/)
- [express-socketio project](https://github.com/aerrity/socket-click-example/blob/master/server.js)
- [express-socketio project #2](https://github.com/onedesign/express-socketio-tutorial)
