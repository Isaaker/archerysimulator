# Flask (Python)
![Flask logo](https://flask.palletsprojects.com/en/3.0.x/_images/flask-horizontal.png)
## About Flask

Flask is an open-source project maintained by [The Pallets Projects](https://palletsprojects.com).

This project makes posible to code web applications with Python to complement other technologies like HTML, CSS and JS.

> Flask is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions. However, Flask supports extensions that can add application features as if they were implemented in Flask itself.

[Font: Wikipedia](https://en.wikipedia.org/wiki/Flask_(web_framework))
## What we use Flask?

In previous versions, the project has used different technologies: HTML, PHP. And for the new version 3.0 we have started to include CSS to give a better look to the platform, JS that gives us the ability to integrate functionalities only possible with it, and we have decided to replace PHP by Python using Flask. We have made this decision even though PHP is a fundamental part of the platform, because we believe that Python will improve the platform in many aspects: Speed, Security, Integration and will give us new ways to develop by integrating this library its own micro web server that although not suitable for production use can be a good opportunity for developers to not have to download an additional web server.

## Security Considerations

Although Flask is a much more secure library than PHP and is more resistant to some code infection or XSS attacks, it is important to take certain security considerations into account. [Please read this section of the official documentation](https://flask.palletsprojects.com/en/3.0.x/security/).

## Flask Documentation

[Flask Documentation here](https://flask.palletsprojects.com/en/3.0.x/)

## Built-In server

**THIS MICROSERVER SHOULD NEVER BE USED IN PRODUCTION.**

A great feature of Flask is that it comes with a small built-in server that allows the developer to work on the web application without having to install a web server on their computer.
This built-in server displays the application through a localhost port and can even be viewed from other devices by performing certain configurations.

### Starting the micro server

To run the micro server, run the below commands (This commands need to be ruined from the Ghost_Simulator_ES/ directory):

1. `. ./ghost_simulator/.venv/bin/activate`
2. `flask --app ghost_simulator run`

**Flask prints the URL to use in the explorer with the port.**

### Options

--debug / --no-debug            Set debug mode.

-h, --host TEXT                 The interface to bind to.

-p, --port INTEGER              The port to bind to.

--cert PATH                     Specify a certificate file to use HTTPS.

--key FILE                      The key file to use when specifying a certificate.

--reload / --no-reload          Enable or disable the reloader. By default the reloader is active if debug is enabled.

--debugger / --no-debugger      Enable or disable the debugger. By default the debugger is active if debug is enabled.

--with-threads / --without-threads Enable or disable multithreading.

--extra-files PATH              Extra files that trigger a reload on change. Multiple paths are separated by ':'.

--exclude-patterns PATH         Files matching these fnmatch patterns will not trigger a reload on change. Multiple patterns are separated by ':'.

--help                          Show this message and exit.

Example: `flask --app ghost_simulator run --debug`
### More info

The information about the usage of the micro server can be found [here](https://flask.palletsprojects.com/en/3.0.x/server/)

## Deploy to Production

Information about deploy to production can be found [here](https://flask.palletsprojects.com/en/3.0.x/tutorial/deploy/)