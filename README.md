y# Openai Exploration for Image Generation and Audio Transcriptions (Speech to Text)
The Openai task involves exploring the GPT-3.5 architecture for image generation and audio transcriptions (Speech to Text). 

## Aims
- The aim is to see if the architecture can generate high-quality images based on given text prompts - Further exploration & research are required here.
- Another aim is to see if the architecture can accurately transcript Speech to Test - Which it did!

## How to get OpenAI API keys
- Go to the OpenAI website (https://openai.com/) and click on the "API" tab in the top menu.

- Scroll down to the "Get API Key" section and click on the "Get started for free" button. This will take you to the OpenAI API sign-up page (https://beta.openai.com/signup/).

- Fill in your email address and choose a password to create an account, or signup using your Google account.

- Once you have created an account, log in to the OpenAI API dashboard (https://beta.openai.com/dashboard/).

- In the dashboard, click on the "API Keys" tab in the left-hand menu or use this link (https://platform.openai.com/account/api-keys).

- Click on the "Generate API Key" button to create a new API key.

- Copy the API key to your clipboard and keep it safe. This key will be used to authenticate your requests to the OpenAI API.

- Next, you can use the API key to make requests to the OpenAI API using your preferred programming language or tool. I have used Python Programming Language.

## About the Image Generating function in the Python code that can be found in this repository.
This is a Python function named "Create_images" that uses the OpenAI Image API to generate images based on a given text prompt. It takes one argument, "text," which should be a string representing the text prompt to use for generating the image.

Inside the function, the "openai.Image.create" method is used to create the image. The first argument of this method is the text prompt to use for generating the image, which is passed as the "prompt" parameter. The "n" parameter specifies the number of images to generate (in this case, one). The "size" parameter specifies the size of the generated image(s), which is set to "512x512" in this example.

The generated image(s) are stored in the "res" variable, which is then returned from the function using the "return" statement.

Note that this function requires the OpenAI API keys and the OpenAI SDK to be installed and properly configured in order to work.

## About the Audio Transcription function in the Python code that can be found in this repository
This is a Python function named "Transcribe_speech" that uses the OpenAI Audio API to transcribe speech. It takes one argument, "speech," which should be a string representing the path to the audio file that needs to be transcribed.

Inside the function, the "openai.Audio.transcribe" method is used to perform the transcription. The first argument of this method is the model ID to use for the transcription, which in this case is "whisper-1". The second argument is the actual audio file, which is opened using the built-in "open" function with the "rb" mode (read-binary).

The transcribed text is stored in the "res" variable and then returned from the function using the "return" statement.

Note that this function requires the OpenAI API keys and the OpenAI SDK to be installed and properly configured in order to work...
