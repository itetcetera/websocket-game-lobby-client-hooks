# websocket-game-lobby-client-hooks

> ⚛️ React hooks for use with websocket-game-lobby

[![NPM Version](http://img.shields.io/npm/v/websocket-game-lobby-client-hooks.svg?style=flat)](https://www.npmjs.org/package/websocket-game-lobby-client-hooks)

## Install

```bash
$ npm install websocket-game-lobby-client-hooks
```

## API

### useWebSocketGameLobbyClient

```javascript
const { data, connected, send } = useWebSocketGameLobbyClient();
```

#### send(type, data);

##### Type

| Name     | Description                        |
| -------- | ---------------------------------- |
| `create` | Create a new game.                 |
| `join`   | Join existing game with game code. |
| `leave`  | Leave current game.                |
| `start`  | Start current game.                |
| `end`    | End current game.                  |

##### Examples

```javascript
send('create'); // Create new game
send('join', { gameCode: 'ABCD' }); // Join game with game code
send('leave'); // Leave current game
send('start'); // Start current game
send('end'); // End current game
```
