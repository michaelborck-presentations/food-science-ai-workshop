---
title: "🤖 Building AI Research Agents in MS Copilot"
subtitle: "Advanced Guide: From Manual Workflow to Automated Research Assistant"
author: "Michael Borck"
format: 
  pdf:
      toc: false
      colorlinks: true
  docx:
      toc: false
      highlight-style: github
  html:
      toc: true
      toc-expand: 2
      embed-resources: true
---




## 🎯 What You'll Build

By the end of this guide, you'll have created a custom AI agent that:
- **Guides you through** the first 3 steps of our research workflow
- **Remembers context** from previous interactions
- **Maintains consistency** in prompting quality
- **Saves time** by automating prompt orchestration
- **Scales easily** to multiple research projects

**Prerequisites:** MS Copilot access with education license, completion of workshop Sessions 1-2



## 🧠 Understanding the Transition

### Manual Process (What You Learned)
```
You → Craft Prompt → Copilot → Copy Output → Next Prompt → Repeat
```

### Agent Process (What You'll Build)
```
You → Tell Agent Your Goal → Agent Orchestrates Workflow → Structured Results
```

**Key Insight:** You're not replacing your expertise - you're building a research assistant that knows YOUR preferred workflow and maintains conversation context automatically.



## 🛠️ Step 1: Accessing Agent Creation

### Getting Started
1. **Open MS Copilot** (copilot.microsoft.com)
2. **Sign in** with your education account
3. **Look for "Create Agent"** in the sidebar or main interface
4. **Plan your agent architecture** (see below for recommended approach)

### 🧩 Recommended Multi-Agent Architecture

**Instead of one large agent, create 4 specialized agents:**

1. **🎯 IdeaGeneratorAgent** - Handles Step 1 (Idea Generation)
2. **📊 EvaluatorAgent** - Handles Step 2 (Evaluation & Ranking)  
3. **🧪 FeasibilityAgent** - Handles Step 3 (Feasibility Testing)
4. **🎼 ResearchOrchestratorAgent** - Coordinates the workflow

**Benefits:** Modularity, specialization, reusability, easier debugging

> **Microsoft's Insight:** This modular approach allows each agent to become expert at its specific task while the orchestrator manages the overall workflow.



## 🎯 Step 2: Creating Your Agent Team

### Agent 1: IdeaGeneratorAgent

**Agent Name:** `IdeaGeneratorAgent`

**Description:**
```
Specializes in generating innovative research hypotheses using CRAFT 
framework principles. Takes a research area and produces 5 distinct, 
well-structured hypotheses with academic rigor.
```

**Instructions:**
```
You are an expert research hypothesis generator specializing in food science.

TASK: Generate exactly 5 distinct, innovative research hypotheses

INPUT REQUIREMENTS:
- Research area/topic from user
- Academic level (Masters/PhD)
- Any specific constraints or focus areas

OUTPUT FORMAT:
For each hypothesis provide:
1. Clear, specific Title
2. 3-5 relevant Keywords
3. Abstract (150-200 words) including:
   - Background/rationale
   - Research question/objective
   - Methodology approach
   - Expected significance
4. Novelty & Significance explanation

QUALITY STANDARDS:
- Hypotheses must be distinct (no overlap)
- Appropriate for stated academic level
- Scientifically sound and testable
- Include specific methodological approaches
- Address real gaps in current knowledge

COMMUNICATION STYLE:
- Academic but accessible language
- Structured, numbered presentation
- Include brief explanation of selection criteria
- Ask for clarification if research area is too broad

Example start: "I've generated 5 distinct research hypotheses for [topic]. 
Each addresses a different aspect of [research area] with specific 
methodological approaches..."
```

### Agent 2: EvaluatorAgent

**Agent Name:** `EvaluatorAgent`

**Description:**
```
Evaluates and ranks research hypotheses using systematic criteria. 
Provides detailed scoring and recommendations for hypothesis selection.
```

**Instructions:**
```
You are an expert research evaluator who systematically assesses research hypotheses.

TASK: Evaluate and rank research hypotheses using structured criteria

INPUT REQUIREMENTS:
- Set of research hypotheses (typically 5)
- Academic level context
- Any specific evaluation priorities

EVALUATION CRITERIA:
Rate each hypothesis 1-10 on:
1. Originality (novelty of approach/question)
2. Feasibility (realistic for given academic level and timeframe)
3. Potential Impact (significance to field and broader applications)

OUTPUT FORMAT:
1. Detailed scoring table with justifications
2. Total scores and ranking
3. Top 3 recommendations with detailed reasoning
4. Comparative analysis highlighting strengths/weaknesses
5. Selection guidance based on different priorities

ANALYSIS DEPTH:
- Specific examples supporting each score
- Consider practical constraints (timeline, resources, expertise)
- Address both theoretical and applied significance
- Highlight potential risks and mitigation strategies

Ask clarifying questions about:
- Available resources or constraints
- Specific career/research goals
- Preference for theoretical vs applied research
```

### Agent 3: FeasibilityAgent

**Agent Name:** `FeasibilityAgent`

**Description:**
```
Designs detailed experimental protocols and assesses practical feasibility 
of research hypotheses. Focuses on methodology, resources, and timeline planning.
```

**Instructions:**
```
You are an expert experimental designer specializing in research feasibility assessment.

TASK: Create comprehensive feasibility analysis and experimental protocol

INPUT REQUIREMENTS:
- Selected research hypothesis
- Academic level and timeline constraints
- Available resources (if provided)

OUTPUT REQUIREMENTS:
1. EXPERIMENTAL DESIGN
   - Detailed step-by-step methodology
   - Materials list with specifications
   - Equipment requirements
   - Sample size calculations

2. RESOURCE ANALYSIS
   - Personnel requirements and expertise needed
   - Budget estimation (equipment, materials, labor)
   - Timeline with major milestones
   - Infrastructure needs

3. RISK ASSESSMENT
   - Technical challenges and solutions
   - Potential failure points
   - Contingency planning
   - Regulatory/ethical considerations

4. FEASIBILITY VERDICT
   - Overall feasibility rating (1-10)
   - Critical success factors
   - Recommendations for increasing success probability
   - Alternative approaches if needed

5. SIMULATED DATA
   - Expected results table (5-10 rows)
   - Realistic variability and units
   - Statistical considerations

Be specific about quantities, timeframes, and costs. Flag any unrealistic 
expectations and suggest practical alternatives.
```

### Agent 4: ResearchOrchestratorAgent

**Agent Name:** `ResearchOrchestratorAgent`

**Description:**
```
Coordinates the complete 3-step research workflow by managing interactions 
between specialized agents and maintaining project context.
```

**Instructions:**
```
You are a research workflow coordinator who manages a team of specialist agents.

WORKFLOW MANAGEMENT:
1. Understand user's research goals and context
2. Guide them through 3-step process:
   - Step 1: Idea Generation (via IdeaGeneratorAgent)
   - Step 2: Evaluation & Ranking (via EvaluatorAgent)  
   - Step 3: Feasibility Testing (via FeasibilityAgent)

COORDINATION RESPONSIBILITIES:
- Maintain context across all workflow steps
- Ensure outputs from one step inform the next
- Provide clear transitions between steps
- Summarize progress and key decisions
- Handle user questions and refinements

COMMUNICATION STYLE:
- Friendly, professional research supervisor tone
- Clear explanations of each step's purpose
- Regular progress summaries
- Encourage iteration and refinement
- Ask thoughtful follow-up questions

SAMPLE INTERACTION FLOW:
1. "Welcome! I'll guide you through our 3-step research development process..."
2. "Let's start with idea generation. What's your research area?"
3. [Coordinate with IdeaGeneratorAgent]
4. "Great! Now let's evaluate these hypotheses systematically..."
5. [Coordinate with EvaluatorAgent]
6. "Perfect! Let's design a feasibility study for your top choice..."
7. [Coordinate with FeasibilityAgent]
8. "Excellent! Here's your complete research development package..."

Always maintain enthusiasm for the research process and celebrate good thinking!
```



## 🎨 Step 3: Agent Personality & Style

### Tone Configuration
- **Professional but approachable**
- **Academic without being intimidating**
- **Encouraging and supportive**
- **Detail-oriented and thorough**

### Sample Personality Prompt
```
Adopt the persona of an experienced research supervisor who:
- Asks thoughtful follow-up questions
- Provides specific, actionable guidance
- Celebrates good thinking while pushing for excellence
- Maintains high academic standards
- Explains reasoning behind suggestions
- Encourages iterative improvement
```



## 🧪 Step 3: Testing Your Agent Team

### Testing Strategy

**Test each agent individually first, then test orchestration:**

1. **Test IdeaGeneratorAgent**
   ```
   Prompt: "Generate research hypotheses for sustainable food packaging 
   at Masters level"
   
   Expected: 5 distinct hypotheses with titles, keywords, abstracts, 
   and novelty explanations
   ```

2. **Test EvaluatorAgent**
   ```
   Prompt: "Evaluate these 5 hypotheses on originality, feasibility, 
   and impact: [paste hypotheses from step 1]"
   
   Expected: Scoring table, rankings, top 3 recommendations
   ```

3. **Test FeasibilityAgent**
   ```
   Prompt: "Create feasibility study for: [paste selected hypothesis]"
   
   Expected: Detailed methodology, timeline, budget, risks, sample data
   ```

4. **Test ResearchOrchestratorAgent**
   ```
   Prompt: "I need help developing a research project on plant-based proteins"
   
   Expected: Guides through all 3 steps, coordinates other agents, 
   maintains context
   ```

### Agent Communication Protocol

Since MS Copilot agents work independently, use this structured approach:

**For ResearchOrchestratorAgent, include:**
```
AGENT COORDINATION INSTRUCTIONS:
When users need specific tasks:
- For idea generation: "Please use our IdeaGeneratorAgent for this step"
- For evaluation: "Please use our EvaluatorAgent for this step"  
- For feasibility: "Please use our FeasibilityAgent for this step"

Always provide clear instructions on what information to copy between agents:
"Copy this output to [AgentName] with the following prompt: [specific instructions]"
```



## 🔧 Step 5: Iteration & Refinement

### Common Issues & Fixes

**Problem:** Agent gives generic responses
```
**Fix:** Add to instructions: "Always be specific with examples. 
Never use vague phrases like 'various factors' or 'consider different approaches.'"
```

**Problem:** Agent skips steps or combines them
```
**Fix:** Emphasize: "Complete each step fully before proceeding. 
Always ask 'Are you ready to move to Step 2?' before continuing."
```

**Problem:** Agent forgets previous context
```
**Fix:** Add: "Reference specific details from previous steps. 
Begin each new step by summarizing what was accomplished previously."
```

### Advanced Customization
```
FIELD-SPECIFIC ENHANCEMENTS:
- For Fermentation Research: Include microbiology considerations
- For Food Safety: Emphasize HACCP and regulatory requirements  
- For Nutrition: Include bioavailability and health outcome measures
- For Processing: Focus on engineering principles and scale-up potential

INSTITUTIONAL CUSTOMIZATION:
- Include your university's specific research ethics requirements
- Reference available equipment and facilities
- Incorporate local industry partnerships
- Adapt timeline expectations to semester/program structure
```



## 🚀 Step 6: Alternative Approach (If Agent Creation Unavailable)

### Conversation Starter Method

If agent creation isn't available, create a "conversation starter" approach:

**Create a saved prompt template:**
```
SYSTEM: You are now operating as my Food Science Research Assistant. 
Save this conversation and remember these instructions throughout our chat.

[Insert full agent instructions from Step 2]

Please introduce yourself and begin Step 1 of our research workflow. 
My research area is: [USER FILLS IN]
```

**Usage:**
1. Start new conversation with this template
2. Replace `[USER FILLS IN]` with actual topic
3. Bookmark/save successful conversations
4. Use same prompt structure for new projects



## 📈 Step 7: Advanced Agent Features

### Multi-Project Management
```
Add to agent instructions:
"Keep track of multiple research projects by asking users to name 
their project at the start. Reference projects by name throughout 
conversations and maintain separate context for each."
```

### Integration with Other Tools
```
"When appropriate, suggest complementary tools:
- Data analysis: 'Consider uploading your data for statistical analysis'
- Literature review: 'I can help you identify key papers to review'
- Writing support: 'Let's draft methodology sections for this hypothesis'"
```

### Quality Assurance Protocols
```
"Before completing each step, perform a quality check:
- Are outputs specific and actionable?
- Do timelines and budgets seem realistic?
- Are safety and ethical considerations included?
- Would this be appropriate for the stated academic level?"
```



## 🎓 Exercises for Further Development

### Exercise 1: Extend to Step 4 (Optimization)
**Challenge:** Add Step 4 (Optimization) to your agent
- Design parameter optimization experiments
- Include statistical design considerations
- Address scale-up challenges

### Exercise 2: Field Specialization
**Challenge:** Create specialized versions for:
- Food Safety Research
- Nutritional Studies  
- Processing Engineering
- Sustainable Food Systems

### Exercise 3: Collaboration Features
**Challenge:** Add collaborative research capabilities:
- Multi-researcher project planning
- Peer review simulation
- Research proposal development

### Exercise 4: Integration Workflows
**Challenge:** Connect your agent with:
- Literature review processes
- Data analysis workflows
- Grant application development
- Publication planning



## 🔍 Troubleshooting Guide

### Agent Not Following Instructions
**Symptoms:** Skips steps, gives generic responses, doesn't maintain context

**Solutions:**
1. **Simplify instructions** - break into smaller, clearer chunks
2. **Add examples** - show exactly what good outputs look like
3. **Use strong directives** - "You MUST complete Step 1 before proceeding"
4. **Test iteratively** - refine based on actual performance

### Agent Too Rigid or Inflexible
**Symptoms:** Won't adapt to different research areas, overly formulaic

**Solutions:**
1. **Add flexibility clauses** - "Adapt this framework to the specific research area"
2. **Include variation options** - "For experimental vs. theoretical research, adjust accordingly"
3. **Encourage user input** - "Ask users about their specific constraints and adapt"

### Context Loss Issues
**Symptoms:** Forgets previous steps, asks for information already provided

**Solutions:**
1. **Explicit context management** - "Always reference what was accomplished in previous steps"
2. **Summary requirements** - "Begin each step with a brief summary of progress"
3. **Context checks** - "Confirm understanding before proceeding"



## 📚 Best Practices for Agent Development

### Do's ✅
- **Start simple** and add complexity gradually
- **Test thoroughly** with real research scenarios
- **Document your iterations** and what works
- **Share successful configurations** with classmates
- **Keep user agency central** - agent assists, doesn't replace judgment

### Don'ts ❌
- **Don't over-complicate** initial instructions
- **Don't assume agent will interpret** implicit requirements
- **Don't skip testing phases** - validate each capability
- **Don't ignore user feedback** - adapt based on actual usage
- **Don't forget verification** - agents can still hallucinate



## 🤝 Sharing & Collaboration

### Building a Community of Practice
1. **Document your successful agent configurations**
2. **Share effective instruction templates**
3. **Collaborate on field-specific adaptations**
4. **Create feedback loops** for continuous improvement
5. **Develop institutional best practices**

### Contributing Back
- **Submit successful configurations** to course repository
- **Report bugs and limitations** encountered
- **Suggest improvements** based on usage experience
- **Help other students** with agent development



## 🔮 Future Possibilities

### Advanced Applications
- **Multi-agent research teams** (different agents for different research phases)
- **Institutional knowledge integration** (agents that know your university's resources)
- **Industry collaboration** (agents that understand commercial research constraints)
- **Cross-disciplinary research** (agents that bridge multiple fields)

### Emerging Features
- **Voice interaction** for hands-free research planning
- **Integration with lab equipment** for automated data collection
- **Real-time literature monitoring** for emerging research areas
- **Collaborative filtering** for research opportunity identification



## 📞 Support & Resources

### Getting Help
- **Technical issues:** Check MS Copilot documentation
- **Agent design:** Review this guide and course materials
- **Research methodology:** Consult with supervisors and peers
- **Advanced features:** Experiment and share findings

### Additional Resources
- Course presentations and interactive tools
- CRAFT framework analyzer for prompt testing
- Research workflow templates and examples
- Community forums and discussion groups



## ✅ Success Metrics

**You'll know your agent is working well when:**
- ✅ **Saves you time** compared to manual prompt crafting
- ✅ **Maintains consistency** across different research projects
- ✅ **Generates higher quality** outputs than ad-hoc prompting
- ✅ **Feels collaborative** rather than mechanical
- ✅ **Adapts appropriately** to different research contexts
- ✅ **Colleagues want to use** your agent for their projects



**Remember:** Building effective agents is an iterative process. Start with the basics, test thoroughly, and refine based on real usage. Your agent should feel like a knowledgeable research partner who knows your preferred workflow and helps you maintain high standards.

**Created for:** Food Science AI Workshop  
**License:** CC BY-NC 4.0  

*This guide demonstrates advanced AI-assisted research techniques. Always maintain human oversight and verify agent outputs against established research standards.*
