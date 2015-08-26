# Basic Test for Nodejs UDP

This test fires up a basic nodejs [server](server.js) and wait for inputs at a UDP port.

In order to make it easier to have [netcat](http://radarearth.com/content/using-netcat-udp-port-troubleshooting) client and [nodejs](https://nodejs.org/api/dgram.html) server on the same console, [tmuxinator](https://github.com/tmuxinator/tmuxinator) wrapper was used by [nodejs_udp project](nodejs_udp.yml).

## Installation & Execution

**NOTE:** nodejs_udp.yml should be modified to point to your deployment folder.

- Pull server code in your deployment folder:

      git clone <project>

- Create *tmux* session project:

      mux edit nodejs_udp.yml

   or maybe just by copying configuration to your **tmuxinator** project folder:

       cp nodejs_udp.yml ~/.tmuxinator

- Start tmux session:

      mux start nodejs_udp.yml
