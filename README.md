🛡️ SecureScan Pro: AI-Powered SAST & Triage Suite

SecureScan Pro is a high-performance, browser-based Static Application Security Testing (SAST) tool. It leverages State-of-the-Art (SOTA) LLMs—including Gemini 3.1 Pro, GPT-5.3, and Claude 3.7 Sonnet to perform deep contextual analysis of entire codebases, identify vulnerabilities, and provide a live triage workflow.

🚀 Key Features

Multi-Engine Support: Switch between Google Gemini, OpenAI (including o1-preview), and Anthropic models seamlessly.
Deep Project Indexing: Uses the File System Access API to map entire project directories while automatically ignoring noise like node_modules and .git.
Visual Risk Dashboard: Generates real-time charts of vulnerability density (Critical, High, Medium, Low).
Interactive Triage Table: Converts AI findings into a live checklist where you can track remediation progress.
Enterprise Reporting: Export full technical audits to formatted PDF documents.
Zero-Server Architecture: All processing happens in your browser and via direct AI API calls. No code is ever stored on an intermediary server.
Persistence: Auto-saves your API keys, model preferences, and triage status using LocalStorage.

🛠️ Getting Started

Prerequisites
To use this tool, you need an API key from at least one of the following providers:

Google AI Studio (Gemini)
OpenAI Platform (GPT-4o / o1)
Anthropic Console (Claude)

Installation
Clone the repository:

Bash
git clone https://github.com/your-username/securescan-pro.git
Open the Tool:
Simply open the index.html file in any modern web browser (Chrome or Edge recommended for File System API support).

📖 How to Use

Configure Engine: Select your preferred AI model and paste your API key into the secure input field.

Load Code:

Click "Map Project Directory" to select your entire source code folder.
SecureScan Pro will index all relevant files (.js, .py, .java, .go, etc.) into the local memory buffer.
Run Audit: Click "Initiate System Audit".
The AI will perform a "Source-to-Sink" analysis, tracing user input to execution points.
Scanning usually takes 30–60 seconds depending on the project size.

Triage Findings:

Review the Risk Chart for an overview of the security posture.
Use the Remediation Triage table to check off vulnerabilities as you fix them in your IDE.
Export: Click "Generate PDF Report" to save a formal audit trail for your team or clients.

🛡️ Security & Privacy

Direct-to-API: This tool communicates directly with the AI providers. There is no backend database.
Local Processing: Project code is stored in your browser's RAM during the session and is cleared upon refresh (unless saved in the report).
Exclusions: By default, the tool ignores .env files and sensitive directories to prevent accidental credential leakage to the AI engines.

📊 Vulnerability Classification

SecureScan Pro follows the OWASP Top 10 and CWE standards to classify findings:

🔴 CRITICAL: Remote Code Execution (RCE), Hardcoded Credentials, Unauthenticated Data Access.
🟠 HIGH: SQL Injection, Broken Access Control, Command Injection.
🟡 MEDIUM: Cross-Site Scripting (XSS), Insecure Headers, CSRF.
🟢 LOW: Informational leaks, Version Disclosure, General Hardening.

🤝 Contributing

Contributions are welcome! If you have ideas for new parsers or UI improvements:

Fork the Project.

Create your Feature Branch (git checkout -b feature/AmazingFeature).
Commit your Changes (git commit -m 'Add some AmazingFeature').
Push to the Branch (git push origin feature/AmazingFeature).

Open a Pull Request.

Disclaimer: SecureScan Pro is an auxiliary tool designed to assist security researchers. It should be used as part of a multi-layered security strategy including manual code review and dynamic testing.
