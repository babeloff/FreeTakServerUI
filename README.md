# FTS Web UI
![image](https://user-images.githubusercontent.com/60719165/177003787-c1322f17-a55e-4d81-a0a1-25c6178cb42e.png)

This FreeTAKServer UI repository hosts the web user interface for the FreeTAKServer project. 
It is built using Python with Flask, 
employing additional technologies such as SQLite for database management, 
Alembic for database schema migrations, and 
Flask_Login for session-based authentication. 
The UI supports various features like modular design through 
Flask Blueprints, forms validation, and provides a dashboard for server management. 
The front-end utilizes HTML, CSS, SCSS, and JavaScript, 
making it a comprehensive tool for administrators to manage the FreeTAKServer. 
The project is licensed under the EPL/MIT License.

FTS Web UI allows administrators to easily manage the [FTS](https://github.com/FreeTAKTeam/FreeTakServer) server.
This component requires a working backend. 
The WebUI is a completely separate application connecting to  the FTS backend. 
It uses an API to seamless query server functions. 
Depending on his deployment, may or may not be  seen from remote machines.

This [video](https://www.youtube.com/watch?v=ot3PNY903ns&t=3sa), 
provides an overview of most features described in the 
[user manual](https://github.com/FreeTAKTeam/FreeTakServer/blob/master/docs/FTS%20UI%20Documention.pdf).

## Installation and configuration
This section provides an overview of the installation process. 
Refer to the online 
[documentation](https://freetakteam.github.io/FreeTAKServer-User-Docs/Installation/Linux/Install/) 
for details. 

To install FTS and the UI type in a console
```
sudo python3 -m pip install FreeTAKServer[ui]
```

Setup your Configuration
your administrator will need to configure the following files
```
Config.py for the UI
MainConfig.py for FTS
```

### Start FTS

```
nohup sudo python3 -m FreeTAKServer.controllers.services.FTS 
```

## Start the WebUI

In the console type navigate to the installation path:
```
cd /usr/local/lib/python3.8/dist-packages/FreeTAKServer-UI
```

```
nohup sudo python3 run.py
```

## Dashboard Features

- SQLite,  
- Alembic (DB schema migrations)
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
 
- **MIT License**
