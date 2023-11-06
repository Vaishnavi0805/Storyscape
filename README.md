# Storyscape
StoryScape is an AI-powered app designed to spark the imagination of children by generating captivating story videos based on user prompts. With StoryScape, the possibilities for storytelling are endless.

How to Use
Follow these steps to set up and use StoryScape:

Installation
Before running the app, make sure to install the required libraries. If you're using Google Colab, you can run the provided code cell to install the necessary dependencies.

Fill in Experiment Environment Variables
In the provided code, fill in the following variables with your specific values:

PROJECT_ID: Your Cloud project ID.
REGION: The region where you want to run the jobs.
GCS_BUCKET: The Cloud Storage bucket for storing experiment output.
SERVICE_ACCOUNT: The service account for deploying fine-tuned models.
Initialize Vertex-AI API
Initialize the Vertex-AI API using the provided code to set up your project, location, and staging bucket.

Define Constants
These are pre-defined constants for training and serving Docker images.

Deploy Model
You can deploy the model using the deploy_model function. Provide the model_id and task as parameters.

Generate Story
Use the story function to generate a story based on user input. The function returns the generated story text.

Generate Audio
The audio function converts the story text into audio files and uploads them to a specified bucket.

Generate Image
The image function generates images based on the story text and uploads them to a specified bucket.

Merge Audio and Image
The merge_audio_image function combines audio and image files to create a final video.

Generate Video
Click the "Generate Video" button to create and display the final video.

Usage
Input your text prompt in the provided field.
Click "Generate Video" to initiate the story video creation process.
Important Notes
Make sure to replace placeholder values (such as PROJECT_ID and SERVICE_ACCOUNT) with your specific information.
Ensure you have the necessary permissions and credentials set up for the associated services (Google Cloud, Vertex-AI, etc.).
Enjoy creating imaginative and captivating stories with StoryScape!
