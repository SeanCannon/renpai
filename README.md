# Ren'Py AI-Driven Proof of Concept Repository

This repository demonstrates a proof of concept for a Ren'Py game with dynamic, AI-generated dialogue and scenes.

## Features
- **Dynamic Dialogue Generation**: Leverages an AI language model to generate dialogue and plot elements based on player choices.
- **AI-Generated Visuals**: Uses AI-generated character images for dynamic poses and scenes (optional).

## Prerequisites

1. **Ren'Py SDK**
   - Download the Ren'Py SDK from [Ren'Py's official website](https://www.renpy.org/).
2. **Python 3.x**
   - Ensure Python 3.x is installed. The game relies on external Python scripts.
3. **OpenAI API** (or any other text-generation API):
   - An API key for OpenAI or another compatible language model.
4. **Stable Diffusion / DALL-E** (optional for dynamic visuals):
   - Ensure you have access to an image-generation model and its API.

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/seancannon/renpai.git
   cd renpy-ai-poc
   ```

2. Install required Python packages:
   ```bash
   pip install openai
   ```

3. Configure the API keys:
   - Add your OpenAI API key to `dynamic_dialogue.py`:
     ```python
     OPENAI_API_KEY = "your_openai_api_key_here"
     ```

4. Open the `project_root` folder in the Ren'Py launcher.

5. Run the game.

## File Structure
```
project_root/
├── game/
│   ├── script.rpy              # Main Ren'Py script
│   ├── dynamic_dialogue.py     # Python script for AI integration
├── README.md                   # This file
```

## Usage
- The game starts with a simple scene.
- Based on the player's choices, the AI generates the next dialogue dynamically.

## Limitations
- **Performance**: Generating content in real-time might introduce delays.
- **Consistency**: AI-generated content may vary in quality.

## Future Work
- Integrate Stable Diffusion for dynamic visuals.
- Expand the story template for more complex branching.
- Fine-tune AI models for better consistency and coherence.

---

Contributions and feedback are welcome! Feel free to open issues or submit pull requests.

