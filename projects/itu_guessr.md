# ITUGuessr

This idea comes from the GeoGuessr game, where users see images from GoogleMaps and try to find where it is.

In this project, we are using our own dataset from DatathonAI'24 to create a similar game to GeoGuessr, where users see images from ITU Ayazaga Campus and try to find where it is.

## Tech Stack

### Frontend

Frontend will be an addition to the current ITUAI Club project website.
Current repository: https://github.com/ITU-Artificial-Intelligence-Club/ituai-club

- **Environment:** TypeScript with Next.js
- **CI/CD:** Vercel
- **Deployment:** Vercel


### Backend

We will have to create a new repository for the backend of this project.

- **Environment:** Python 3.12 with FastAPI
- **Deployment:** Manual from our server
- **Database:** PostgreSQL

## Project Description

We have a dataset of JPG images, and their labels in one CSV file. We will need to decide on a database to store these images and labels, and then create an API to serve these images to the frontend.

We have a simple demo that runs on local, but it's completely written on HTML. We need to refactor this demo to use Next.js.
