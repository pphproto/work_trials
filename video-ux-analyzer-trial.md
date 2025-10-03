# Work Trial: Video UX Analyzer

**Duration:** 3-5 days  
**Tech Stack:** Next.js, TypeScript, Node.js, LangChain/LangGraph

## The Challenge
Build an AI-powered tool that analyzes product demo videos and identifies UX issues. Users upload a product demo video, and the system analyzes it frame-by-frame to detect usability problems, interaction issues, and areas for improvement.

## What We're Looking For

You'll need to demonstrate:
- Full-stack development: UI, API design, and backend logic
- Video processing and analysis with LLMs
- Structured analysis output with LangGraph
- Product thinking for video analysis tools

## Core Requirements

### Frontend
Build a web interface that allows users to:
- Upload product demo videos (your choice of supported formats)
- View video playback
- See AI-generated UX analysis with timestamps
- Navigate to specific issues in the video
- See appropriate feedback during processing

**What we'll evaluate:**
- Component structure and reusability
- Type safety and state management
- User experience and error handling
- How you present video analysis results
- Video player integration and timeline navigation
- Responsive design considerations

### Backend
Create API endpoints to handle:
- Video uploads and validation
- AI analysis orchestration
- Returning structured findings with timestamps

**What we'll evaluate:**
- API design and data modeling
- How you handle video file uploads
- Error handling and edge cases
- Choice of storage/persistence strategy
- Handling of async/long-running operations

### AI Integration
Implement an LLM-powered system that:
- Processes video content using vision-capable LLMs
- Identifies UX issues in product demos:
  - Navigation problems
  - Confusing UI elements
  - Poor user flows
  - Accessibility issues
  - Interaction delays or friction
  - Unclear labels or messaging
- Provides timestamp references for each issue
- Generates actionable recommendations

**What we'll evaluate:**
- Your approach to video analysis with LLMs
- How you structure the LangGraph workflow
- Prompt design for video analysis
- Quality and relevance of identified issues
- Timestamp accuracy
- Actionability of recommendations

## Technical Constraints
- Must use TypeScript
- Must use Next.js for frontend/API
- Must use LangChain/LangGraph for AI orchestration
- Must use an LLM provider with video analysis capabilities (we can provide API keys)
- You decide on architecture and output structure

## Bonus Points
- Deployed working demo
- Support for multiple video formats
- Video timeline with issue markers
- Severity scoring for issues
- Export analysis report
- Side-by-side video and analysis view
- Tests

## Evaluation Criteria

### Code Quality (40%)
- Clean, readable TypeScript code
- Proper separation of concerns
- Error handling and edge cases
- Type safety

### AI Implementation (30%)
- Effective video/frame analysis approach
- LangGraph workflow design
- Prompt engineering for visual analysis
- Quality and relevance of UX issues detected
- Timestamp accuracy

### Product Thinking (20%)
- UX of the analysis tool itself
- Performance (handling large videos)
- Presentation of findings
- Error messages and user feedback
- Trade-off decisions documented

### Completeness (10%)
- Video upload and processing works
- Analysis generates meaningful output
- Project runs without errors
- Documentation is clear

## Submission

1. Push code to a GitHub repository
2. Deploy to Vercel (or include clear run instructions)
3. Include a `NOTES.md` file with:
   - Key design decisions and trade-offs
   - How your LangGraph workflow is structured
   - What you'd improve with more time
   - Any challenges faced
4. Include 1-2 sample demo videos to test with (or links to them)

## Constraints & Assumptions

- Use OpenAI/Gemini/Anthropic API (video-capable models)
- Can use any open-source libraries
- Focus on short demo videos (1-5 minutes)
- In-memory storage is acceptable (no need for real DB)
- Define your own UX issue categories

## Support
- Feel free to use AI assistants (ChatGPT, Claude, etc.) as you would in daily work
- Google/Stack Overflow is encouraged
- If you get blocked >30min on something, document it and move on