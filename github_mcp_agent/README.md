# GitHub MCP Agent

A professional-grade Streamlit application for intuitive exploration and analysis of GitHub repositories using natural language queries, powered by the Model Context Protocol (MCP).

## 🚀 Features

### Natural Language Interface
Query repositories in plain English—no technical jargon required.

### Comprehensive Analysis
Explore issues, pull requests, repository activity, and code statistics for a holistic view.

### Interactive UI
User-friendly interface with example queries and customizable input.

### MCP Integration
Leverages the Model Context Protocol to interact seamlessly with the GitHub API.

### Real-Time Results
Receive immediate insights on repository activity and health.

## 📋 Prerequisites

- Python 3.8 or higher
- Node.js and npm (required for MCP GitHub server)
- GitHub Personal Access Token with `repo` and `user` scopes
- OpenAI API Key

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
cd mcp-github-agent
```

### 2. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 3. Verify Node.js and npm Installation

```bash
node --version
npm --version
npx --version
```

If any command fails, download and install Node.js from the [official website](https://nodejs.org/).

### 4. Set Up API Keys

Set your OpenAI API key as an environment variable:

```bash
export OPENAI_API_KEY=your-openai-api-key
```

The GitHub token will be entered directly in the app interface.

### 5. Create a GitHub Personal Access Token

1. Visit [GitHub Tokens](https://github.com/settings/tokens)
2. Generate a token with `repo` and `user` permissions
3. Store the token securely

## 🚀 Usage

### Start the Streamlit App

```bash
streamlit run app.py
```

### Interact with the App

1. Enter your GitHub token in the sidebar
2. Specify the repository you wish to analyze
3. Select a predefined query or enter a custom one
4. Click "Run Query" to view results

## 💡 Example Queries

### Issues
- Show issues by label
- What issues are being actively discussed?
- Find issues labeled as bugs

### Pull Requests
- What PRs need review?
- Show me recent merged PRs
- Find PRs with conflicts

### Repository Analysis
- Show repository health metrics
- Show repository activity patterns
- Analyze code quality trends

## 📁 Project Structure

```
mcp-github-agent/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
├── .env.example          # Environment variables template
└── assets/               # Static assets (if any)
```

## 🔧 Configuration

### Environment Variables

Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your-openai-api-key
GITHUB_TOKEN=your-github-token  # Optional: can be entered in UI
```

### MCP Server Configuration

The application automatically handles MCP server setup for GitHub integration. Ensure you have the necessary permissions for the repositories you want to analyze.

## 🐛 Troubleshooting

### Common Issues

#### Node.js/npm Not Found
- Ensure Node.js is properly installed and added to your PATH
- Restart your terminal after installation

#### GitHub Token Issues
- Verify your token has the correct permissions (`repo`, `user`)
- Check that the token hasn't expired
- Ensure you're using a Personal Access Token, not a GitHub App token

#### OpenAI API Errors
- Verify your OpenAI API key is valid and has sufficient credits
- Check for any rate limiting issues

#### MCP Connection Issues
- Restart the Streamlit application
- Check your internet connection
- Verify GitHub API status

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Setup

```bash
# Install development dependencies
pip install -r requirements-dev.txt

# Run tests
pytest

# Format code
black .
isort .
```

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 🙏 Acknowledgements

- [Streamlit](https://streamlit.io/) - Web application framework
- [GitHub API](https://docs.github.com/en/rest) - Repository data source
- [OpenAI](https://openai.com/) - Natural language processing
- [Model Context Protocol (MCP)](https://github.com/modelcontextprotocol) - API integration framework

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/Shubhamsaboo/awesome-llm-apps/issues) page
2. Create a new issue with detailed information
3. Join our community discussions

## 🔮 Future Enhancements

- [ ] Multi-repository comparison
- [ ] Advanced filtering options
- [ ] Export functionality for reports
- [ ] Integration with additional version control systems
- [ ] Custom dashboard creation
- [ ] Automated report scheduling

---

This application streamlines the process of extracting actionable insights from GitHub repositories, making advanced analysis accessible to both technical and non-technical users.