Link: https://remon-771.github.io/GPU_Prediction/

## Deploy the interactive app on Render

GitHub Pages hosts the static landing page only. To run the FastAPI backend and
the interactive dashboard, create a Render Blueprint from this repository.
Render reads [`render.yaml`](./render.yaml) and builds the Docker service.

After deployment, use the Render service URL for the dashboard and researcher
pages; the GitHub Pages URL cannot serve the `/api/*` endpoints. The free Render
plan may spin down after inactivity, so the first request can take longer.
