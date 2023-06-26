# LLM_Summarizer - Too Lazy to View

## Too Lazy To View
Too Lazy To View is a web application that allows users to summarize content they are too lazy to read or view. The application supports both text and audio/video input, with the ability to transcribe audio files using Whisper. Summaries are generated using OpenAI's GPT-3.5 model. For very long text, summaries will be generated for each segment, and the overall summary will be generated from the concatenation of the segment summaries.

## Getting Started
To use the application, simply open the index.html file in your browser or visit https://troyanovsky.github.io/LLM_Summarizer/

## Prerequisites
The following resources are required to run the application:

A modern web browser (tested on Chrome)  
An internet connection (for loading external libraries and Whisper model)  
An OpenAI API key (to generate summaries)  

## Usage
Upon opening the index page, you can select a file to upload for transcription by clicking the "Choose file" button. If the file is a text-based file, the content will be loaded to the text area; if the file is an audio file, you can click the "Transcribe audio" button to initiate the transcription process. Transcription may take some time depending on the length of the audio file. For the first time transcribing the audio, the application will use the transformer.js library to download the Whisper-tiny model to transcribe your audio. Subsequent transcription will be much faster. All transcription is done locally.

Once the transcription process is complete, the raw text will be displayed in the text area below the buttons. Users can then enter their OpenAI API key in the input field provided and click the "Summarize" button to generate a summary of the text.

## Built With
Vue.js - JavaScript framework used for building user interface  
Tailwind CSS - CSS framework used for styling  
transformers.js - JavaScript library used for machine learning-based speech-to-text transcription  
OpenAI GPT-3.5 model - LLM for generating summaries  

## Author
Troy (Guodong) Zhao - https://github.com/Troyanovsky
