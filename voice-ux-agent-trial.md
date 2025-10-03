# Work Trial: Voice UX Agent

**Duration:** 3-5 days  
**Tech Stack:** Next.js, TypeScript, Puppeteer, LangChain/LangGraph, Gemini Live API

## The Challenge
Build a voice agent that analyzes web pages and conducts UX feedback conversations. Users input a URL, the system captures a screenshot, analyzes it for UX issues, and engages in a voice conversation about the findings.

## What We're Looking For

You'll need to demonstrate:
- Integration with browser automation tools
- Multimodal AI (vision + voice) implementation
- Real-time voice conversation handling
- Creative product thinking for voice UX

## Core Requirements

### Frontend
Build a web interface that allows users to:
- Input any URL for analysis
- View the captured screenshot
- See initial UX analysis results
- Engage in voice conversation with the AI about the page

**What we'll evaluate:**
- Clean, simple UI design
- Real-time voice interaction UX
- Feedback during async operations (screenshot, analysis)
- Error handling for failed URLs

### Backend
Create the system to:
- Accept URL input and validate
- Use Puppeteer to capture full-page screenshots
- Process screenshot through Gemini Vision API
- Orchestrate voice conversation with context from analysis

**What we'll evaluate:**
- Browser automation implementation
- API design for async operations
- How you manage voice streaming
- Error handling (invalid URLs, timeout, etc.)

### AI Integration
Implement an AI system that:
- Analyzes screenshots for UX/UI issues using Gemini Vision
- Generates suggested discussion questions about the page
- Maintains voice conversation with context awareness
- References specific page elements during conversation

**What we'll evaluate:**
- Your approach to vision + voice multimodal AI
- How you structure the conversation flow (use LangGraph)
- Quality of UX analysis
- Voice response latency and naturalness

## Technical Constraints
- Must use TypeScript
- Must use Next.js for frontend/API
- Must use Puppeteer for screenshot capture
- Must use Gemini Live API for voice + Gemini Vision for analysis
- Can use LangChain/LangGraph for orchestration
- You decide on architecture and state management

## Bonus Points
- Deployed working demo
- Support for mobile/desktop viewport options
- Voice conversation history
- Export analysis report
- Multi-language support

## Evaluation Criteria

### Code Quality (40%)
- Clean, readable TypeScript code
- Proper separation of concerns
- Error handling and edge cases
- Type safety

### AI Implementation (30%)
- Effective use of Gemini Vision and Live APIs
- LangGraph conversation flow
- Quality of UX analysis
- Voice interaction responsiveness

### Product Thinking (20%)
- Voice UX design decisions
- Performance (screenshot <10s, voice <3s response)
- User feedback and error messages
- Trade-off decisions documented

### Completeness (10%)
- Core functionality works end-to-end
- Project runs without errors
- Documentation is clear

## Submission

1. Push code to a GitHub repository
2. Deploy to Vercel or similar (or include clear run instructions)
3. Include a `NOTES.md` file with:
   - Key design decisions and trade-offs
   - How you structured the voice conversation flow
   - What you'd improve with more time
   - Any challenges faced
4. Include a 5-minute demo video showing end-to-end flow

## Constraints & Assumptions

- Use Gemini API (we can provide API keys)
- Can use any open-source libraries
- Screenshot capture should work for most standard websites
- Voice conversation can be text-to-speech if Live API is unavailable

## Support
- Feel free to use AI assistants (ChatGPT, Claude, etc.) as you would in daily work
- Google/Stack Overflow is encouraged
- If you get blocked >30min on something, document it and move on
