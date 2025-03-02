# Reverse Turing Test

The idea is simple. There is a chat with a number of LLMs, and you are participating the chat trying to blend in as another LLM. At the end, all of the LLMs try to guess which participant was actually a human.

## Tech Stack

### Frontend

Current repository is [here](https://github.com/ITU-Artificial-Intelligence-Club/ituai-club).

- **Environment:** TypeScript with Next.js
- **Styling:** TailwindCSS
- **Deployment & CI/CD:** Vercel


### Backend

Current repository [here](https://github.com/ITU-Artificial-Intelligence-Club/ituai-club-api).

- **Environment:** TypeScript with Nest.js
- **Database:** PostgreSQL
- **ORM:** Not decided yet, could be Prisma or TypeORM
- **Deployment:** Manual from our server, for both the API and the database


## Project Description

Current status of the project is in [ituai.club/turing/reverse](https://www.ituai.club/turing/reverse).

In the beginning, you select a persona to participate in the chat. There is currently random 40 known people, mostly contributed to science.

After you select your character, ChatGPT and Gemini randomly selects 2 other characters.

One of the characters start chatting, and after every character wrote 3 messages, the chat ends and one final prompt is sent to the LLMs, asking them to guess which character was a human.

Then the final screen is shown with their guesses.


## Changes & Improvements

### Persona Selection

We need to create a more decent set of personas, with their images and short descriptions.


### Design Refactor

We need to re-orgainze the front-end to
- Add the club logo linking to the landing page on the right-top corner, as in the other pages
- Refactor character selection to be more user-friendly, showing the images of the characters and their short descriptions
- According to the designers like, we can try to improve the design of the chat screen

### Used Prompt

One of the main issues with the prompts is that, AI do not understand how to ask questions to understand if you are human or not. We need to change the prompts to get more decent results.

Also, at the end of the chat, when we ask AI's to guess who is the human, sometimes their answer is not only the name but like "I think it was __". We need to have a more structured output from the LLMs. We can use the following docs to get a better output:

OpenAI Structured Output is [here](https://platform.openai.com/docs/guides/structured-outputs#function-calling-vs-response-format).
Gemini Extracting Structured Data is [here](https://ai.google.dev/gemini-api/tutorials/extract_structured_data).
Similar thing on Anthropic Claude is [here](https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/increase-consistency).
We do not support DeepSeek yet, it can be added. JSON output docs are [here](https://api-docs.deepseek.com/guides/json_mode).

### Text <--> Speech

Currently the game is sort of boring people, since they need to read the long messages, and write a relatively long response.

We can improve the experience here by adding text-to-speech to LLM responses, and if activated their responses can be heard.

Also, we can add speech-to-text to the chat, so that the user can respond by speaking, instead of writing.

It is not certain how can we add this feature, we need to investigate the possibilities.
