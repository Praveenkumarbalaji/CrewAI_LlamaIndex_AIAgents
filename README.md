
<body>
  <h1>Financial Analyst Agent Using CrewAI and LlamaIndex</h1>
  <p>
    This notebook demonstrates a Financial Analyst Agent that leverages CrewAI and LlamaIndex to perform intelligent analysis on financial reports. The agent is designed to extract insights from documents (for example, the Infosys Annual Report) and generate both analytical summaries and engaging blog posts.
  </p>

  <h2>Table of Contents</h2>
  <ul>
    <li><a href="#overview">Overview</a></li>
    <li><a href="#installation">Installation &amp; Dependencies</a></li>
    <li><a href="#setup">Setup &amp; Configuration</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#notebook-structure">Notebook Structure</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
    <li><a href="#license">License</a></li>
  </ul>

  <h2 id="overview">Overview</h2>
  <p>
    The Financial Analyst Agent notebook uses a combination of tools to:
  </p>
  <ul>
    <li>Install and configure required dependencies (including various llama-index packages and CrewAI tools).</li>
    <li>Set up a language model (LLM) with Groq and Langchain for generating responses.</li>
    <li>Download and parse financial documents (e.g., the Infosys Annual Report).</li>
    <li>Build a document index using LlamaIndex and a HuggingFace embedding model.</li>
    <li>Instantiate a query engine, tools, and agents (Researcher and Writer) to analyze the data and generate output.</li>
    <li>Define tasks and execute a workflow (crew) to produce a comprehensive analysis and a blog post.</li>
  </ul>

  <h2 id="installation">Installation &amp; Dependencies</h2>
  <p>
    Before running the notebook, install the required packages. You can install these dependencies using <code>pip</code>:
  </p>
  <pre><code>!pip install llama-index --quiet
!pip install llama-index-llms-groq --quiet
!pip install llama-index-core --quiet
!pip install llama-index-readers-file --quiet
!pip install llama-index-tools-wolfram-alpha --quiet
!pip install llama-index-embeddings-huggingface --quiet
!pip install "crewai[tools]" --quiet
!pip install langchain_openai</code></pre>
  <p>
    These packages support the LLM, indexing, and agent workflows required by the project.
  </p>

  <h2 id="setup">Setup &amp; Configuration</h2>
  <p>
    To get started:
  </p>
  <ul>
    <li>
      Open the notebook in Google Colab using the provided link:
      <br>
      <a href="https://colab.research.google.com/github/Praveenkumarbalaji/CrewAI_LlamaIndex_AIAgents/blob/main/CrewAI_LlamaIndex_AIAgents.ipynb" target="_blank">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
      </a>
    </li>
    <li>Set up your Groq API key in the notebook where prompted.</li>
    <li>Configure any other model parameters as needed (e.g., for the ChatOpenAI instance).</li>
    <li>Ensure you have network access for downloading necessary files (e.g., the Infosys Annual Report).</li>
  </ul>

  <h2 id="usage">Usage</h2>
  <p>
    Once the dependencies are installed and the configuration is complete, run the notebook cells sequentially. The main workflow involves:
  </p>
  <ul>
    <li>Installing required packages.</li>
    <li>Setting up the LLM environment using Groq and Langchain.</li>
    <li>Downloading and parsing the financial document (e.g., <code>infy_nav.pdf</code>).</li>
    <li>Building an index of the document with LlamaIndex using a HuggingFace embedding model.</li>
    <li>Constructing a query engine and instantiating it as a tool.</li>
    <li>Defining and assigning tasks to Researcher and Writer agents.</li>
    <li>Executing the crew workflow to generate an analysis report and a blog post.</li>
  </ul>

  <h2 id="notebook-structure">Notebook Structure</h2>
  <pre>
├── CrewAI_LlamaIndex_AIAgents.ipynb    // Main Jupyter Notebook
└── README.html                         // This README file in HTML format
  </pre>

  <h2 id="acknowledgements">Acknowledgements</h2>
  <p>
    This project is built using open-source libraries including CrewAI, LlamaIndex, and Langchain. Special thanks to the developers of these tools for their contributions.
  </p>

  <h2 id="license">License</h2>
  <p>
    This project is licensed under the MIT License.
  </p>
</body>
</html>

