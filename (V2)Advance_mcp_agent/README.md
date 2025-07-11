# 🚀 Multi-MCP Intelligent Assistant

The Multi-MCP Intelligent Assistant is a powerful productivity tool that integrates multiple Model Context Protocol (MCP) servers to provide seamless access to GitHub, Perplexity, Calendar, and Gmail services through natural language interactions. This advanced AI assistant is powered by Agno's AI Agent framework and designed to be a productivity multiplier across your digital workspace.

## ✨ Features

### Multi-Agent System
- **🐙 GitHub Integration**: Complete repository management, issue tracking, and code analysis
- **🔍 Perplexity Research**: Real-time web search and information gathering
- **📅 Calendar Management**: Event scheduling and meeting coordination
- **📧 Gmail Integration**: Email management and communication workflows

### Core Capabilities
- Repository management (create, clone, fork, search)
- Issue & PR workflow (create, update, review, merge, comment)
- Real-time web search and research
- Event scheduling and availability management
- Email organization and automated responses
- Cross-platform workflow automation

### Advanced Features
- Interactive CLI with streaming responses
- Conversation memory and context retention
- Tool chaining for complex workflows
- Session-specific user and session IDs
- Markdown-formatted responses
- Proactive workflow suggestions

### Productivity Focus
- Cross-platform automation (GitHub issues → Calendar events)
- Research-driven development workflows
- Project management integration
- Documentation and knowledge sharing

## 🛠️ Prerequisites

- Python 3.8 or higher
- Node.js and npm (required for MCP servers)
- OpenAI API Key
- GitHub Personal Access Token
- Perplexity API Key
- Stable internet connection

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
cd awesome-llm-apps/mcp_ai_agents/multi_mcp_agent
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Verify Node.js Installation

```bash
node --version
npm --version
npx --version
```

If Node.js is not installed, download it from [nodejs.org](https://nodejs.org/)

### 4. Set Up API Keys

Create a `.env` file in the project directory with the following variables:

```env
OPENAI_API_KEY=your-openai-api-key
GITHUB_PERSONAL_ACCESS_TOKEN=your-github-token
PERPLEXITY_API_KEY=your-perplexity-api-key
```

#### API Key Sources
- **OpenAI API Key**: https://platform.openai.com/api-keys
- **GitHub Personal Access Token**: https://github.com/settings/tokens
  - Required scopes: `repo`, `user`, and `admin:org`
- **Perplexity API Key**: https://www.perplexity.ai/

### 5. Run the Application

```bash
python multi_mcp_agent.py
```

### 6. Start Interacting

The assistant will:
- Validate your environment variables
- Generate unique user and session IDs
- Initialize connections to all MCP servers
- Start the interactive CLI interface

## 💡 Usage Examples

### GitHub Operations
```
"Show my recent GitHub repositories"
"Create a new issue in my project repo"
"Search for Python code in my repositories"
"Review the latest pull requests"
```

### Research & Information
```
"Search for the latest AI developments"
"What are the trending topics in machine learning?"
"Find documentation for FastAPI"
"Research best practices for microservices"
```

### Calendar Management
```
"Schedule a meeting for next week"
"Show my upcoming appointments"
"Find available time slots for a 2-hour meeting"
```

### Cross-Platform Workflows
```
"Create a GitHub issue and schedule a follow-up meeting"
"Research a topic and create a summary document"
"Find trending repositories and add them to my watchlist"
```

## 🏗️ Architecture

The Multi-MCP Agent leverages:

- **Agno Framework**: For agent orchestration and tool management
- **OpenAI GPT-4o**: As the core language model
- **MCP Servers**: For external service integrations
- **Async Architecture**: For efficient concurrent operations
- **Memory System**: For context retention and conversation history

## 📁 Project Structure

```
multi_mcp_agent/
├── multi_mcp_agent.py    # Main application file
├── requirements.txt      # Python dependencies
├── .env                  # Environment variables (create this)
├── README.md            # Project documentation
└── .env.example         # Environment variables template
```

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `OPENAI_API_KEY` | OpenAI API key for GPT-4o | Yes |
| `GITHUB_PERSONAL_ACCESS_TOKEN` | GitHub token with repo/user/admin:org scopes | Yes |
| `PERPLEXITY_API_KEY` | Perplexity API key for web search | Yes |

### MCP Server Configuration

The application automatically configures MCP servers for:
- GitHub integration
- Perplexity search
- Calendar management
- Gmail integration

## 🎯 Session Management

- **Unique IDs**: Each session generates unique user and session IDs
- **Context Retention**: Conversation history is maintained throughout the session
- **Memory System**: Cross-conversation learning and adaptation
- **Session Control**: Type `exit`, `quit`, or `bye` to end the session

## 🐛 Troubleshooting

### Common Issues

#### Environment Variables Not Found
- Ensure your `.env` file is in the correct directory
- Verify all required API keys are set
- Check for typos in variable names

#### Node.js/MCP Server Issues
- Verify Node.js installation with `node --version`
- Ensure stable internet connection
- Check MCP server logs for connection errors

#### API Key Issues
- Verify API keys are valid and haven't expired
- Check API key permissions and scopes
- Monitor API usage limits

#### Connection Problems
- Ensure stable internet connection
- Check firewall settings
- Verify API endpoint accessibility

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow Python PEP 8 style guidelines
- Add proper error handling and logging
- Include docstrings for all functions
- Test with multiple MCP servers
- Update documentation for new features

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 🙏 Acknowledgements

- [Agno Framework](https://github.com/agno-ai/agno) - AI Agent orchestration
- [OpenAI](https://openai.com/) - Language model provider
- [Model Context Protocol](https://github.com/modelcontextprotocol) - Server integration framework
- [GitHub API](https://docs.github.com/en/rest) - Repository management
- [Perplexity AI](https://www.perplexity.ai/) - Web search capabilities

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/Shubhamsaboo/awesome-llm-apps/issues) page
2. Create a new issue with detailed information
3. Join our community discussions

## 🔮 Future Enhancements

- [ ] Additional MCP server integrations
- [ ] Web-based UI interface
- [ ] Advanced workflow automation
- [ ] Custom plugin development
- [ ] Multi-language support
- [ ] Enterprise authentication
- [ ] Performance analytics dashboard
- [ ] Workflow templates and presets

---

**Note**: The assistant connects to multiple MCP servers using Node.js packages. Ensure you have a stable internet connection and valid API keys for all services. The tool chaining capabilities allow for complex workflows that span multiple platforms, making it a powerful productivity multiplier for developers and professionals.