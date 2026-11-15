# Business Idea Evaluator Agent 🚀

An autonomous multi-agent system built with **LangGraph** and **Groq API** to evaluate business ideas from four critical perspectives: Market Analysis, Legal & Regulatory, Technical Feasibility, and Strategic Roadmap.

## 🧠 Project Architecture & Workflow
The system utilizes a state-graph architecture (`StateGraph`) to orchestrate specialized advisory agents:
1. **Decision & Routing Node (`decide_node`):** Initializes the evaluation state and controls the workflow path.
2. **Parallel Fanout (`fanout`):** Distributes the business idea simultaneously to multiple expert advisors.
3. **Expert Advisors:**
   - 📊 **Market Analyst:** Evaluates target audience, market fit, and demand.
   - ⚖️ **Legal Advisor:** Reviews regulatory compliance and legal requirements.
   - 💻 **Technical Feasibility:** Assesses tech stack, operational needs, and execution.
   - ♟️ **Strategist:** Builds a business roadmap, pricing strategy, and scaling plan.
4. **Aggregation Node (`collect_and_report`):** Synthesizes all advisor reports into a cohesive final evaluation report.

## 🛠️ Tech Stack
- **Python** (Jupyter Notebook)
- **LangGraph** (State management & workflow orchestration)
- **LangChain & Groq API** (`llama-3.3-70b-versatile` LLM integration)
- **IPython** (Graph visualization via Mermaid)

## 🚀 How to Run
1. Clone the repository and open the Jupyter Notebook:
   ```bash
   jupyter notebook business_idea_evaluator.ipynb
