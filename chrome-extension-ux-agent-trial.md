# Work Trial: Chrome Extension UX Agent

**Duration:** 3-5 days  
**Tech Stack:** TypeScript, Chrome Extension Manifest V3, LangChain/LangGraph, Gemini AI

## The Challenge
Build a Chrome extension with an AI agent that analyzes the current webpage to identify UX issues and provide actionable improvement recommendations. Users click the extension icon to trigger analysis and view results in-browser.

## What We're Looking For

You'll need to demonstrate:
- Chrome extension development skills
- Working with multimodal LLMs (vision)
- Structured AI output and reasoning
- Product sense for developer tools

## Core Requirements

### Extension UI
Build a Chrome extension with:
- Popup UI to trigger analysis and display results
- One-click analysis of the current webpage
- In-browser display of findings
- Loading states and error handling

**What we'll evaluate:**
- Extension UX and interaction design
- How you display analysis results
- Handling of different page types
- Visual design and clarity

### Extension Architecture
Create the extension with:
- Content script to analyze DOM and extract page information
- Background service worker to orchestrate AI analysis
- Chrome APIs for DOM access and screenshot capture
- Proper messaging between components

**What we'll evaluate:**
- Chrome extension architecture (Manifest V3)
- Proper use of content scripts, service workers, messaging
- How you handle async operations
- Error handling and edge cases

### AI Integration
Implement an AI system that:
- Analyzes the current webpage structure and content
- Uses screenshot analysis for visual issues
- Identifies UX problems (accessibility, navigation, layout, etc.)
- Provides specific, actionable recommendations

**What we'll evaluate:**
- Your approach to multimodal analysis (DOM + screenshot)
- How you structure the LangGraph workflow
- Quality and relevance of identified issues
- Actionability of suggestions

## Technical Constraints
- Must use TypeScript
- Must use Chrome Extension Manifest V3
- Must use LangChain/LangGraph for AI orchestration
- Must use Gemini AI for analysis
- You decide on analysis categories, output format, and architecture

## Bonus Points
- Visual highlighting of problematic elements on the page
- Categorizing feedback by type (accessibility, layout, etc.)
- Severity scoring for issues
- Export findings as report
- Tests

## Evaluation Criteria

### Code Quality (40%)
- Clean, readable TypeScript code
- Proper separation of concerns
- Type safety

### AI Implementation (30%)
- Langchain/LangGraph workflow design
- Prompt engineering for vision models
- Structure and quality of analysis
- Handling of different UI types

### Product Thinking (20%)
- Extension UX design
- Presentation of findings
- Feature choices and prioritization
- Trade-off decisions documented

### Completeness (10%)
- Core functionality works end-to-end
- Extension loads and runs without errors
- Documentation is clear

## Submission

1. Push code to a GitHub repository
2. Include clear instructions on how to load the extension locally
3. Include a `NOTES.md` file with:
   - Key design decisions and trade-offs
   - How your LangGraph workflow is structured
   - What you'd improve with more time
   - Any challenges faced
4. Include 2-3 example screenshots or URLs to test with

## Constraints & Assumptions

- Gemini API (recommended)
- Can use any open-source libraries
- Focus on web UI analysis
- Define your own set of UX issue categories

## Support
- Feel free to use AI assistants (ChatGPT, Claude, etc.) as you would in daily work
