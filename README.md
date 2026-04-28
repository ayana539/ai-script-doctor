# AI Script Doctor 🎬

An intelligent screenplay analysis tool powered by multi-agent LLMs and RAG (Retrieval-Augmented Generation).

## Overview

AI Script Doctor analyzes screenplays using three specialized AI agents:
1. **Structure Agent** - Analyzes three-act structure, conflicts, and pacing
2. **Dialogue Agent** - Evaluates character voices, subtext, and dialogue quality
3. **Style Agent** - Assesses tone, genre conventions, originality, and clichés

The system uses RAG with ChromaDB to reference classic screenplays from Pulp Fiction, Breaking Bad, Parasite, Shawshank Redemption, and The Godfather.

## Features

✅ Multi-agent LLM analysis  
✅ RAG system with classic screenplay examples  
✅ Three specialized analysis perspectives  
✅ Web interface with Streamlit  
✅ Real-time feedback and recommendations  

## Tech Stack

- **Frontend**: Streamlit
- **LLM**: OpenAI GPT-3.5/GPT-4
- **RAG**: ChromaDB + LangChain
- **Python**: 3.8+

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ayana539/ai-script-doctor.git
cd ai-script-doctor
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Create .env file:
```bash
cp .env.example .env
# Edit .env and add your OpenAI API key
```

5. Run the application:
```bash
streamlit run main.py
```

The application will open at http://localhost:8501

## Usage

1. Upload your screenplay (TXT format)
2. Click "Analyze Script"
3. Receive detailed feedback from three agents:
   - Structure analysis with plot recommendations
   - Dialogue quality assessment with character voice feedback
   - Style analysis with genre and originality insights
4. View RAG examples from classic films

## Project Structure

```
ai-script-doctor/
├── main.py              # Streamlit web application
├── requirements.txt     # Python dependencies
├── .env.example        # Environment variables template
├── README.md           # This file
└── utils/
    ├── __init__.py
    ├── rag_setup.py    # RAG system with ChromaDB
    ├── agents.py       # 3 specialized AI agents
    └── sample_data.py  # Sample screenplays
```

## Environment Variables

- `OPENAI_API_KEY` - Your OpenAI API key (required)

## Contributing

This is an educational project. Feel free to fork and extend!

## License

MIT License - See LICENSE file for details
