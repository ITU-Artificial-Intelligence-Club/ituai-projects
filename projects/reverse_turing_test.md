# Reverse Turing Test

The idea is simple. There is a chat with a number of LLMs, and you are participating the chat trying to blend in as another LLM. At the end, all of the bots try to guess which participant was actually a human.

## Tech Stack

### Frontend

Current repository: https://github.com/ITU-Artificial-Intelligence-Club/ituai-club

- **Environment:** TypeScript with Next.js
- **CI/CD:** Vercel
- **Deployment:** Vercel


### Backend

Current repository: https://github.com/ITU-Artificial-Intelligence-Club/ituai-club-api

- **Environment:** TypeScript with Nest.js
- **Deployment:** Manual from our server
- **Database:** PostgreSQL

## Project Description

We need to create a decent set of personas, with their images and short descriptions.

We need to re-orgainze the front-end:
- Adding the club logo for going to the landing page on the right-top
- Refactor character selection and chat screes

We need to organize the prompts on the backend to get a more structured output and change the prompts fro the chat to get more decent responses.
https://platform.openai.com/docs/guides/structured-outputs#function-calling-vs-response-format

We want to add text-to-speech and speech-to-text features to the chat; so that LLMs responses can be heard and the human can respond by speaking.
