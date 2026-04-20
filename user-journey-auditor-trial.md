---

# **User Journey Auditor (Browser Extension)**

## **What to Build**

Build an AI-powered Chrome extension that analyzes a live website and evaluates how easily users can navigate key journeys (e.g. signup, pricing, core actions).

The tool should extract interaction data directly from the DOM, identify common user journeys, and highlight friction points in those journeys.

---

## **What the Tool Should Do**

### 1. Accept a Live Website Context

* Run on any active webpage via a Chrome extension
* Access and process the DOM of the current page

---

### 2. Extract Interactive Elements

* Identify:

  * links, buttons, CTAs
  * navigation menus
  * forms and inputs
* Build a basic representation of possible user actions

---

### 3. Generate User Journeys

* Identify common journeys such as:

  * exploring the product
  * finding pricing
  * signing up or getting started

* For each journey, provide:

  * step-by-step flow
  * number of clicks / steps
  * entry and exit points

---

### 4. Perform Journey-Based UX Audit

* Analyze each journey for usability issues such as:

  * excessive steps or click depth
  * unclear or missing CTAs
  * dead ends or broken flows
  * poor visibility of key actions

---

### 5. Provide Structured Output

* Display results in a clear, organized format
* Each journey should include:

  * steps
  * key actions
  * identified issues

---

### 6. Show Intermediate Results (Important)

* Surface at least one of:

  * extracted elements
  * navigation structure
  * detected journeys

---

### 7. (Bonus) Question-Based Interaction

* Allow users to ask questions such as:

  * “How easy is it to sign up?”
  * “What’s the shortest path to pricing?”
  * “Where might users drop off?”

---

## **Tech Stack**

### Required

* **Next.js** (for UI layer — popup or web interface)
* **Chrome Extension APIs** (content scripts, messaging, etc.)
* **TypeScript**

---

### LLM / AI

* Use any LLM of your choice (we suggest Gemini 3.0 Flash)
* Expected usage:

  * interpreting journeys
  * identifying friction points
  * (bonus) answering user queries
* Avoid relying solely on LLMs for raw data extraction

---

## **Submission**

* Push code to a GitHub repository

* Include detailed instructions on how to run your code (deployment is optional, not required)

* Include a `NOTES.md` file with:

  * High level design
  * Instructions to run
  * What issues you foresee which need to be taken care of in a productionized version of the tool

* **Record a Loom** walking through the working extension — show the popup, trigger a journey audit on a live page, and narrate what's happening

* If you used AI tools (Claude, Cursor, GitHub Copilot, ChatGPT, etc.), export and include your chat history so we can evaluate the prompts used to generate code

**Note:**
We highly recommend using AI copilots (Claude, Cursor, GitHub Copilot, ChatGPT, etc.) to complete this trial efficiently. If you're unable to complete the implementation, you can still submit your work. In your `NOTES.md`, document what you attempted, what worked, what didn't, and why. We evaluate based on effort, problem-solving approach, and the progress you made—not just the final outcome.
