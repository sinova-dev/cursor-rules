# MCP (Model Context Protocol) - Professional Development Tools

> **Enterprise-Level AI Development Tools & Extensions for Modern Software Development**

This directory contains comprehensive MCP (Model Context Protocol) server configurations designed to enhance your AI-powered development workflow. These tools extend the capabilities of AI assistants like Cursor, providing access to external services, advanced thinking capabilities, and specialized development tools.

## 🎯 What is MCP (Model Context Protocol)?

MCP is a standardized protocol that enables AI assistants to securely connect to external tools and services. It acts as a bridge between your AI coding assistant and various development tools, APIs, and services, significantly expanding what your AI can do for you.

## 🚀 Key Benefits for Developers

### **Enhanced AI Capabilities**

- ✅ Access to real-time web information and documentation
- ✅ Advanced reasoning and problem-solving capabilities
- ✅ Integration with design tools and external APIs

### **Improved Development Workflow**

- ✅ Seamless integration with existing development tools
- ✅ Context-aware assistance with external data
- ✅ Enhanced debugging and problem-solving capabilities

### **Professional Development Tools**

- ✅ Integration with design systems and Figma
- ✅ Advanced thinking and reasoning capabilities
- ✅ Browser automation and web interaction tools

## 📚 Available MCP Servers

### 🔧 **Core Development Tools**

#### **Context7** - Documentation & Library Access

- **Purpose**: Real-time access to comprehensive documentation for thousands of libraries and frameworks
- **Capabilities**: Latest library documentation, API references, code examples, and best practices
- **Use Cases**: Research libraries, get up-to-date documentation, find code examples

#### **Sequential Thinking** - Advanced Reasoning

- **Purpose**: Enhanced problem-solving with step-by-step analysis and logical reasoning
- **Capabilities**: Break down complex problems, systematic debugging, algorithm design
- **Use Cases**: Complex algorithm design, debugging, architectural decisions

#### **Next.js DevTools MCP** - Next.js Development Integration

- **Purpose**: Real-time integration with Next.js 16+ development server for live debugging and development
- **Capabilities**: Error detection, live state queries, page metadata, Server Actions inspection, Next.js documentation
- **Use Cases**: Debug Next.js apps, analyze errors, query application state, access Next.js best practices

#### **Browser Tools** - Web Automation

- **Purpose**: Advanced browser monitoring, interaction, and auditing capabilities
- **Capabilities**: Web scraping, form automation, performance/SEO audits, screenshot capture
- **Use Cases**: Automated testing, data extraction, web research, accessibility audits

### 🎨 **Design & Collaboration Tools**

#### **Framelink Figma MCP** - Design Integration

- **Purpose**: Advanced Figma integration for seamless design-to-code workflows
- **Capabilities**: Design file access, asset extraction, design token management, component analysis
- **Use Cases**: Implementing designs, extracting assets, maintaining design consistency

#### **Figma Dev Mode MCP** - Official Figma Integration

- **Purpose**: Official Figma Dev Mode MCP Server for direct design-to-code workflows
- **Capabilities**: Code generation from frames, design token extraction, Code Connect integration
- **Use Cases**: Generate React code, extract design tokens, reuse existing components

### 🐛 **Debugging & Issue Tracking Tools**

#### **Jam MCP** - Bug Analysis & Issue Tracking

- **Purpose**: Advanced bug analysis and issue tracking with video recordings and user session data
- **Capabilities**: Video analysis, console logs, network requests, user events, screenshot analysis
- **Use Cases**: Debug issues, analyze user behavior, track bugs with full context

## 🛠️ MCP Server Descriptions

### **Context7** - Documentation & Library Access

**Purpose**: Context7 provides AI assistants with access to comprehensive, up-to-date documentation for thousands of libraries and frameworks. This MCP server is essential for modern development workflows.

**Key Benefits**:

- Latest library documentation and API references
- Code examples and best practices
- Version information and migration guides
- Real-time access to official documentation
- Framework-specific examples and patterns

**Quick Setup**: No API keys required, works out of the box with Node.js 18+

#### **Complete Setup Process**

##### **Step 1: Configuration**

Add to your `mcp.json`:

```json
{
  "mcpServers": {
    "context7": {
      "command": "npx",
      "args": ["-y", "@upstash/context7-mcp"]
    }
  }
}
```

##### **Step 2: Verification**

- **Restart your IDE** after configuration
- **Test with documentation queries** in your AI assistant
- **Verify Context7 tools are available**

#### **Advanced Capabilities**

- **Library Documentation**: Access to thousands of libraries and frameworks
- **Code Examples**: Practical implementation examples and snippets
- **API References**: Complete API documentation with parameters and return types
- **Version Information**: Current and historical version details
- **Best Practices**: Community-approved usage patterns and recommendations
- **Migration Guides**: Framework upgrade and migration assistance

#### **Usage Examples**

```markdown
# Documentation Research:

"Research the latest React 19 features using Context7"
"Get Next.js 15 documentation and examples"
"Find Tailwind CSS v3.4 examples and best practices"

# Framework-Specific Queries:

"Show me Vue 3 Composition API examples"
"Get Django REST framework documentation"
"Find Prisma ORM query examples"

# Migration and Updates:

"Help me migrate from React 18 to React 19"
"Show me Next.js 14 to 15 migration guide"
"Get TypeScript 5.0 new features documentation"

# Best Practices:

"Show me React performance optimization best practices"
"Get Next.js SEO best practices"
"Find Tailwind CSS responsive design patterns"
```

#### **Resources**

- [GitHub Repository](https://github.com/upstash/context7-mcp)
- [Video Tutorial](https://www.youtube.com/watch?v=qZfENAPMnyo)
- [Context7 Documentation](https://github.com/upstash/context7-mcp)

---

### **Sequential Thinking** - Advanced Reasoning

**Purpose**: Enhanced problem-solving with step-by-step analysis and logical reasoning capabilities for complex development challenges.

**Key Benefits**:

- Break down complex problems into manageable steps
- Systematic debugging and architecture planning
- Algorithm design and code review assistance
- Logical reasoning and decision-making processes
- Hypothesis testing and solution validation
- Reflection and revision of thinking processes

**Quick Setup**: No dependencies required, works offline

#### **Complete Setup Process**

##### **Step 1: Configuration**

Add to your `mcp.json`:

```json
{
  "mcpServers": {
    "sequential-thinking": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-sequential-thinking"]
    }
  }
}
```

##### **Step 2: Verification**

- **Restart your IDE** after configuration
- **Test with complex problem queries** in your AI assistant
- **Verify Sequential Thinking tools are available**

#### **Advanced Capabilities**

- **Step-by-Step Analysis**: Break down complex problems into manageable steps
- **Logical Reasoning**: Structured approach to problem-solving
- **Decision Trees**: Visual representation of decision processes
- **Hypothesis Testing**: Systematic approach to testing solutions
- **Reflection & Revision**: Ability to review and refine thinking processes
- **Problem Decomposition**: Breaking complex problems into smaller, manageable parts

#### **Usage Examples**

```markdown
# Algorithm Design:

"Use sequential thinking to design a caching strategy for our API"
"Break down this complex algorithm into steps"
"Design an efficient data structure for this use case"

# Debugging and Analysis:

"Analyze the performance implications of this database query"
"Debug this complex state management issue step by step"
"Identify the root cause of this memory leak"

# Architecture Planning:

"Plan the architecture for a microservices system"
"Design a scalable authentication system"
"Break down the requirements for this feature"

# Code Review:

"Review this complex function for potential issues"
"Analyze the security implications of this code"
"Suggest improvements for this algorithm"
```

#### **Resources**

- [GitHub Repository](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking)
- [Video Tutorial](https://www.youtube.com/watch?v=RCFe1L9qm3E)
- [Sequential Thinking Documentation](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking)

---

### **Browser Tools** - Web Automation

**Purpose**: Advanced browser monitoring, interaction, and auditing capabilities with Chrome extension integration.

**Key Benefits**:

- Automated web testing and data extraction
- Performance, SEO, and accessibility audits
- Screenshot capture and web research
- Console log monitoring and network traffic analysis
- NextJS-specific auditing capabilities

**Quick Setup**: Requires Chrome extension + two servers (complex setup)

#### **Complete Setup Process**

Browser Tools MCP requires **three components** to work properly:

##### **Step 1: Install Chrome Extension**

1. Download the Chrome extension from: [v1.2.0 BrowserToolsMCP Chrome Extension](https://github.com/AgentDeskAI/browser-tools-mcp)
2. Install it in your Chrome browser
3. Enable the extension

##### **Step 2: Install MCP Server (for your IDE)**

Add to your `mcp.json`:

```json
{
  "mcpServers": {
    "browser-tools": {
      "command": "npx",
      "args": ["-y", "@agentdeskai/browser-tools-mcp@latest"],
      "autoStart": true
    }
  }
}
```

##### **Step 3: Run Local Node Server**

Open a **new terminal** and run:

```bash
npx @agentdeskai/browser-tools-server@latest
```

**Important**: Keep this terminal running - this is the middleware server that connects everything.

##### **Step 4: Enable Browser Tools Panel**

1. Open Chrome DevTools (F12)
2. Look for the **"BrowserToolsMCP"** panel
3. Click on it to access the tools

#### **Troubleshooting Setup**

If you encounter issues:

1. **Close Chrome completely** (not just the window, but all Chrome processes)
2. **Restart the local node server** (browser-tools-server)
3. **Make sure only ONE instance** of Chrome DevTools is open
4. **Check that both servers are running**:
   - MCP server in your IDE
   - Node server in terminal

#### **Architecture Overview**

```
┌─────────────┐     ┌──────────────┐     ┌───────────────┐     ┌─────────────┐
│  MCP Client │ ──► │  MCP Server  │ ──► │  Node Server  │ ──► │   Chrome    │
│  (Cursor)   │ ◄── │  (Protocol   │ ◄── │ (Middleware)  │ ◄── │  Extension  │
│             │     │   Handler)   │     │               │     │             │
└─────────────┘     └──────────────┘     └───────────────┘     └─────────────┘
```

#### **Advanced Features (v1.2.0)**

- **Accessibility Audits**: WCAG compliance checks
- **Performance Audits**: Lighthouse-driven analysis
- **SEO Audits**: On-page SEO optimization
- **NextJS Audits**: Framework-specific improvements
- **Auto-Paste Screenshots**: Direct integration with Cursor
- **Debugger Mode**: Comprehensive debugging tools

#### **Usage Examples**

```markdown
# Basic Web Interaction:

"Take a screenshot of this page"
"Scrape data from this website"
"Fill out this form with test data"

# Advanced Auditing:

"Run an accessibility audit on this page"
"Check the performance of this page"
"Run an SEO audit"
"Enter audit mode"
"Run a NextJS audit"

# Debugging:

"Enter debugger mode"
"Monitor console logs"
"Check network traffic"
```

#### **Prerequisites**

- Chrome or Chromium browser installed
- Node.js 18+ installed
- Internet connection for web interactions
- Chrome extension installed and enabled
- Two separate servers running (MCP + Node middleware)

#### **Resources**

- [GitHub Repository](https://github.com/AgentDeskAI/browser-tools-mcp)
- [Official Documentation](https://browsertools.agentdesk.ai/installation)
- [Chrome Extension Download](https://browsertools.agentdesk.ai/installation)
- [Video Tutorial](https://www.loom.com/share/88f493eb9c114d3b901ea97e9251e5e6?sid=241311b6-b2a7-4b2d-9b6c-70c0f64f8062)

---

### **Framelink Figma MCP** - Design Integration

**Purpose**: Advanced Figma integration for seamless design-to-code workflows with comprehensive design system access.

**Key Benefits**:

- Access to design files and component libraries
- Asset extraction and design token management
- Real-time collaboration with design teams
- Design system documentation generation
- Component specification extraction
- Style guide automation

**Quick Setup**: Requires Figma API key and account access

#### **Complete Setup Process**

##### **Step 1: Get Figma API Key**

1. Go to [Figma Developer Settings](https://www.figma.com/developers/api#authentication)
2. Generate a personal access token
3. Copy the token for environment setup

##### **Step 2: Environment Configuration**

```bash
# Set your Figma API key
export FIGMA_API_KEY="your_figma_api_key_here"
```

##### **Step 3: MCP Configuration**

Add to your `mcp.json`:

```json
{
  "mcpServers": {
    "Framelink Figma MCP": {
      "command": "cmd",
      "args": ["/c", "npx", "-y", "figma-developer-mcp", "--stdio"],
      "env": {
        "FIGMA_API_KEY": "${FIGMA_API_KEY}"
      }
    }
  }
}
```

#### **Advanced Capabilities**

- **Design Token Extraction**: Automatically extract colors, typography, spacing, and other design tokens
- **Component Analysis**: Get detailed component specifications, variants, and properties
- **Asset Management**: Download and organize design assets in various formats
- **Design System Documentation**: Generate comprehensive style guides from Figma files
- **Code Generation**: Convert design tokens to CSS/SCSS variables
- **Collaboration Tools**: Real-time sync with design team changes

#### **Usage Examples**

```markdown
# Design Token Extraction:

"Extract all colors from this Figma file"
"Get the typography scale from this design system"
"Export spacing tokens as CSS variables"

# Component Analysis:

"Get component specifications for this button"
"Analyze the variants of this card component"
"Extract component properties and states"

# Asset Management:

"Download all icons from this Figma file"
"Export images in different formats and sizes"
"Generate a style guide from this design system"

# Design System Workflow:

"Create CSS variables from these design tokens"
"Generate a component library documentation"
"Sync design changes with development workflow"
```

#### **Prerequisites**

- Figma account with appropriate permissions
- Figma API key (personal access token)
- Node.js 18+ installed
- Internet connection for Figma API access
- Access to Figma files you want to integrate

#### **Resources**

- [GitHub Repository](https://github.com/GLips/Figma-Context-MCP)
- [Official Documentation](https://www.framelink.ai/docs/quickstart)
- [Figma API Documentation](https://www.figma.com/developers/api)
- [Video Tutorial](https://www.youtube.com/watch?v=6G9yb-LrEqg)

---

### **Figma Dev Mode MCP** - Official Figma Integration

**Purpose**: Official Figma Dev Mode MCP Server for seamless design-to-code workflows with direct Figma desktop app integration.

**Key Benefits**:

- Generate code from selected frames and components
- Extract design context with variables and layout data
- Code Connect integration for component reuse
- Real-time design system access
- Asset management with local image server
- Component specification extraction

**Quick Setup**: Requires Figma desktop app + Dev Mode access (Professional/Organization/Enterprise plans)

#### **Complete Setup Process**

##### **Step 1: Enable MCP Server in Figma**

1. **Download Figma Desktop App** (required - web version not supported)
2. **Open Figma Design file**
3. **Go to Figma menu → Preferences**
4. **Enable "Enable local MCP Server"**
5. **Confirm server is running at `http://127.0.0.1:3845/mcp`**

##### **Step 2: Configure Your IDE**

Add to your `mcp.json`:

```json
{
  "mcpServers": {
    "Figma": {
      "url": "http://127.0.0.1:3845/mcp"
    }
  }
}
```

##### **Step 3: Verify Connection**

- **Restart your IDE** after configuration
- **Test with `#get_code`** command in your AI assistant
- **Check that Figma MCP tools are available**

#### **Advanced Features**

- **Code Generation**: Convert Figma frames to React + Tailwind code
- **Design Token Extraction**: Access variables, colors, typography, spacing
- **Component Analysis**: Get detailed specifications and variants
- **Asset Management**: Download images and SVGs with local server
- **Code Connect Integration**: Reuse existing components from your codebase
- **Multi-Selection Support**: Work with multiple frames or entire pages

#### **Usage Methods**

##### **Selection-Based Workflow**

1. **Select frame/layer in Figma desktop app**
2. **Prompt your AI assistant**: "Generate code for my current selection"
3. **Get structured React + Tailwind output**

##### **Link-Based Workflow**

1. **Copy Figma frame/layer link**
2. **Prompt your AI assistant**: "Generate code for this design: [paste link]"
3. **AI extracts node-id and generates code**

#### **Available Tools**

- **`get_code`**: Generate React + Tailwind code from selection
- **`get_metadata`**: Get XML representation with layer properties
- **`get_variable_defs`**: Extract design tokens and variables
- **`get_code_connect`**: Access Code Connect mappings for component reuse

#### **Usage Examples**

```markdown
# Code Generation:

"Generate React code from my current Figma selection"
"Create a Next.js component from this frame"
"Convert this design to Tailwind CSS"

# Design Token Extraction:

"Extract all design tokens from this component"
"Get the color variables used in this frame"
"Export typography scale as CSS variables"

# Component Analysis:

"Get component specifications for this button"
"Analyze the variants of this card component"
"Extract component properties and states"

# Code Connect Integration:

"Use our existing Button component from the design system"
"Generate code that reuses components from our codebase"
"Connect this design to our component library"
```

#### **Resources**

- [Official Documentation](https://help.figma.com/hc/en-us/articles/32132100833559-Guide-to-the-Dev-Mode-MCP-Server)
- [Code Connect Guide](https://help.figma.com/hc/en-us/articles/360040328273)
- [Figma Desktop App Download](https://www.figma.com/downloads/)
- [Video Tutorial](https://www.youtube.com/watch?v=yO3Wr7DEWF0)

---

### **Jam MCP** - Bug Analysis & Issue Tracking

**Purpose**: Advanced bug analysis and issue tracking with comprehensive video recordings, user session data, and debugging context for faster issue resolution.

**Key Benefits**:

- Video analysis of user sessions and bug reproduction
- Console logs and network request monitoring
- User event tracking and interaction analysis
- Screenshot analysis for visual debugging
- Automated bug report generation
- Customer support integration

**Quick Setup**: No API keys required, works with existing Jam recordings

#### **Complete Setup Process**

##### **Step 1: Record a Jam**

1. **Install Jam Chrome Extension** from [jam.dev](https://jam.dev)
2. **Hit Record** to capture your screen and voice
3. **Stop the recording** and get your Jam link
4. **Share the Jam link** with your AI assistant

##### **Step 2: Configure MCP**

Add to your `mcp.json`:

```json
{
  "mcpServers": {
    "jam": {
      "url": "https://mcp.jam.dev/mcp"
    }
  }
}
```

##### **Step 3: Authentication**

1. **Paste Jam link** into your AI assistant
2. **Authenticate with Jam** when prompted
3. **Approve tool requests** from the agent
4. **Start debugging** with full context

#### **Advanced Capabilities**

- **Video Analysis**: AI-powered analysis of recorded user sessions
- **Console Logs**: Access to all console logs and error messages
- **Network Requests**: Complete network traffic analysis with request/response data
- **User Events**: Detailed tracking of clicks, inputs, and navigation
- **Screenshot Analysis**: Visual debugging with screenshot data
- **Bug Context**: Full reproduction context for faster debugging

#### **Available Tools**

- **`getDetails`**: Quick snapshot of the Jam with metadata
- **`getConsoleLogs`**: Access to all console logs from the session
- **`getNetworkRequests`**: Network traffic analysis as JSON
- **`getScreenshot`**: Screenshot data for visual debugging
- **`getUserEvents`**: User interaction tracking in plain language
- **`analyzeVideo`**: AI-powered video analysis for insights and issues

#### **Usage Examples**

```markdown
# Bug Analysis:

"Review this Jam and analyze the problem, cross-reference with the codebase"
"Debug this issue using the Jam recording context"
"Analyze the user behavior in this session"

# Customer Support:

"Analyze these customer Jams and create bug reports"
"Review user feedback and identify common issues"
"Generate support tickets from Jam recordings"

# Product Feedback:

"Analyze this product feedback Jam and create implementation plan"
"Review user experience issues from this recording"
"Extract feature requests from user sessions"

# Development Workflow:

"Use this Jam to understand the bug reproduction steps"
"Analyze the console errors from this session"
"Review network requests to identify API issues"
```

#### **Integration Examples**

**Product Engineer Workflow**:

```markdown
"Review this Jam <Jam Link> and analyze the problem, cross-reference it with the existing codebase, and prepare a detailed plan for implementation."
```

**Product Manager Workflow**:

```markdown
"Analyze these Jams, perform root-cause analysis, and organize them into efficient work packages to minimize engineers' context switching; create Linear tickets from the analysis."
```

**Product Designer Workflow**:

```markdown
"I recorded product feedback in a Jam. Create an implementation plan for the changes requested in this Jam: <Jam Link>"
```

#### **Prerequisites**

- Jam Chrome extension installed
- Existing Jam recordings (anyone can record)
- Internet connection for Jam MCP access
- Jam account for authentication

#### **Security & Privacy**

- **Data Privacy**: Jam opts out of training on customer data
- **Access Control**: MCP mirrors existing Jam permissions
- **Admin Controls**: Use normal admin controls for workspace access
- **No New Access**: MCP doesn't grant additional permissions

#### **Resources**

- [Official Documentation](https://jam.dev/docs/debug-a-jam/mcp)
- [Jam Chrome Extension](https://jam.dev)
- [Setup Guide](https://jam.dev/docs/debug-a-jam/mcp)
- [Video Tutorial](https://jam.dev/docs/debug-a-jam/mcp)

### **Next.js DevTools MCP** - Next.js Development Integration

**Purpose**: Real-time integration with Next.js 16+ development server, providing AI assistants with live access to application runtime, errors, state, and development tools for enhanced debugging and development workflows.

**Key Benefits**:

- Real-time error detection and analysis (build, runtime, and type errors)
- Live application state queries and runtime information access
- Page metadata and component hierarchy inspection
- Server Actions analysis and development logs access
- Next.js documentation and best practices integration
- Automated migration and upgrade assistance
- Browser testing integration with Playwright MCP

**Quick Setup**: Requires Next.js 16+ and running development server

#### **Complete Setup Process**

##### **Step 1: Configuration**

Add to your `mcp.json`:

```json
{
  "mcpServers": {
    "next-devtools": {
      "command": "npx",
      "args": ["-y", "next-devtools-mcp@latest"]
    }
  }
}
```

##### **Step 2: Start Development Server**

1. **Start your Next.js development server**:
   ```bash
   npm run dev
   ```

2. **Verify Next.js DevTools MCP automatically connects** to your running instance

##### **Step 3: Verification**

- **Restart your IDE** after configuration
- **Ensure Next.js dev server is running** (`npm run dev`)
- **Test with Next.js-specific queries** in your AI assistant
- **Verify Next.js DevTools MCP tools are available**

#### **Advanced Capabilities**

- **Error Detection**: Real-time access to build errors, runtime errors, and TypeScript type errors
- **Live State Queries**: Query application state and runtime information in real-time
- **Page Metadata**: Access page routes, components, and rendering details
- **Server Actions Inspection**: Analyze Server Actions and component hierarchies
- **Development Logs**: Access development server logs and console output
- **Next.js Knowledge Base**: Query comprehensive Next.js documentation and best practices
- **Migration Tools**: Automated helpers for upgrading to Next.js 16 with codemods
- **Cache Components Guide**: Setup and configuration assistance for Cache Components
- **Browser Testing**: Playwright MCP integration for verifying pages in the browser

#### **Usage Examples**

```markdown
# Error Detection and Debugging:

"What errors are currently in my application?"
"Analyze the build errors and suggest fixes"
"Check for runtime errors in my Next.js app"
"Review TypeScript type errors and resolve them"

# Application State and Runtime:

"Query the current state of my application"
"Show me the page routes in my Next.js app"
"Inspect the component hierarchy for this page"
"Analyze the Server Actions in my application"

# Development Workflow:

"Review the development logs for issues"
"Check the rendering details for this page"
"Analyze the component structure and suggest optimizations"
"Help me understand the current application state"

# Next.js Best Practices:

"Query Next.js documentation for this feature"
"Show me best practices for Server Actions"
"Help me set up Cache Components"
"Guide me through Next.js 16 migration"

# Browser Testing:

"Test this page in the browser using Playwright"
"Verify the page renders correctly"
"Check for accessibility issues on this route"
```

#### **Prerequisites**

- Next.js 16 or later installed
- Next.js development server running (`npm run dev`)
- Node.js 18+ installed
- MCP-compatible AI coding assistant (Cursor, VS Code, etc.)

#### **Troubleshooting**

If the MCP server is not connecting:

- **Verify Next.js version**: Ensure you're using Next.js v16 or above
- **Check configuration**: Verify `next-devtools-mcp` is configured in your `mcp.json`
- **Start dev server**: Ensure your development server is running (`npm run dev`)
- **Restart services**: Restart both your development server and IDE
- **Check MCP status**: Verify your coding agent has loaded the MCP server configuration

#### **Resources**

- [Official Next.js MCP Documentation](https://nextjs.org/docs/app/guides/mcp)
- [Next.js DevTools MCP GitHub Repository](https://github.com/vercel/next.js/tree/canary/packages/next-devtools-mcp)
- [Next.js 16 Documentation](https://nextjs.org/docs)

---

## 🚀 Quick Start Guide

### 0. **Enable Brain 🧠**

### **1. Prerequisites**

Before setting up MCP servers, ensure you have:

- **Node.js 18+** installed on your system
- **Cursor IDE** or compatible AI assistant (VS Code, Windsurf, Claude Code)
- **Internet connection** for external services
- **Required accounts and API keys** (varies by MCP server)

### **2. Choose Your MCP Servers**

#### **Simple Setup (No API Keys Required)**

- **Context7**: Documentation access - just add configuration
- **Sequential Thinking**: Advanced reasoning - just add configuration
- **Next.js DevTools MCP**: Next.js development integration - just add configuration + running dev server
- **Jam MCP**: Bug analysis - just add configuration + Jam recordings

#### **Advanced Setup (Requires Additional Setup)**

- **Browser Tools**: Chrome extension + two servers + DevTools panel
- **Framelink Figma MCP**: Figma API key + account access
- **Figma Dev Mode MCP**: Figma desktop app + Dev Mode access + Professional plan

### **3. Basic Configuration**

#### **Option A: Use Pre-configured Setup (Recommended)**

The `mcp.json` file in this directory contains pre-configured MCP servers. To use them:

1. **Copy the configuration** to your Cursor settings
2. **Set up environment variables** for services requiring API keys
3. **Follow specific setup steps** for complex servers (Browser Tools, Figma)
4. **Restart Cursor** to activate the MCP servers

#### **Option B: Manual Setup**

For custom configurations:

1. **Add MCP server configurations** to your `mcp.json`
2. **Set up environment variables** for services requiring authentication
3. **Follow server-specific setup requirements**
4. **Test connections** to ensure everything is working

### **4. Environment Configuration**

#### **Required Environment Variables**

```bash
# Figma API Key (for Framelink Figma MCP)
export FIGMA_API_KEY="your_figma_api_key_here"

# Optional: Custom MCP server ports
export MCP_SERVER_PORT="3845"
```

#### **Getting API Keys**

- **Figma API Key**: [Figma Developer Settings](https://www.figma.com/developers/api#authentication)
- **Context7**: No API key required
- **Sequential Thinking**: No API key required
- **Next.js DevTools MCP**: No API key required (but needs Next.js 16+ and running dev server)
- **Jam MCP**: No API key required (but needs Jam recordings)
- **Browser Tools**: No API key required (but needs Chrome extension)
- **Figma Dev Mode MCP**: No API key required (but needs Figma desktop app + Dev Mode access)

### **5. Server-Specific Setup**

#### **Next.js DevTools MCP**

1. Ensure your project uses Next.js 16 or later
2. Add configuration to `mcp.json`
3. Start your Next.js development server: `npm run dev`
4. Verify MCP automatically connects to your running instance

#### **Browser Tools (Complex Setup)**

1. Install Chrome extension from [GitHub repository](https://github.com/AgentDeskAI/browser-tools-mcp)
2. Run `npx @agentdeskai/browser-tools-server@latest` in terminal
3. Enable BrowserToolsMCP panel in Chrome DevTools

#### **Framelink Figma MCP**

1. Get Figma API key from developer settings
2. Set `FIGMA_API_KEY` environment variable
3. Add configuration to `mcp.json`

#### **Figma Dev Mode MCP**

1. Download Figma desktop app
2. Enable MCP server in Figma Preferences
3. Add configuration to `mcp.json`
4. Verify connection with `#get_code` command

#### **Jam MCP**

1. Install Jam Chrome extension from [jam.dev](https://jam.dev)
2. Record a Jam session for testing
3. Add configuration to `mcp.json`
4. Test with Jam link in AI assistant

### **6. Verification**

After setup, verify that MCP servers are working:

1. **Open Cursor** and check the MCP status in the settings
2. **Test each server** by asking your AI assistant to use specific capabilities
3. **Check logs** for any connection issues
4. **Verify API keys** are properly configured

## 🎯 Best Practices

### **MCP Server Management**

- **Start with Core Tools**: Begin with Context7 and Sequential Thinking
- **Add Specialized Tools**: Integrate Browser Tools, Figma, and Jam as needed
- **Monitor Performance**: Keep an eye on server performance and resource usage
- **Update Regularly**: Keep MCP servers updated for latest features

### **Security Considerations**

- **API Key Management**: Store API keys securely using environment variables
- **Access Control**: Limit MCP server access to necessary services only
- **Network Security**: Use secure connections for external API calls
- **Data Privacy**: Be aware of data being sent to external services

### **Performance Optimization**

- **Selective Usage**: Use MCP servers only when needed
- **Caching**: Implement caching for frequently accessed data
- **Resource Monitoring**: Monitor CPU and memory usage
- **Connection Pooling**: Optimize connections to external services

## 🔧 Troubleshooting

### **Common Issues**

#### **MCP Server Connection Issues**

- **Check Node.js version**: Ensure Node.js 18+ is installed
- **Verify network connectivity**: Test internet connection
- **Review server logs**: Check for error messages in server logs
- **Restart services**: Try restarting Cursor and MCP servers

#### **API Key Problems**

- **Verify API keys**: Ensure keys are correctly set in environment variables
- **Check permissions**: Verify API keys have necessary permissions
- **Test connections**: Use curl or similar tools to test API endpoints
- **Review documentation**: Check service-specific setup requirements

#### **Performance Issues**

- **Monitor resources**: Check CPU and memory usage
- **Optimize queries**: Reduce unnecessary API calls
- **Implement caching**: Cache frequently accessed data
- **Update servers**: Ensure MCP servers are up to date

### **Getting Help**

- **Check Documentation**: Review official documentation for each MCP server
- **GitHub Issues**: Report issues on respective GitHub repositories
- **Community Forums**: Join MCP community discussions
- **Video Tutorials**: Watch setup and usage tutorials

## 🤝 Contributing

We welcome contributions to improve MCP configurations and documentation:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/mcp-improvement`
3. **Add your improvements**: Follow the existing format and style
4. **Test your changes**: Ensure MCP servers work correctly
5. **Submit a pull request**: Include clear description of changes

### **Contribution Guidelines**

- Follow the existing documentation format
- Include practical examples where possible
- Test MCP server configurations before submitting
- Provide clear reasoning for new configurations

## 📞 Support & Community

### **Getting Help**

- **Issues**: Report bugs or request features via GitHub Issues
- **Discussions**: Join community discussions for best practices
- **Documentation**: Check the detailed guides for each MCP server
- **Video Tutorials**: Watch setup and usage tutorials

### **Community Guidelines**

- Be respectful and constructive
- Share your experiences and use cases
- Help others learn and improve
- Contribute to the community knowledge base

## 🙏 Acknowledgments

These MCP configurations are based on:

- **Community Contributions**: Input from experienced developers
- **Official Documentation**: Guidelines from MCP protocol maintainers
- **Real-World Experience**: Lessons learned from production usage
- **Modern Development Trends**: Current industry standards and practices

---

## 🎉 Getting Started Checklist

- [ ] Install Node.js 18+ on your system
- [ ] Copy `mcp.json` configuration to your Cursor settings
- [ ] Set up required environment variables
- [ ] Install MCP server dependencies
- [ ] Test each MCP server connection
- [ ] Start using enhanced AI capabilities
- [ ] Explore advanced features and integrations
- [ ] Share configurations with your team

**Remember**: MCP servers are designed to enhance your AI development workflow. Start with core tools and gradually add specialized services as your needs grow. The more you use these tools, the more benefits you'll see in your development productivity and code quality.

---

_Happy coding with enhanced AI capabilities! 🚀_

> **Pro Tip**: Start with Context7 and Sequential Thinking for immediate benefits, then add specialized tools like Browser Tools, Figma integration, and Jam for bug analysis as your workflow requires them. The key is to integrate these tools gradually into your development process.
