# PhishGuard
Browser Extension for phishing URL detection
Features:

ML-based phishing classification

Heuristic checks (keywords like login, verify)

Google Safe Browsing & VirusTotal API integration

Instant user alerts for dangerous URLs

Tech Stack:

Frontend: HTML, CSS, JS, Chrome APIs

Backend: Node.js, Express, CORS

ML: Python (Scikit-learn/TensorFlow.js), Pandas, NumPy

Setup:

npm install
pip install pandas scikit-learn requests
# Set API keys in .env
python ml_train.py   # Train ML model
node server.js       # Start server


Load the extension (unpacked) in Chrome

Enter a URL → get instant phishing alert

API: /checkurl (POST)

{ "url": "https://example.com" }


Response:

{ "phishing": true, "ml": "1", "heuristic": true, "vt": true, "google_safe": false }


Future:

Auto-detect active tab URL

Retrain ML model

Regex heuristics

Firefox/Edge support
