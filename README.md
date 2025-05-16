# Smart-Air-Canvas
Smart Air Canvas is an intelligent, gesture-driven interface that redefines human-computer interaction by integrating computer vision, generative AI, and natural language processing. Built on a real-time hand tracking system using Mediapipe and OpenCV, the tool enables users to interact with a digital canvas solely through hand gestures — allowing them to draw, write, solve arithmetic problems, and translate text without any physical input device.

The system captures fingertip coordinates to simulate brush strokes on a virtual canvas. Specific gesture patterns trigger distinct processing modes such as character recognition, shape detection, multilingual translation, part-of-speech tagging, and math solving — all powered by Google’s Gemini 1.5 (GenAI) API. The interface supports audio feedback through text-to-speech (gTTS) and visual feedback using PIL with Devanagari rendering for Hindi and Marathi scripts.

Additionally, the platform includes dynamic UI elements like a gesture-controlled palette, eraser, pen-size selector, upload support, and an archive mode to store and review predictions. Smart Air Canvas embodies a seamless fusion of vision-based input capture, AI reasoning, and multilingual accessibility — designed to explore the future of immersive, contactless interaction.


# 🖐️ Smart Air Canvas

**Smart Air Canvas** is an AI-powered gesture recognition system that allows users to draw, write, solve problems, and translate text — all through simple hand gestures in the air.

> 📰 Published in [JETIR Journal – “Smart Canvas: Redefining Digital Workspaces with Intelligent Gestures”](https://www.jetir.org/view?paper=JETIR2502361)  
> 🏆 2nd Runner-Up – Aavishkar: Maharashtra State Inter-University Research Convention (Engineering – UG)


🚀 Features

- ✍️ Real-time gesture-based drawing & writing
- 🔢 Digit and alphabet recognition using AI
- ➗ Math problem solving via GenAI
- 🌐 English-to-Hindi/Marathi translation
- 🧠 Part-of-Speech (POS) tagging
- 🔊 Text-to-Speech feedback
- 🖌️ Smart UI with pen, eraser, color palette
- 📤 Image upload + archive viewing

## 🎥 Demo

[![Watch the demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://youtu.be/YOUR_VIDEO_ID)

> 📌 *Click to watch the full demo in action*

## 🧠 Tech Stack – How It Powers Smart Air Canvas

🎥 Gesture Detection & Input Processing

| Tool       | Role                                                                 |
|------------|----------------------------------------------------------------------|
| **OpenCV** | Handles real-time webcam feed, canvas overlay, and drawing logic     |
| **Mediapipe** | Detects 21 hand landmarks, enabling gesture classification (draw, predict, erase) |
| **NumPy**  | Creates and manipulates the canvas, blends layers                    |

🖌️ UI Rendering & Controls

| Tool       | Role                                                                |
|------------|---------------------------------------------------------------------|
| **Pygame** | Builds the UI buttons (palette, modes, eraser, archive)             |
| **Tkinter**| Provides file upload dialog                                         |
| **Pillow** | Renders Hindi/Marathi text on canvas using custom Devanagari font   |

🤖 AI & Language Intelligence

| Mode         | Powered by Gemini GenAI (Google)                                   |
|--------------|--------------------------------------------------------------------|
| **Math**     | Solves hand-written arithmetic problems                            |
| **English**  | Recognizes drawn characters/words                                  |
| **POS**      | Classifies part-of-speech for words                                |
| **Shape**    | Detects simple geometric shapes                                    |
| **Translate**| Converts English → Hindi/Marathi with contextual accuracy          |
| **TTS**      | Recognizes text and prepares for audio output                      |

🔊 Speech Output

| Tool     | Role                                                                   |
|----------|------------------------------------------------------------------------|
| **gTTS** | Converts translated output into spoken English                         |
| **Pygame** (Mixer) | Plays back `.mp3` audio using real-time trigger              |

🧠 Logic Layer

- `getUpFingers()` → Maps hand gestures to commands
- Buffers fingertip coordinates for realistic drawing
- Saves input-output pairs to memory for archive review
- Hotkey support (`Q`, `←`, `→`, `E`) to navigate app

## 📬 Contact Details

Want to collaborate or learn more?

- 📧 Email: `anand.ipshika@gmail.com`
- 🔗 [LinkedIn](https://www.linkedin.com/in/ipshika-anand-b4b6b9250/)
