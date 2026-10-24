<h1>Abel — AI-Assisted Website Troubleshooting Assistant</h1>

<p>
  Abel is a Chrome extension project designed to identify potential website issues,
  explain findings, and help users understand possible fixes. The long-term goal is
  to combine rule-based website diagnostics with local AI-assisted analysis while
  keeping users in control of any changes.
</p>

<h2>Current Features</h2>

<h3>Chrome Extension</h3>
<ul>
  <li>Built with React, TypeScript, Vite, and Tailwind CSS.</li>
  <li>Uses a rule-based scanner to identify website issues.</li>
  <li>Checks areas including metadata, accessibility, images, links, heading structure, and HTML identifiers.</li>
  <li>Classifies findings by severity and type.</li>
  <li>Displays scan results with descriptions and suggested fixes.</li>
  <li>Includes scan history backed by Chrome's local storage, with options to view or delete saved scans.</li>
</ul>

<h3>Local AI Backend — In Progress</h3>
<ul>
  <li>Python-based backend using FastAPI.</li>
  <li>LangChain integration through <code>langchain-ollama</code>.</li>
  <li>Local inference using Ollama and the <code>llama3.2</code> model.</li>
  <li>Implemented a health-check endpoint: <code>GET /api/health</code>.</li>
  <li>Implemented an AI analysis endpoint: <code>POST /api/analyze</code>.</li>
  <li>Designed to explain scanner findings and recommend next steps without automatically modifying websites.</li>
</ul>

<h2>Technology Stack</h2>
<ul>
  <li><strong>Extension frontend:</strong> React, TypeScript, Vite, Tailwind CSS</li>
  <li><strong>Browser platform:</strong> Chrome Extensions Manifest V3</li>
  <li><strong>Scanner:</strong> TypeScript-based rule engine</li>
  <li><strong>Backend:</strong> Python, FastAPI, Uvicorn</li>
  <li><strong>AI orchestration:</strong> LangChain</li>
  <li><strong>Local model runtime:</strong> Ollama</li>
  <li><strong>Language model:</strong> Llama 3.2</li>
  <li><strong>Local scan storage:</strong> Chrome Storage API</li>
</ul>

<h2>Current Development Status</h2>
<ul>
  <li>☑ Build the Chrome extension interface.</li>
  <li>☑ Implement rule-based website scanning.</li>
  <li>☑ Display scanner findings and suggested fixes.</li>
  <li>☑ Add persistent scan history.</li>
  <li>☑ Install Ollama and run the Llama 3.2 model locally.</li>
  <li>☑ Create the FastAPI backend.</li>
  <li>☑ Confirm that the backend health check responds successfully.</li>
  <li>☑ Confirm that the OpenAPI schema is accessible.</li>
  <li>☑ Implement the <code>/api/analyze</code> endpoint.</li>
  <li>☐ Verify end-to-end AI analysis through the API.</li>
  <li>☐ Connect the extension to the AI backend.</li>
  <li>☐ Add AI-generated explanations and prioritization to the extension.</li>
  <li>☐ Test and refine the complete workflow.</li>
</ul>

<h2>Design Principles</h2>
<ul>
  <li><strong>User control:</strong> AI recommendations should be reviewed before any changes are applied.</li>
  <li><strong>Local-first AI:</strong> Use local inference to reduce dependence on hosted AI services.</li>
  <li><strong>Evidence-based explanations:</strong> AI should explain the scanner's findings rather than inventing website issues.</li>
  <li><strong>Incremental development:</strong> Build and verify the scanner, backend, and integration in manageable stages.</li>
</ul>

<h2>Running the AI Backend Locally</h2>

<p>From the project directory:</p>

<pre><code>cd ~/abel/abel-ai
source .venv/bin/activate
uvicorn main:app --host 127.0.0.1 --port 8000</code></pre>

<p>Health check:</p>

<pre><code>curl http://127.0.0.1:8000/api/health</code></pre>

<p>
  The backend currently runs locally and is not yet connected to the Chrome extension.
</p>

<h2>Project Status</h2>
<p><strong>Active development — local AI integration in progress.</strong></p>
