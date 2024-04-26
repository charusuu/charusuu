### Olá, eu sou o Charles Júnio! 😉


[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/charlless_jr/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/charusuu)
[![Twitter](https://img.shields.io/badge/Twitch-9146FF?style=for-the-badge&logo=twitch&logoColor=white)](https://www.twitch.tv/charleszzard)

SnakeMatch
+-- common (client/Server shared files)
|   +-- game-objects (classes that represents the different game objects)
|   |   |-- board.js
|   |   |-- pellet.js
|   |   |-- snake-part.js (represent a single part of a snake)
|   |   |-- snake-head.js (represnt the snake head, inherits from snake-part)
|   |   |-- snake.js (represent the snake, a collection of snake-part and head)
|   |-- protocol.js (protocol functions for encoding / decoding messages)
|   |-- rectangle.js
+-- client (client code)
|     +-- deploy (holds the files for deploy)
|     +-- js
|       +-- lib
|       |   |-- graphics.js (functions for drawing on the canvas)
|       |   |-- util.js (Polyfill for necessary node.js util functions in the client)
|       |-- index.js (common client functions/enums, also declare our namespace on window)
|       |-- connector.js (responsible for sever communication)
|       |-- snake-engine.js (manages the game on the client)
|       |-- game-state.js (object to hold the current game state)
+-- server (server code)
|   +-- game
|   |   |-- snake-engine.js (manages the snake game on the server)
|   |   |-- match.js (manages a snake match between 2 players)
|   |   |-- player.js (represnts a single player, basically sending/receiving messages)
|   |-- server.js (starts the web server, our main file)
|   |-- lobby.js (manages client connections and pair players to matches)
|-- Gruntfile.js (grunt build tasks)
|-- .jshintrc (some jshint rules)
|-- package.json
