# Solaris

**An Autonomous AI Agent System with Infinite Context Capability**

Solaris is a desktop-based autonomous AI agent that can complete complex computer and web-based projects with minimal human intervention. Using the innovative RSAU Loop combined with RLM-graph memory architecture, Solaris overcomes AI model context limitations and achieves superior accuracy in long-horizon tasks.

## 🚀 Key Features

### 🧠 **Infinite Context Window**
- **RSAU Loop** (Reason-Search-Act-Update) enables unlimited task length
- **Session Continuation** automatically checkpoints at 85% context usage
- **Fresh Context Windows** prevent context rot and maintain accuracy
- **Executive Summary** provides task continuity across sessions

### 🛠️ **Comprehensive Tool Suite**
- **38 Browser Automation Tools** - Full web interaction capabilities
- **Complete Office Suite** - Word, Excel, PowerPoint generation & manipulation
- **File System Operations** - Read, write, edit, search across projects
- **PDF Operations** - Generate and parse PDF documents
- **Scratchpad System** - Intelligent context offloading

### 🎯 **Multi-Model AI Support**
- **OpenRouter** - Access to 100+ models via single API

### 📚 **Skills & Knowledge**
- **builtin skills and hundreds of load-able Skills** for specialized tasks
- **Knowledge Store** learns from your preferences
- **Reflection System** improves over time

### 🖥️ **Modern Desktop Application**
- **Tauri Framework** - Lightweight, secure, cross-platform
- **React 18 + TypeScript** - Modern, responsive UI
- **Real-time Streaming** - Watch the agent think and work

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

### 📚 **Knowledge Store**
Learns from your interactions:
- **User Preferences** - Coding styles, frameworks, patterns
- **Error Solutions** - Problems encountered and resolved
- **Workflow Patterns** - How you approach tasks
- **Reflection System** - Improves over time

## 🛠️ Tool Capabilities

### 🌐 **Browser Automation** (38 Tools)
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

Solaris includes intelligent HITL for safety:

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

## 📚 Skills System

### 🔧 **Agent Skills** (146 available)
- **Development**: React, Node.js, Python, Rust
- **Data Science**: Pandas, NumPy, Matplotlib
- **Web**: HTML, CSS, JavaScript, APIs
- **Office**: Excel formulas, PowerPoint templates
- **Productivity**: Git, Docker, CI/CD

### 📦 **External Skills**
```bash
# Install community skills
Settings → Skills → Browse Skills → Install
```

### 🎯 **Custom Skills**
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


## 📄 License

Solaris is proprietary software. 

## 🤝 Contributing

We're not accepting external contributions at this time, but we appreciate:
- **Bug Reports**: Please file issues with detailed reproduction steps
- **Feature Requests**: Submit with clear use cases
- **Feedback**: Share your experience and suggestions

---

