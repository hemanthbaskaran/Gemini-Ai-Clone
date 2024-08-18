# 🌟 Gemini React Application

## 🚀 Overview

Welcome to the **Gemini** React application! This project provides an interactive interface where users can input prompts, receive AI-generated responses, and view recent interactions. The application leverages Google's Generative AI API to deliver rich, engaging responses based on user input.

### 🌐 Live Demo

Check out the live version of the Gemini React application: [**Gemini React App**](https://poetic-sunburst-e73fb4.netlify.app/)

Explore the features and see how the application works in real-time!

## 🧩 Components

### 1. `ContextProvider`
The `ContextProvider` manages the global state of the application using the React `useContext` API. Here's what it tracks:

- **📝 `input`**: The current user input.
- **📌 `recentPrompt`**: The latest prompt submitted by the user.
- **🕒 `prevPrompts`**: A history of past prompts.
- **👁️ `showResult`**: Whether the generated result is displayed.
- **⏳ `loading`**: Indicates if a response is being generated.
- **💬 `resultData`**: The generated response content.

Key functions include:
- **✉️ `onSent`**: Handles the submission of prompts, retrieves responses from the AI, and updates the state.
- **🔄 `newChat`**: Resets the interface for a new conversation.

### 2. `Sidebar`
The `Sidebar` component provides navigation and utility options:

- **📂 Recent**: Displays a list of past prompts for quick access.
- **➕ New Chat**: Starts a new conversation.
- **❓ Help**, **🕒 Activity**, **⚙️ Settings**: Additional options for managing the application.

Key features:
- **🔄 Toggleable Menu**: Expand or collapse the menu.
- **🔄 Load Prompt**: Reload previous prompts with a click.

### 3. `Main`
The `Main` component is where the interaction happens. Depending on the state, it can display:

- **👋 Greeting**: A welcome message when no prompt has been submitted.
- **💡 Suggestion Cards**: Predefined suggestions for users to choose from.
- **📄 Result Display**: The AI-generated response, formatted for readability.

## 🤖 Integration with Google's Generative AI API

This application integrates with Google's **Generative AI SDK** to provide intelligent responses to user prompts.

### 📦 Installation

To use the Google Generative AI SDK, first install the package:

```bash
$ npm install @google/generative-ai
