# Cursor Rules - Professional Software Development Guidelines

> **Enterprise-Level Coding Standards & Best Practices for Modern Software Development**

This repository contains comprehensive cursor rules and development guidelines designed to elevate your coding standards and ensure consistent, maintainable, and scalable software development practices across your projects.

## 🎯 What Are Cursor Rules?

Cursor rules are AI-powered development guidelines that help you write better code by providing context-aware suggestions, enforcing best practices, and maintaining consistency across your codebase. These rules are designed to work with AI coding assistants like Cursor, GitHub Copilot, and similar tools.

## 📚 What's Included

### 🏗️ **Core Development Guidelines**

- **Technology-Agnostic Principles**: Universal coding standards that apply to any tech stack
- **Enterprise-Level Best Practices**: Battle-tested patterns from large-scale applications
- **Professional Development Workflows**: Proven methodologies for team collaboration

### 🔧 **Technology-Specific Rules**

#### Backend Development

- **NestJS & TypeScript**: Complete framework-specific conventions and patterns
- **Database & ORM**: Best practices for data modeling and database operations
- **API Documentation**: Swagger/OpenAPI standards and documentation practices
- **Error Handling**: Comprehensive error management strategies
- **Microservices**: Architecture patterns and messaging protocols

#### Frontend Development

- **Next.js & React**: Modern React patterns and Next.js conventions
- **TypeScript**: Type safety and interface design best practices
- **Component Architecture**: Reusable component patterns and state management
- **Server Actions**: Next.js server action patterns
- **UI/UX Standards**: Shadcn/UI and Tailwind CSS best practices

## 🚀 Quick Start Guide

### 0. **Enable Brain 🧠**

### 1. **Understanding Cursor Rules Structure**

Cursor rules can be organized in different ways depending on your project needs:

#### **Option 1: Single File Approach**

Create a `.cursorrules` file in your project root:

```
your-project/
├── .cursorrules                    # All rules in one file
├── src/
└── README.md
```

#### **Option 2: Organized Folder Structure (Recommended)**

Create a `.cursor/rules/` directory for better organization:

```
your-project/
├── .cursor/
│   └── rules/
│       ├── global.mdc              # Global development rules
│       ├── backend.mdc             # Backend-specific rules
│       ├── frontend.mdc            # Frontend-specific rules
│       └── ui.mdc                  # UI/Styling rules
├── src/
└── README.md
```

### 2. **Setup Cursor Rules in Your Project**

#### Option A (recommended): Reference Rules Directly from Repository

**How to use raw repository links:**

Simply put the raw GitHub URLs inside your `.cursorrules` file or `.cursor/rules/` files. Cursor will automatically fetch and apply these rules when needed.

**Example - In your `.cursorrules` file:**

```
# Your custom rules here...

# Reference external rules
@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/.cursorrules
@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/backend/nestjs-typescript-cursorrules-prompt-file/nestjs-conventions.mdc
@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/frontend/nextjs-react-typescript-cursorrules-prompt-file/next-js-conventions.mdc
```

**Example Rules (Full list available in repository):**

- [Main Cursor Rules](https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/.cursorrules) - Core development principles and technology-agnostic guidelines
- [Next.js Conventions](https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/frontend/nextjs-react-typescript-cursorrules-prompt-file/next-js-conventions.mdc) - Next.js framework-specific patterns and conventions
- [UI/Styling Rules](https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/frontend/shadcn-and-tailwind/ui-and-styling-with-shadcn-ui-and-tailwind.mdc) - UI/UX standards and styling best practices

**💡 Pro Tip**: You can reference ANY file from the repository using the same pattern:
`@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/[file-path]`

Browse the full repository at: [sinova-dev/cursor-rules](https://github.com/sinova-dev/cursor-rules) to see all available rules and copy the paths you need.

#### Alternative CLI approach:

**💡 What these commands do:**

These commands create files and put URL references to rules in the repository. Each file will contain the actual rule content that Cursor can read and apply to your project directly from the GitHub repo.

**Commands to run:**

```bash
# Creates .cursorrules file with URL @import reference to main rules
echo "@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/.cursorrules" > .cursorrules

# Creates .cursor/rules directory for organized rule files
mkdir -p .cursor/rules

# Creates backend.mdc file with URL @import reference to NestJS rules
echo "@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/backend/nestjs-typescript-cursorrules-prompt-file/nestjs-conventions.mdc" > .cursor/rules/backend.mdc

# Creates frontend.mdc file with URL @import reference to Next.js rules
echo "@import https://raw.githubusercontent.com/sinova-dev/cursor-rules/master/frontend/nextjs-react-typescript-cursorrules-prompt-file/next-js-conventions.mdc" > .cursor/rules/frontend.mdc

```

#### Option B: Copy the Rules File

```bash
# First, clone or download the repository
git clone https://github.com/sinova-dev/cursor-rules.git
cd cursor-rules

# Then copy the .cursorrules file to your project root
cp .cursorrules /path/to/your/project/

**💡 Pro Tips:**
- **Backend rules**: `backend/nestjs-typescript-cursorrules-prompt-file/*.mdc` - Includes NestJS conventions, database patterns, error handling, API docs, and microservices
- **Frontend rules**: `frontend/nextjs-react-typescript-cursorrules-prompt-file/*.mdc` - Includes Next.js patterns, React components, server actions, and frontend error handling
- **UI rules**: `frontend/shadcn-and-tailwind/*.mdc` - Includes UI/UX standards, Shadcn/UI patterns, and Tailwind CSS best practices
```

### 3. **Configure Your Development Environment**

#### For Cursor IDE:

1. Place `.cursorrules` in your project root
2. Restart Cursor or reload the workspace
3. The rules will automatically apply to your AI interactions

#### For VS Code with GitHub Copilot:

1. Create a `.github/copilot/` directory in your project
2. Add rule files as `.md` or `.txt` files
3. Reference these in your Copilot settings

#### For Other AI Assistants:

- Copy relevant sections to your project documentation
- Use as prompts in your AI interactions
- Integrate into your team's development guidelines

## 📖 How to Use These Rules

### **For Individual Developers**

1. **Start with Core Principles**: Begin with the technology-agnostic guidelines in `.cursorrules`
2. **Add Technology-Specific Rules**: Include relevant backend/frontend rules based on your stack
3. **Customize for Your Project**: Adapt rules to match your team's preferences and project requirements
4. **Use as AI Prompts**: Reference these rules when asking AI assistants for code suggestions

### **For Teams**

1. **Establish Standards**: Use these rules as a foundation for your team's coding standards
2. **Code Reviews**: Reference rules during pull request reviews
3. **Onboarding**: Use as training material for new team members
4. **Documentation**: Integrate into your project documentation

### **For Project Managers**

1. **Quality Assurance**: Use rules to establish quality gates
2. **Team Alignment**: Ensure consistent development practices across teams
3. **Performance Metrics**: Track adherence to these standards
4. **Continuous Improvement**: Regularly review and update rules based on team feedback

## 🎯 Key Benefits

### **Code Quality**

- ✅ Consistent coding patterns across your codebase
- ✅ Reduced technical debt and maintenance overhead
- ✅ Improved code readability and maintainability
- ✅ Better error handling and edge case management

### **Team Productivity**

- ✅ Faster onboarding for new team members
- ✅ Reduced code review time and conflicts
- ✅ Consistent development workflows
- ✅ Better collaboration and knowledge sharing

### **Project Scalability**

- ✅ Architecture patterns that scale with your project
- ✅ Maintainable codebase as your team grows
- ✅ Reduced debugging time and production issues
- ✅ Better performance and security practices

## 📋 Rule Categories Explained

### **Core Development Principles**

- **SOLID Principles**: Object-oriented design fundamentals
- **DRY (Don't Repeat Yourself)**: Code reusability and maintainability
- **Functional Programming**: Modern programming paradigms
- **Separation of Concerns**: Clean architecture patterns

### **Code Organization**

- **Feature-Based Structure**: Scalable project organization
- **Module Boundaries**: Clear component separation
- **Import Organization**: Logical dependency management
- **File Naming**: Consistent naming conventions

### **Error Handling**

- **Early Returns**: Clean error flow management
- **Guard Clauses**: Precondition validation
- **Structured Logging**: Better debugging and monitoring
- **User-Friendly Messages**: Better user experience

### **Security & Performance**

- **Input Validation**: Security-first development
- **Authentication/Authorization**: Proper access control
- **Caching Strategies**: Performance optimization
- **Monitoring**: Production-ready observability

## 🔧 Customization Guide

### **Adapting Rules for Your Project**

1. **Technology Stack**: Modify rules to match your specific technologies
2. **Team Preferences**: Adjust conventions to match your team's style
3. **Project Requirements**: Add project-specific guidelines
4. **Industry Standards**: Incorporate industry-specific best practices

### **Creating Custom Rules**

```markdown
# Your Custom Rules

## Project-Specific Guidelines

- Follow your company's naming conventions
- Use your preferred state management patterns
- Implement your authentication strategy
- Follow your deployment and CI/CD practices

## Team Conventions

- Code review checklist items
- Testing requirements
- Documentation standards
- Performance benchmarks
```

## 📚 Learning Resources

### **Cursor Rules Documentation & Collections**

- [Cursor Rules Official Documentation](https://docs.cursor.com/context/rules) - Complete guide to creating and using cursor rules
- [Awesome Cursor Rules](https://github.com/PatrickJS/awesome-cursorrules) - Curated collection of cursor rules for various technologies and frameworks
- [PromptHub Cursor Rules Collection](https://app.prompthub.us/prompthub/collection/cursor-rules) - Community-contributed cursor rules and templates

## 🤝 Contributing

We welcome contributions to improve these guidelines:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/new-rule`
3. **Add your improvements**: Follow the existing format and style
4. **Test your changes**: Ensure rules work with AI assistants
5. **Submit a pull request**: Include clear description of changes

### **Contribution Guidelines**

- Follow the existing documentation format
- Include practical examples where possible
- Test rules with AI assistants before submitting
- Provide clear reasoning for new guidelines

## 📞 Support & Community

### **Getting Help**

- **Issues**: Report bugs or request features via GitHub Issues
- **Discussions**: Join community discussions for best practices
- **Documentation**: Check the detailed guides in each subdirectory

### **Community Guidelines**

- Be respectful and constructive
- Share your experiences and use cases
- Help others learn and improve
- Contribute to the community knowledge base

## 🙏 Acknowledgments

These guidelines are based on:

- **Industry Best Practices**: Proven patterns from successful projects
- **Community Contributions**: Input from experienced developers
- **Real-World Experience**: Lessons learned from production applications
- **Modern Development Trends**: Current industry standards and practices

---

## 🎉 Getting Started Checklist

- [ ] Copy `.cursorrules` to your project root
- [ ] Review and customize rules for your tech stack
- [ ] Set up your development environment
- [ ] Share rules with your team
- [ ] Integrate into your development workflow
- [ ] Start using AI assistants with these guidelines
- [ ] Monitor and improve based on team feedback

**Remember**: These rules are designed to evolve with your project. Regularly review and update them based on your team's experience and changing requirements.

---

_Happy coding! 🚀_

> **Pro Tip**: Start with the core principles and gradually add technology-specific rules as your project grows. Consistency is key - the more you follow these guidelines, the more benefits you'll see in your codebase quality and team productivity.
