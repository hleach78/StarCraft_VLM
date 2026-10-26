STARCRAFT II VLM AGENT — QUICK SETUP

Requirements:
- Python 3.10
- StarCraft II installed
- Google Gemini API key

Downloads and Links:
- Python: https://www.python.org/downloads/
- StarCraft II: https://starcraft2.blizzard.com/
- Gemini API Key: https://aistudio.google.com/app/apikey
- Original GitHub Repository: https://github.com/camel-ai/VLM-Play-StarCraft2

Packages:

Run these commands from the project root directory:
py -3.10 -m pip install -e . --no-deps
py -3.10 -m pip install -r vlm_attention/requirements.txt
py -3.10 -m pip install google-genai

If you encounter Protobuf compatibility issues, refer to the repository's README for the recommended fix.

Set Gemini API Key (PowerShell):
$env:GEMINI_API_KEY="YOUR_API_KEY_HERE"

Replace `YOUR_API_KEY_HERE` with your own key. Keep the key private.

Run the Project:
py -3.10 vlm_attention/run_env/pure_image_run_game.py

Maps:
The project requires the appropriate StarCraft II map files. If a required map is missing, 
copy the provided map files into the correct StarCraft II Maps folder.

Maps used for testing:
- `ability_test_map`
- `3s_vs_3z_vlm_attention`

For additional setup instructions and troubleshooting, see the GitHub repository linked above.