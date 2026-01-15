# IIT-ROPAR-PROJECT
📖 Branched Storyteller

An Interactive, Choice-Driven Narrative Generation Engine

🔍 Project Overview

Branched Storyteller is an interactive storytelling system that generates non-linear narratives where each user decision influences how the story unfolds. Instead of a fixed storyline, the system uses a branching story graph to dynamically traverse different narrative paths based on user choices.

The project demonstrates how graph structures, decision logic, and generative AI can be combined to create immersive, personalized storytelling experiences.

🧩 Architecture Overview (Diagram Explanation)

The architecture is built around a story graph, where narratives evolve through connected decision nodes.

🏗 Core Components
1. Story Graph

Represents the entire story as a directed graph

Each node = one scene

Each edge = a possible user choice

Enables multiple endings and narrative paths

Scene A
 ├── Choice 1 → Scene B
 │              ├── Choice → Scene D
 └── Choice 2 → Scene C
                └── Choice → Scene E

2. Scene Nodes

Each scene node contains:

Narrative text (story content)

Available choices

Metadata (emotion, tone, intensity – optional & extendable)

Example:

scene = {
  "id": "forest_path",
  "text": "You stand at the edge of a silent forest...",
  "choices": ["Enter the forest", "Turn back"]
}

3. Decision Engine

Captures user choice

Maps choice → next scene node

Ensures correct traversal through the story graph

Prevents invalid transitions

4. Story Flow Controller

Maintains current story state

Tracks path history

Handles branching, looping, or termination (endings)

5. Generative Layer (Optional / Extendable)

Enhances static scenes with AI-generated variations

Can adapt:

Emotion

Tone

Length

Supports future upgrades (LLMs, emotion-aware logic)

6. Output Layer

Currently text-based

Easily extendable to:

Image generation

Audio narration

Video storytelling

⚙️ Installation
Prerequisites

Python 3.8+

pip

Setup
# Clone the repository
git clone https://github.com/your-username/branched-storyteller.git
cd branched-storyteller

# Install dependencies
pip install -r requirements.txt

▶️ Running the Demo
python main.py


You will:

Be presented with a story scene

Choose from multiple options

Experience a unique story path based on your decisions

🧪 Example Interaction
You wake up in a quiet village at dawn.

1. Leave the village
2. Stay and explore

Enter your choice:

Each selection leads to a different storyline, environment, and ending.

Terminal interaction screenshots

Story choice prompts

Sample branching paths

Example markdown:

![Story Start](screenshots/start.png)
![Branching Choice](screenshots/choice.png)

🚀 Future Scope

🔮 Planned & Possible Enhancements:

Emotion-aware branching logic

AI-generated scene variations

Image, audio, and video storytelling

Memory-based long-term narratives

Game engine integration

Personalized user storytelling profiles

🎯 Use Cases

Interactive fiction & games

AI narrative simulations

Educational storytelling

Emotional & therapeutic storytelling

Narrative-driven UX experiments

🧠 Key Learnings & Concepts

Graph-based system design

Decision trees & state management

Narrative logic modeling

AI-assisted creative systems
