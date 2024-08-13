# Senior-CapStone-Project
Introducing: Abby AI
A Voice-activated assistant with OpenAI Integration

Overview: we'll explore how to create an AI-powered chatbot using Python, OpenAI, and speech recognition.

Research and Planning
Python: Programming language used for development
OpenAI: AI platform for natural language processing
Tkinter: Python GUI toolkit for building the chat interface
SpeechRecognition: Python library for recognizing speech input

We explored available Python libraries for voice recognition, such as SpeechRecognition, and text-to-speech conversion, such as pyttsx3 or gTTS. While discovering different libraries we evaluated each library based on features, ease of use, compatibility, and documentation. And then, implemented voice recognition libraries to capture and transcribe audio commands into responses to create a personable AI system.

Development
1 .We started by setting up / purchasing access to  OpenAI with our API key, allowing us to access their powerful language models. (sk_1234…etc)

2. We then use the SpeechRecognition library to capture user input through speech.
The “listen()” function captures audio input from the microphone and converts it to text.

3. We had to make adjustments for ambient noise to improve recognition accuracy.
“ recognizer.adjust_for_ambient_noise(source, duration=1) ”

4. Afterwards, we leverage OpenAI's ChatCompletion API to generate AI responses based on user input.
Using Function: generate_response() function sends user input to OpenAI's model and retrieves the generated response.

5. We specify model, temperature, max tokens, and other parameters for response generation.
“ response = openai.ChatCompletion.create(…) “

Testing and Refinement
 Our testing process includes both manual and automated tests to identify and address any potential issues or bugs, we create a GUI interface using Tkinter to interact with the chatbot.

Features: Input field for typing messages, chat history display, and send button.
Code: Implementation of the ChatApp class with methods for sending messages and displaying chat history.

User InteractionUsers can choose between starting AbbyAI or AbbyChatbotAI.

AbbyAI: Interactive mode where users can converse with the AI assistant.
AbbyChatbotAI: Chatbot mode where users can type messages and receive AI responses.

After choosing a text-to-speech conversion library that best fits ,we then
integrate the selected library into the project and configure it to convert text into spoken audio.
Test the text-to-speech functionality to ensure accurate vocalization of responses.We've conducted comprehensive testing of our application to ensure its functionality and reliability.
Through rigorous testing, we've identified and resolved various bugs and issues within our application.
By addressing these issues, we've improved the stability and performance of our application, enhancing the overall user experience.

