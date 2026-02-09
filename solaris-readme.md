# Solaris

<p align="center">
  <img src="solaris.jpg" alt="Solaris Logo" width="200" height="200">
</p>

**Version 3.0 - An Autonomous AI Agent System with Infinite Context Capability**

Solaris is a desktop-based autonomous AI agent that can complete complex computer and web-based projects with minimal human intervention. Using the innovative RSAU Loop combined which is an iteration of the **Recursive Language Model (RLM)** method, combined with **Knowledge Graph (KG)**, Solaris overcomes AI model context limitations and achieves superior accuracy and completeness in long-horizon tasks.

## 🆕 Recent Updates (v3.0)

### 🎨 **AI Image Generation & Analysis**
- Generate images via OpenRouter with Gemini 2.5 Flash, Flux, and more
- Analyze existing images with vision-capable AI models
- Customizable aspect ratios, image sizes, and model selection

### 🔌 **MCP Client & Subagent Support**
- Connect to external Model Context Protocol servers
- Delegate tasks to specialized subagents
- Dynamic tool discovery and namespace management

### 🛑 **Enhanced Control & Safety**
- Real-time stop button with proper cancellation
- Multiple permission modes for different use cases
- Checkpoint timeline safety warnings
- Interactive `ask_user` tool for AI-initiated questions

### 🎯 **UI/UX Improvements**
- Refactored settings page with modular components
- Fixed project display on landing page
- Enhanced skills organization and management
- Improved reference search performance

### 📚 **Enhanced Skills System**
- Upgraded Python office skills with critical rules
- Centralized skills directory location
- Enhanced content creation capabilities
- Creator mode planning for specialized content creation

## 🚀 Key Features

### 🧠 **Infinite Context Window**
- **RSAU Loop** (Reason-Search-Act-Update) with file system as context enables (almost) unlimited context - disregarding the context limit of the underlying AI model.
- **Session Continuation** automatically checkpoints at 85% context usage
- **Fresh Context Windows** prevent context rot and maintain accuracy
- **Executive Summary** provides task continuity across sessions

### 🛠️ **Comprehensive Tool Suite**
- **40+ Browser Automation Tools** - Full web interaction capabilities
- **Complete Office Suite** - Word, Excel, PowerPoint generation & manipulation
- **File System Operations** - Read, write, edit, search across projects
- **PDF Operations** - Generate and parse PDF documents
- **AI Image Generation & Analysis** - Create and analyze images with vision models
- **Scratchpad System** - Intelligent context offloading
- **MCP Client Support** - Connect to external Model Context Protocol servers
- **Subagent System** - Delegate tasks to specialized agents

### 🎯 **Multi-Model AI Support**
- **OpenRouter** - Access to 100+ models via single API
- **AI Image Generation** - OpenRouter integration with Gemini, Flux, and more
- **Vision Models** - Image analysis and understanding capabilities

### 📚 **Skills & Knowledge**
- **builtin skills and hundreds of load-able Skills** for specialized tasks
- **Knowledge Store** learns from your preferences
- **Reflection System** improves over time

### 🖥️ **Modern Desktop Application**
- **Tauri Framework** - Lightweight, secure, cross-platform
- **React 18 + TypeScript** - Modern, responsive UI
- **Real-time Streaming** - Watch the agent think and work
- **Refactored Settings** - Modular, tabbed configuration interface
- **Enhanced Project Management** - Improved landing page and project organization

## 🔄 The RSAU Loop: Breaking Context Barriers

The RSAU (Reason-Search-Act-Update) loop is Solaris's core innovation for handling unlimited task complexity:

### 1. **REASON**
- Think about current state and next steps
- Read executive summary for task context
- Analyze project structure and progress

### 2. **SEARCH**
- Gather context from filesystem
- Retrieve relevant knowledge
- Search for specific information

### 3. **ACT**
- Execute the next action using appropriate tools
- Modify files, interact with web, create documents
- Handle complex multi-step operations

### 4. **UPDATE**
- Update executive summary with progress
- Save important context to scratchpad
- Prepare for next iteration

### 🔄 **Session Continuation**

When context reaches 85% utilization:
1. **Checkpoint Creation** - Full state snapshot saved
2. **Session End** - Clean termination with summary
3. **Fresh Start** - New session with clean context window
4. **Continuation** - Seamlessly resume from checkpoint

This process creates **infinite effective context** while maintaining **high accuracy** by preventing context rot.

## 🧠 RLM-Graph Memory Architecture

Solaris uses a sophisticated multi-tier memory system:

| Tier | Purpose | Location | Lifetime |
|------|---------|----------|----------|
| **Short-term** | Active working context | Thread messages | Session |
| **Medium-term** | Context offloading | `.solaris/scratchpad/` | Project |
| **Long-term** | Planning documents | `.solaris/guide/` | Project |
| **Persistent** | Checkpoints | `.solaris/state/` | Project |
| **Knowledge** | Learned patterns | `.solaris/knowledge/` | Project |

### 🗃️ **Scratchpad System**
Intelligently offloads content from context window:
- `scratchpad_write` - Save research findings, large content
- `scratchpad_read` - Retrieve when needed
- Automatic summaries keep context lean

### 📚 **Knowledge Store** (In development)
Learns from your interactions:
- **User Preferences** - Coding styles, frameworks, patterns
- **Error Solutions** - Problems encountered and resolved
- **Workflow Patterns** - How you approach tasks
- **Reflection System** - Improves over time

## 🛠️ Tool Capabilities

### 🌐 **Browser Automation** (40+ Tools)
- Navigation and content extraction
- Form filling and submission
- Multi-tab management
- Cookie and authentication handling
- Screenshot capture
- PDF printing from web

### 📊 **Office Suite**
- **Word Documents** (.docx) - Create, read, modify
- **Excel Spreadsheets** (.xlsx) - Full read/write with charts
- **PowerPoint** (.pptx) - 100+ shapes, tables, charts
- **PDF Operations** - Generate and parse documents

### 📁 **File Management**
- Read, write, edit files
- Directory operations
- Search and grep across projects
- File system monitoring

### 🎯 **Specialized Tools**
- Planning and executive summary management
- Tool discovery and search
- Skills loading and execution
- Human-in-the-loop approvals
- **AI Image Generation** - Create images via OpenRouter with customizable parameters
- **AI Image Analysis** - Analyze images with vision-capable models
- **ask_user Tool** - AI can ask questions and get user feedback
- **MCP Client** - Connect to external Model Context Protocol servers
- **Subagent Delegation** - Delegate tasks to specialized subagents

## 🚀 Installation

### 📦 **Download Installer**
Download the installer - Install - Use
* Currently only Windows is supported

### ⚙️ **Installation Steps**
1. Run the downloaded installer
2. Follow the installation wizard
3. Launch Solaris from your applications

### 🔑 **API Key Setup**
1. Open Solaris Settings
2. Add your AI provider API keys

## 🎯 Quick Start

### 1. **Create a New Project**
```
File → New Project → Choose directory
```

### 2. **Configure AI Model**
```
Settings → AI Provider → Select model
```

### 3. **Start Your First Task**
```
Chat Panel: "Build a REST API for task management"
```

### 4. **Watch Solaris Work**
- Real-time agent activity display
- Tool execution monitoring
- Context usage tracking
- Session continuation when needed

## 📖 Usage Examples

### 💻 **Software Development**
```
"Create a React TypeScript application with user authentication,
including login, registration, and dashboard with user profile."
```

### 📊 **Data Analysis**
```
"Analyze the sales data in sales.xlsx, create charts showing
monthly trends, and generate a PowerPoint presentation for stakeholders."
```

### 🌐 **Web Research**
```
"Research the latest AI trends, compile findings into a structured
report, and create a summary document with key insights."
```

### 📝 **Document Generation**
```
"Create a comprehensive project proposal document including
timeline, budget estimates, and risk analysis."
```

## 🔧 Configuration

### 🎛️ **Agent Settings**
- **Max Iterations**: 100 (default)
- **Context Threshold**: 85% (triggers checkpoint)
- **Streaming**: Enabled for real-time updates
- **HITL**: Human-in-the-loop for dangerous actions
- **Permission Modes**: Default, AcceptEdits, Plan, BypassAll
- **RALPH Mode**: Auto-resume capability for autonomous completion
- **Stop Button**: Real-time agent cancellation with proper cleanup

### 🧠 **Memory Settings**
- **Scratchpad Size**: Unlimited
- **Knowledge Retention**: Permanent
- **Checkpoint History**: 50 sessions
- **Reflection Interval**: Every 10 tasks

### 🌐 **Provider Settings**
- **Primary Model**: Choose your preferred AI
- **Fallback Models**: Automatic failover
- **Cost Tracking**: Real-time token usage
- **Rate Limits**: Respect provider limits
- **Image Generation Model**: Dedicated model selection for image creation
- **OpenRouter Integration**: Access to 100+ models including vision and image generation

## 🏢 System Requirements

### 💻 **Minimum Requirements**
- **OS**: Windows 10+
- **RAM**: 8GB (16GB recommended)
- **Storage**: 500MB free space
- **Network**: Internet connection for AI services

### 🚀 **Recommended Requirements**
- **OS**: Windows 11
- **RAM**: 16GB+ (for large projects)
- **Storage**: 2GB+ (for projects and knowledge)
- **Network**: Stable broadband connection

## 🔒 Security & Privacy

### 🛡️ **Local Processing**
- All project files remain on your device
- API keys encrypted and stored locally
- No data sent to external servers except AI API calls

### 🔐 **API Key Security**
- AES-256 encryption for stored keys
- Secure key derivation function
- No plaintext key storage

### 🚫 **Sandboxing**
- File access limited to project directories
- Browser operations in isolated Chrome instance
- Tool execution with permission checks

## 🤝 Human-in-the-Loop (HITL)

Solaris includes intelligent HITL for safety and collaboration:

### ⚠️ **Dangerous Actions**
- File deletions outside project
- System-level operations
- Network requests to unknown domains
- Large financial transactions

### ✅ **Approval Workflow**
1. Agent detects dangerous action
2. Approval dialog appears with details
3. User reviews and approves/denies
4. Agent proceeds based on decision

### 🗣️ **Interactive Features**
- **ask_user Tool**: AI can ask questions with 2-4 options
- **Multi-select Support**: Complex decision making
- **Context-aware Questions**: Relevant to current task
- **Fast Response**: 500ms polling for immediate feedback

## � Advanced Features

### 🎨 **AI Image Generation & Analysis**
- **Generate Images**: Create images via OpenRouter with models like Gemini 2.5 Flash, Flux
- **Customizable Parameters**: Aspect ratio, image size, model selection
- **Image Analysis**: Analyze existing images with vision-capable models
- **Integration**: Seamlessly integrate AI-generated images into documents and graphics

### 🔌 **MCP (Model Context Protocol) Support**
- **External Tool Integration**: Connect to MCP servers for extended capabilities
- **Configuration Management**: CRUD operations for MCP server settings
- **Dynamic Tool Loading**: Automatically discover and load MCP tools
- **Namespace Support**: Organized tool naming with server prefixes

### 🤖 **Subagent System**
- **Task Delegation**: Delegate specialized tasks to subagents
- **Filesystem-based Definitions**: Store subagent configurations in `.solaris/agents/`
- **YAML Frontmatter**: Structured subagent definitions
- **Specialized Expertise**: Domain-specific subagents for complex tasks

### 🛑 **Enhanced Control & Safety**
- **Real-time Stop Button**: Cancel agent execution with proper cleanup
- **CancellationToken**: Rust-based cancellation system
- **Checkpoint Timeline Safety**: Warnings for newer checkpoints when resuming
- **Permission Modes**: 
  - `Default`: Standard HITL checks
  - `AcceptEdits`: Auto-accept file operations
  - `Plan`: Planning-only mode
  - `BypassAll`: Skip all permissions

### 🎯 **Creator Mode (Planned)**
- **Content Creation Specialist**: Focus on graphics, documents, presentations
- **Python-First Approach**: Direct Python execution for content creation
- **Sandboxed Coding**: All code execution in `.solaris/creator_code/`
- **Skill-Guided Workflows**: Proven patterns for professional outputs

## � Skills System

### 🔧 **Agent Skills** (146+ available)
- **Development**: React, Node.js, Python, Rust
- **Data Science**: Pandas, NumPy, Matplotlib
- **Web**: HTML, CSS, JavaScript, APIs
- **Office**: Enhanced Excel, PowerPoint, Word, PDF patterns with critical rules
- **Productivity**: Git, Docker, CI/CD
- **Content Creation**: Algorithmic art, brand guidelines, canvas design
- **Creator Skills**: Specialized skills for graphics, posters, infographics

### 📦 **External Skills**
```bash
# Install community skills
Settings → Skills → Browse Skills → Install
```

### 🎯 **Custom Skills** (In development )
Create your own skills with simple YAML format:
```yaml
---
name: "my-custom-skill"
description: "Does something specific"
category: "custom"
tools:
  - name: "my_tool"
    description: "Tool description"
    parameters:
      type: "object"
      properties:
        input:
          type: "string"
---
# Implementation details...
```

## 📊 Performance Monitoring

### 📈 **Real-time Metrics**
- **Token Usage**: Input/output tokens per iteration
- **Cost Tracking**: Estimated cost in USD
- **Context Utilization**: Percentage of context window used
- **Session Count**: Number of RSAU sessions used

### 🎯 **Optimization Features**
- **Smart Context Management**: Automatic offloading
- **Cost Optimization**: Model routing based on task complexity
- **Performance Tuning**: Adaptive iteration limits

## 🐛 Troubleshooting

### 🔧 **Common Issues**

#### **Context Window Full**
- Solution: Solaris automatically creates checkpoint
- Manual: Use scratchpad tools to offload content

#### **API Rate Limits**
- Solution: Switch to different provider/model
- Prevention: Configure rate limits in settings

#### **Browser Automation Fails**
- Solution: Check Chrome installation
- Update: Ensure Chrome is updated to latest version

#### **File Permission Errors**
- Solution: Run as administrator (Windows)
- Check: Ensure project directory is writable

#### **Stop Button Not Working**
- Solution: Use the enhanced stop button with proper cancellation
- Fixed: Real-time cancellation with CancellationToken support

#### **Project Display Issues**
- Solution: Fixed landing page to show correct project names
- Update: Projects now display directory names instead of default "New Project"

#### **Settings Page Performance**
- Solution: Refactored from monolithic 800+ lines to modular components
- Improvement: Tabbed interface with separate configuration sections

#### **Skills Not Loading**
- Solution: Skills moved to central location at `~/solaris/skills/`
- Fix: No longer appear in project file references


## 📄 License

Solaris is proprietary software. 

## 🤝 Contributing

We're not accepting external contributions at this time, but we appreciate:
- **Bug Reports**: Please file issues with detailed reproduction steps
- **Feature Requests**: Submit with clear use cases
- **Feedback**: Share your experience and suggestions

---

