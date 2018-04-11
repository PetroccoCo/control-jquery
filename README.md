## Nest Control sample app with jQuery

A simple thermostat control application that demonstrates how to access the Nest API from a web
application.

## Requirements

The development environment is a simple Node.js server managed by Yeoman.
If you don't have them already install these tools first:

* [Node][node]
* [Yeoman][yeoman]

## Prerequisite

In order to run this example you must first create an OAuth Client in the [Nest Developer portal][portal].  
The client should be created with the following required attributes:

OAuth Redirect URI: `http://localhost:8080/auth/nest/callback`  
Permissions: Thermostat read/write

All other attributes values are not specific and can be determined by the developer.

## Running

To install required Bower components and Node modules, simply type:

    $ bower install
    $ npm install

Next you will need your OAuth client ID and client secret in the [Nest Developer portal][portal] to set as environment variables:

    $ export NEST_ID='Your OAuth client ID here'
    $ export NEST_SECRET='Your OAuth client secret here'

And finally to start the server:

    $ npm start

Then open http://localhost:8080 in your browser and you will be walked through the authentication process.

## Contributing

Contributions are always welcome and highly encouraged.

See [CONTRIBUTING][contrib] for more information on how to get started.

## License

LCDBOLD - Standard Font License - Copyright 1999 by Samuel Reynolds. See [`app/fonts/LCDBOLD/readme.txt`][font-license] for more information.

control-jquery - Apache 2.0 - See [LICENSE][license] for more information.

[node]: https://nodejs.org/en/download/
[yeoman]: http://yeoman.io/learning/index.html
[portal]: https://console.developers.nest.com
[contrib]: CONTRIBUTING.md
[license]: LICENSE
[font-license]: https://github.com/nestlabs/control-jquery/blob/master/app/fonts/LCDBOLD/readme.txt
