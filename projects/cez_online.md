# CezRoom

Cez is a chess-variant created by Huseyin. This project is to create an online platform for the game.

URL: ituai.club/cez/

## Tech Stack

### Frontend

Current repository: https://github.com/ITU-Artificial-Intelligence-Club/ituai-club

- **Environment:** TypeScript with Next.js
- **CI/CD:** Vercel
- **Deployment:** Vercel


### Backend

Current repository: https://github.com/ITU-Artificial-Intelligence-Club/cez-api

- **Environment:** Python 3.12 with FastAPI
- **Deployment:** Manual from our server

## Project Description

This project is not going to start from scratch but rather will be an addition to the current Cez project.

### Additions and Changes

#### Frontend

Canvas rendering is a bit messy, it needs to be refactored and cleaned up.

#### Backend

Currently there is only AI for Cez on the backend. We need to create a continuous websocket connection for the game, where users will be able to:
- Create a game
- Join a game
- Watch a game - would be cool

And do some certain actions while playing the game.

Websocket communication needs to be implemented with FastAPI.

## Project Plan

0. Play and learn Cez ♟️
1. Figure out how to establish WebSocket (WS) connections between two players 🔌
    - Test out the WS connection with dummy data
2. Add ability to create rooms/matches. People should be able to join either by code or by link
3. Implement serialization/deserialization for Cez game state (?)
    - The game should render the new state when it's recieved
    - Are there any security concerns? Hacks, open to exploits?
4. Implement player roles, which person plays black/white
    - E.g. if a player who is playing white sends a move for black, it should be discarded
