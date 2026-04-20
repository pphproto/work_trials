---

# **Conversion Funnel Analyzer (Web App)**

## **What to Build**

Build an AI-powered web application that analyzes a website (via URL input) and evaluates how effectively it drives users toward conversion.

The tool should extract key elements from the page, construct a conversion funnel, identify drop-offs and friction points, and present the analysis through a clear dashboard with visualizations.

---

## **What the Tool Should Do**

### 1. Accept a Website URL

* Allow users to input a website or landing page URL
* Fetch and process the page content

---

### 2. Extract Page Structure

* Identify:

  * headings and sections
  * primary and secondary CTAs
  * navigation elements
  * key content blocks

* Build an understanding of:

  * page hierarchy
  * content flow

---

### 3. Construct Conversion Funnel

* Infer a funnel such as:

  * landing / awareness
  * exploration
  * consideration
  * conversion

* Map page elements to each stage

---

### 4. Identify Friction & Drop-Off Points

* Analyze the funnel to detect:

  * weak or missing CTAs
  * unclear value proposition
  * excessive cognitive load
  * lack of trust signals
  * dead ends or broken flow

* Highlight where users are most likely to drop off

---

### 5. Provide Structured Insights

* For each funnel stage, output:

  * key elements
  * issues detected
  * impact (low / medium / high)

---

### 6. Visual Dashboard (Important)

* Present results in a clear, visual format such as:

  * funnel diagram showing stages and drop-offs
  * section-wise breakdown
  * issue severity indicators

* Avoid plain text outputs — focus on readability and structure

---

### 7. Summary & Recommendations

* Provide a concise summary of:

  * overall funnel effectiveness
  * top issues impacting conversion
  * actionable improvements

---

## **Tech Stack**

### Required

* **Next.js** (for frontend and API routes)
* **TypeScript**

---

### LLM / AI

* Use any LLM of your choice (we suggest Gemini 3.0 Flash)
* Expected usage:

  * interpreting page structure
  * identifying friction points
  * generating insights and recommendations

---

## **Submission**

* Push code to a GitHub repository

* Include detailed instructions on how to run your code (deployment is optional, not required)

* Include a `NOTES.md` file with:

  * High level design
  * Instructions to run
  * What issues you foresee which need to be taken care of in a productionized version of the tool

* **Record a Loom** walking through the working tool — enter a URL, show the funnel analysis and dashboard, and narrate what's happening

* If you used AI tools (Claude, Cursor, GitHub Copilot, ChatGPT, etc.), export and include your chat history so we can evaluate the prompts used to generate code

**Note:**
We highly recommend using AI copilots (Claude, Cursor, GitHub Copilot, ChatGPT, etc.) to complete this trial efficiently. If you're unable to complete the implementation, you can still submit your work. In your `NOTES.md`, document what you attempted, what worked, what didn't, and why. We evaluate based on effort, problem-solving approach, and the progress you made—not just the final outcome.
