# factorio-control-panel
Web admin interface for [Factorio](http://factorio.com/) headless game server

### Installation (Linux server)

- Install [Factorio headless server](http://www.factorio.com/download-headless/stable) and [Node.js](https://nodejs.org/en/download/).

- Install the node module

        npm install -g factorio-control-panel
    
- Set environment variables and start the web server
    
        export FACTORIO_DIR='/usr/local/factorio'
        export ADMIN_PASSWORD='******'
        export PORT=8000
        factorio-control-panel

### Installation (Docker container)

    docker pull jjclark/factorio
    docker run -d -p 8000:8000 -p 34197:34197/udp --env ADMIN_PASSWORD='******' jjclark/factorio
    
### Usage

- Navigate to the control panel at [http://localhost:8000](http://localhost:8000).

- Upload save files and mods for the server to use. Other players can download them from here.

- Click "Start Server." This and other admin actions require the `ADMIN_PASSWORD` set above.
