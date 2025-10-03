# Work Trial: User Persona Builder

**Duration:** 3-5 days  
**Tech Stack:** Next.js, TypeScript, Node.js, LangChain/LangGraph

## The Challenge
Build an AI-powered tool that analyzes product/service information and generates comprehensive user personas. Users can input text descriptions, upload images, or provide a URL, and the system will create a product profile, ideal customer profile (ICP), and detailed user personas.

## What We're Looking For

You'll need to demonstrate:
- Full-stack development: UI, API design, and backend logic
- Multimodal AI integration: Processing text, images, and web content
- Structured data generation with LangGraph
- Product thinking: UX decisions, error handling, performance trade-offs

## Core Requirements

### Frontend
Build a web interface that allows users to:
- Input product/service information via multiple methods:
  - Text description (paste or type)
  - Image upload (product screenshots, marketing materials, etc.)
  - URL input (website, landing page, etc.)
- View generated outputs in an organized, readable format
- Export or save personas
- See appropriate feedback during processing

**What we'll evaluate:**
- Component structure and reusability
- Type safety and state management
- User experience and error handling
- How you present complex structured output
- Responsive design considerations

### Backend
Create API endpoints to handle:
- Text, image, and URL inputs with validation
- Processing different input types
- Orchestrating multi-step AI analysis
- Generating structured persona data

**What we'll evaluate:**
- API design and data modeling
- How you structure and validate requests/responses
- Error handling and edge cases
- Choice of storage/persistence strategy
- Handling of async operations

### AI Integration
Implement an LLM-powered system that:
- Extracts and analyzes product information from multiple input types
- Generates a comprehensive product profile
- Creates an ideal customer profile (ICP)
- Produces 3-5 detailed user personas with:
  - Demographics
  - Goals and motivations
  - Pain points
  - Behaviors and preferences
  - Use cases

**What we'll evaluate:**
- Your approach to multimodal content analysis
- How you structure the LangGraph workflow (should have multiple nodes for profile building, ICP generation, persona creation)
- Prompt design and output quality
- Structure and completeness of generated personas
- How you balance depth vs breadth in persona generation

## Technical Constraints
- Must use TypeScript
- Must use Next.js for frontend/API
- Must use LangChain/LangGraph for AI orchestration
- Can use any LLM provider (we can provide API keys if needed)
- You decide on output format, storage strategy, and architecture

## Bonus Points
- Deployed working demo
- Multiple persona templates or styles
- Comparison view for multiple personas
- Edit/refine generated personas
- Export to different formats (PDF, JSON, etc.)
- Tests

## Evaluation Criteria

### Code Quality (40%)
- Clean, readable TypeScript code
- Proper separation of concerns
- Error handling and edge cases
- Type safety

### AI Implementation (30%)
- Correct use of LangChain/LangGraph concepts
- Effective multimodal content analysis
- Quality and realism of generated personas
- Structured workflow for persona generation
- Prompt engineering quality

### Product Thinking (20%)
- UX considerations and polish
- Performance (reasonable load times)
- Error messages and user feedback
- Output presentation and usability
- Trade-off decisions documented

### Completeness (10%)
- All input types work (text, image, URL)
- Generated output is comprehensive
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
4. Include at least one example for each input type (text, image, URL)

## Constraints & Assumptions

- Use OpenAI/Gemini/Anthropic API
- Can use any open-source libraries
- In-memory storage is acceptable (no need for real DB)
- Define your own persona structure and fields
- URL scraping can be basic (focus on main content)

## Support
- Feel free to use AI assistants (ChatGPT, Claude, etc.) as you would in daily work
- Google/Stack Overflow is encouraged
- If you get blocked >30min on something, document it and move on