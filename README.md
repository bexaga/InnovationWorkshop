# Generate innovative product and service features

# Multi-Agent Workflow for Strategic Marketing Innovation

This GitHub repository documents a structured multi-agent system designed to streamline and elevate strategic marketing innovation. The workflow integrates the expertise of distinct roles—Brand Manager, Creative Director, Market Researcher, and Marketing Assistant—each performing specialized tasks to collaboratively generate, evaluate, and document ideas that align with a target audience's needs.

---
## **Quick Start (for Users)**
- Create an OPENAI API KEY to empower the agents: https://platform.openai.com/
- Create a SERP API KEY to automate Web searches: https://www.searchapi.io/ (100 free requests)
- Add OPENAI AND SERP API Keys as secret to your Colab or Python notebook
- Modify the input to the flow in the last code block:

      #Run the Workshop
      inputs = {
          "brand_name": "iPhone",
          "company": "Apple",
          "target_customer": "AI enthusiasts"
      }
      result = crew.kickoff(inputs=inputs)
- Run the flow

---

## **Agent configuration**

### **1. Brand Manager Agent**
- **Role:** Senior Brand Manager (ex-Procter & Gamble)
- **Goal:** Design and test product/service innovations to meet customer needs, grow sales revenue, and build brand equity.
- **Key Responsibilities:**
  - Write strategic innovation briefs.
  - Ensure innovations are customer-focused, differentiated, and aligned with brand values.
  - Challenge teams to push beyond "deja-vu" ideas.

### **2. Creative Director Agent**
- **Role:** Award-winning Creative Director
- **Goal:** Develop groundbreaking advertising and innovation ideas.
- **Key Responsibilities:**
  - Ideate using deep customer insights.
  - Challenge conventional norms to develop standout ideas.
  - Use techniques like IDEO brainstorming and "What If" methodology.

### **3. Market Researcher Agent**
- **Role:** Experienced Market Researcher
- **Goal:** Research unmet needs, pain points, and delighters of target groups.
- **Key Responsibilities:**
  - Generate deep insights into customer behavior and motivations.
  - Synthesize trends and data to provide actionable insights.
  - Guide the Brand Manager and inspire the Creative Director.

### **4. Marketing Assistant Agent**
- **Role:** Rigorous Marketing Assistant
- **Goal:** Document strategies, rank ideas, and recommend next steps.
- **Key Responsibilities:**
  - Track discussions and summarize marketing strategies.
  - Rank ideas based on strategic fit and uniqueness.
  - Highlight potential misalignments with brand objectives.

---

## **Tasks and Workflow**
### **1. Write Strategic Brief**
- **Agent:** Brand Manager
- **Description:** Frame the marketing objective, recap known strategy, and inspire innovation with success metrics.
- **Output:** One-page strategic brief.

### **2. Research Customer Insights**
- **Agent:** Market Researcher
- **Description:** Explore customer behavior, unmet needs, and trends.
- **Output:** Detailed report of insights.

### **3. Document Strategy**
- **Agent:** Marketing Assistant
- **Description:** Define marketing strategy (WHERE, WHO, WHAT, HOW) and address gaps.
- **Output:** Consolidated marketing strategy.

### **4. Ideate**
- **Agent:** Creative Director
- **Description:** Brainstorm and create diverse ideas to solve identified customer problems.
- **Output:** List of innovative, award-winning ideas.

### **5. Rank Ideas**
- **Agent:** Marketing Assistant
- **Description:** Rank ideas based on fit, insights, and uniqueness.
- **Output:** Prioritized list of ideas with rationale.

---

## **Tools**

- **Search the Web:** The agent is able to search the web and will decide itself what query to search for based on the goal you set.
- **Parse Website** The agent is able to parse website that were most interesting from the web search results.

---

## **How to Run**
1. Clone the repository.
2. Initialize the agents and tasks by defining the following inputs:
   - `brand_name` (e.g., iPhone)
   - `company` (e.g., Apple)
   - `target_customer` (e.g., AI enthusiasts)
3. Execute the multi-agent system using the `kickoff` function:
   ```python
   result = crew.kickoff(inputs={"brand_name": "iPhone", "company": "Apple", "target_customer": "AI enthusiasts"})
   ```

---

## **Example Workflow Outcome**
| **Step** | **Agent**          | **Task**                           | **Output**                                                                                                                                           |
|----------|--------------------|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1        | Brand Manager      | Write Strategic Brief              | Comprehensive memo framing the objective, strategy, and success metrics.                                                                             |
| 2        | Market Researcher  | Research Customer Insights         | Insights on AI enthusiasts' values like personalization, privacy, and ethical tech.                                                                  |
| 3        | Marketing Assistant| Document Strategy                  | Consolidated strategy aligning Apple's values with AI enthusiasts' preferences.                                                                      |
| 4        | Creative Director  | Ideate                             | Six big ideas (e.g., AI Duel, Privacy Challenge) addressing customer needs creatively.                                                               |
| 5        | Marketing Assistant| Rank Ideas                         | Ranked list with AI Duel as top priority based on strategic fit and uniqueness.                                                                      |

## **Content from Browsing**
- Apple Website: Privacy, innovation, and sustainability as key iPhone features.
- Forbes Article: AI enthusiasts demand personalization, data privacy, and ethical technology.
- Case Studies (Coca-Cola, Heinz): AI marketing campaigns showcasing creativity and interactive user engagement.

---

## **Benefits**
- Combines strategic rigor with creative exploration.
- Encourages customer-centric innovation.
- Enables seamless collaboration between agents with distinct expertise.

---

## **Future Enhancements**
- Add real-time feedback loops between agents.
- Incorporate AI-based insights for rapid ideation.
- Enable visualization tools for strategy and idea mapping.

---

Feel free to contribute by improving agent logic, expanding task functionality, or integrating additional tools for data analysis and visualization.
