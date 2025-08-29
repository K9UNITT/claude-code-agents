# Contributing to Claude Code Agents

We welcome contributions to make this the most comprehensive collection of Claude Code agents for developers! 

## 🤝 How to Contribute

### Adding New Agents

1. **Choose a Category**: Place your agent in the appropriate category folder
2. **Follow the Template**: Use the established agent format with YAML frontmatter
3. **Be Specific**: Include detailed examples and clear trigger scenarios
4. **Test Thoroughly**: Ensure your agent works as expected in Claude Code

### Agent Template

```markdown
---
name: your-agent-name
description: Detailed description of when to use this agent, with specific trigger scenarios and delegation examples
model: sonnet|haiku
---

You are a [ROLE] specialist who helps developers with [SPECIFIC TASK].

## Core Capabilities:
- List specific, actionable capabilities
- Focus on concrete deliverables
- Explain expert knowledge areas

## Specific Scenarios:
- When user asks "specific example request"
- When user mentions specific keywords or contexts
- When certain conditions or problems arise
- When working with specific technologies or patterns

## Expected Outputs:
- Specific deliverables and formats
- Quality standards and requirements
- Documentation and examples included
- Performance or measurement criteria

## Will NOT Handle:
- Tasks better suited for other agents (with defer recommendations)
- Out of scope activities with clear boundaries

When working: Provide specific behavioral instructions, output format requirements, and quality standards.
```

### Agent Quality Standards

#### ✅ Good Agents Have:
- **Specific Trigger Scenarios**: Clear examples of when Claude Code should use this agent
- **Concrete Examples**: Real situations with user quotes and assistant responses
- **Clear Boundaries**: What the agent WILL and WON'T handle
- **Expected Outputs**: Specific deliverables and quality standards
- **Proper Model Selection**: Sonnet for analysis/technical, Haiku for writing/communication

#### ❌ Avoid:
- Generic descriptions without specific use cases
- Vague capabilities like "helps with development"
- Missing examples or delegation scenarios
- Overlapping functionality with existing agents
- Incorrect model selection for the task complexity

### Model Selection Guidelines

**Use Sonnet for:**
- Complex analysis and reasoning tasks
- Technical architecture and system design
- Code review and security analysis
- Strategic planning and prioritization
- Research and competitive analysis

**Use Haiku for:**
- Content creation and writing tasks
- Marketing copy and communications
- Documentation and technical writing
- Simple formatting and template tasks

## 📂 Repository Structure

```
claude-agents/
├── category-name/
│   ├── agent-name.md
│   └── another-agent.md
├── README.md
├── install.sh
└── CONTRIBUTING.md
```

## 🔧 Development Process

### 1. Fork and Clone
```bash
git fork https://github.com/username/claude-agents
git clone https://github.com/your-username/claude-agents
cd claude-agents
```

### 2. Create Agent
- Add your agent file to the appropriate category folder
- Follow the template format exactly
- Include comprehensive examples

### 3. Test Your Agent
```bash
# Install your agents locally
./install.sh

# Test in Claude Code
# Restart Claude Code and test your agent with various scenarios
```

### 4. Submit Pull Request
- Create a descriptive PR title
- Explain what your agent does and why it's needed
- Include examples of the agent in action
- Reference any related issues

## 📝 Agent Categories

### Existing Categories:
- **architecture** - System design and planning
- **code-quality** - Code review, testing, security
- **design** - UI/UX, branding, visual design
- **marketing** - Copy, content, advertising
- **product** - Product management, UX, feedback
- **business** - Legal, strategy, planning
- **devops** - Infrastructure, deployment, monitoring
- **data** - Analytics, SQL, reporting
- **communication** - Documentation, support, presentations  
- **research** - Technology research and analysis

### Suggesting New Categories:
- Create an issue explaining the need for a new category
- Provide examples of 3-5 agents that would fit
- Explain how it's different from existing categories

## 🐛 Bug Reports

When reporting issues with agents:

1. **Agent Name**: Which specific agent has the problem
2. **Expected Behavior**: What you expected the agent to do  
3. **Actual Behavior**: What actually happened
4. **Context**: The request you made to Claude Code
5. **Reproduction Steps**: How to reproduce the issue

## 💡 Feature Requests

For new agent ideas:

1. **Use Case**: What problem would this agent solve
2. **Target Audience**: Who would benefit from this agent
3. **Examples**: Specific scenarios where it would be used
4. **Differentiation**: How it's different from existing agents

## ✅ Code Review Process

All contributions go through review:

1. **Technical Review**: Ensure proper YAML format and agent structure
2. **Quality Review**: Verify examples, scenarios, and capabilities are clear
3. **Testing Review**: Confirm the agent works as described
4. **Documentation Review**: Ensure README updates if needed

## 📖 Style Guide

### Agent Naming
- Use kebab-case: `user-story-writer`, not `UserStoryWriter`
- Be specific: `landing-page-writer`, not `writer`
- Avoid redundant words: `sql-expert`, not `sql-database-expert`

### Description Writing
- Start with "Use this agent when you need to..."
- Include specific trigger scenarios  
- Reference concrete examples with user quotes
- End with model specification

### Examples Format
```markdown
<example>
Context: Brief situation description
user: "Exact quote of what user might say"
assistant: "Response showing how agent helps"
<commentary>
Explanation of why this agent should be used in this scenario
</commentary>
</example>
```

## 🚀 Release Process

1. **PR Approval**: Maintainer approves your contribution
2. **Merge**: Changes merged to main branch  
3. **Testing**: Automated tests run on all agents
4. **Release**: New version tagged and released
5. **Documentation**: README updated with new agents

## 📞 Getting Help

- **Questions**: Open a GitHub issue with the "question" label
- **Discussions**: Use GitHub Discussions for broader topics
- **Chat**: Join our community discussions

## 🎯 Roadmap

Current priorities:
- [ ] Complete all 59 planned agents
- [ ] Add automated testing for agent format validation
- [ ] Create video tutorials for common agent workflows
- [ ] Build web interface for browsing agents
- [ ] Add performance metrics and usage analytics

---

**Thank you for contributing to the Claude Code agents community!** 🙏