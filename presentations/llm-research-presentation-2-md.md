---
title: "From Manual to Magical"
subtitle: "Hands-on Practice & Creating Your AI Research Agent"
author: "Michael Borck"
format: 
  pptx: default
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

## Welcome Back! 🚀 {background-color="#1a1a1a"}

### Session 2: Let's Build Something Amazing

:::: {.columns}
::: {.column width="50%"}
**What We'll Do:**
- Practice the workflow hands-on
- Analyze real(istic) food science data
- Create your own AI research agent
- Level up your research game
:::

::: {.column width="50%"}
**What You Need:**
- Microsoft Copilot access
- One of our datasets
- Your curiosity!
- **A research topic in mind**
:::
::::

. . .

::: {.callout-important}
**Today's Goal:** By the end, you'll have a personal AI research assistant that knows the 10-step workflow!
:::

::: {.notes}
Welcome back! Now we move from theory to practice. Everyone should have Copilot open.
:::

---

## System Check & Troubleshooting 🔧

### Quick Tech Inventory

**✅ Can you access:**
- Microsoft Copilot (copilot.microsoft.com)
- File download capability
- New chat sessions

. . .

### Common Issues & Quick Fixes

| Problem | Solution |
|---------|----------|
| "Can't upload files" | Try bing.com/chat or ChatGPT |
| "Response seems generic" | Add "Be specific" to prompts |
| "AI is confused" | Start new chat session |
| "Access denied" | Try incognito/private browsing |

. . .

::: {.callout-tip}
**Help available:** Raise your hand anytime - we'll have micro-breaks every 15 minutes!
:::

---

## Quick Recap: The 10-Step Workflow 📋

### The Complete Research Journey ⏱️ *~100 minutes total*

:::: {.columns}
::: {.column width="50%"}
**Discovery Phase** *(60 min)*
1. Idea Generation *(8 min)*
2. Parallel Exploration *(12 min)*
3. Feasibility Testing *(10 min)*
4. Optimization *(15 min)*
5. Full Execution *(15 min)*
:::

::: {.column width="50%"}
**Communication Phase** *(40 min)*
6. Component Analysis *(8 min)*
7. Visualization *(10 min)*
8. Writing *(12 min)*
9. Review *(5 min)*
10. Iteration *(5 min)*
:::
::::

. . .

::: {.callout-tip}
Today we'll practice Steps 1-3 together, demo 4-7, then build an agent to do it all!
:::

---

## Let's Get Started! 🎯 {background-color="#1a2c1a"}

### Step 1: Idea Generation *(8 minutes)*

**Everyone follow along:**

1. Open Microsoft Copilot
2. Copy this prompt exactly:

```text
You are an AI research scientist specializing in Food Science.
Given the following research area, generate 5 distinct and 
innovative scientific hypotheses suitable for a Masters-level 
research paper.

For each hypothesis, include:
- A clear Title
- 3-5 Keywords  
- A short Abstract (under 200 words)
- An explanation of its Novelty and Significance

Research Area: "Plant-based dairy alternatives"
```

::: {.callout-note}
**Timer:** Take exactly 5 minutes to run this and read the results
:::

::: {.notes}
Give students 2-3 minutes to run this. Walk around and help anyone struggling.
:::

---

## What Did You Notice? 🤔

### Share Your Observations *(3 minutes)*

:::: {.incremental}
- Did Copilot generate exactly 5 hypotheses?
- Were they all truly distinct?
- How was the formatting?
- Any surprising ideas?
- Quality of the abstracts?
::::

. . .

::: {.callout-important}
**Key Learning:** Even with identical prompts, AI can generate different outputs. This diversity is a feature, not a bug!
:::

. . .

## Introducing CRAFT: Better Prompts, Better Results 🎯

### The Problem You Just Experienced
- Vague outputs? Missing context.
- Generic responses? No role assigned.
- Wrong format? Didn't specify what you wanted.

. . .

### The CRAFT Solution

| **C** | **Context** | "This is food science research data..." |
| **R** | **Role** | "You are an expert food scientist..." |
| **A** | **Action** | "Generate 5 innovative hypotheses..." |
| **F** | **Format** | "Present as a structured table..." |
| **T** | **Tone/Target** | "Use academic language for peer review..." |

. . .

::: {.callout-tip}
**Try it now:** Look at the prompt you just used. Which CRAFT elements were missing? How could you improve it?
:::

. . .

**Remember:** CRAFT is your conversation starter, not your final answer. Follow up, refine, iterate!

### Success Check: ✅
- Ideas are specific and detailed
- Academic language throughout
- Clear research questions

### Red Flags: ❌
- Vague or generic suggestions
- Repetitive ideas
- No specific methodology mentioned

---

## Exporting Your Results 📊

### Making Your Work Persistent

**In Copilot:**
1. Look for the **"Export"** or **"Copy"** button
2. Options might include:
   - Copy to clipboard
   - Export to Word
   - Export to Excel (for tables)

. . .

**Pro Tip:** Create a folder structure now:
```
Research_Project_[Today's Date]/
├── 01_Ideas/
├── 02_Experiments/
├── 03_Data/
├── 04_Analysis/
└── 05_Manuscripts/
```

. . .

::: {.callout-tip}
**Organization = Success:** Name files with step numbers so you can track progress!
:::

---

## Step 2: Scoring and Selection 🎯

### Copy your hypotheses back into Copilot *(5 minutes)*

**New prompt:**
```text
Here are 5 research hypotheses I generated. 
Please score each from 1-10 on:
- Originality (1=common, 10=groundbreaking)
- Feasibility (1=impossible, 10=easily doable for Masters)  
- Potential Impact (1=minor contribution, 10=field-changing)

Present as a table with total scores and recommend the top 3.
Explain your reasoning for the scores.

[PASTE YOUR 5 HYPOTHESES HERE]
```

. . .

**Take 3 minutes to run this, then we'll discuss results**

. . .

**Question:** Which hypothesis scored highest? Do you agree with the AI's reasoning?

---

## Step 3: Feasibility Testing 🧪

### Let's Design an Experiment! *(10 minutes)*

**Select your top hypothesis and use this prompt:**

```text
I have selected this hypothesis:
[PASTE YOUR #1 HYPOTHESIS]

Design a minimal, step-by-step experimental plan to test 
its basic feasibility. This should be a small-scale 
prototype, not a full study.

Include:
- Materials needed (be specific about equipment)
- Step-by-step procedure (numbered list)
- Expected measurements and units
- Estimated timeline with milestones
- Budget estimate (if possible)
- Potential challenges and solutions

After the plan, generate a small table of simulated 
data (5-10 rows) showing what results we might expect.
```

::: {.callout-note}
**Timer:** 7 minutes to run this, 3 minutes to review your results
:::

---

## Checkpoint: Evaluating Your Progress 📊

### Success Metrics for Steps 1-3

**Your outputs should have:**

:::: {.columns}
::: {.column width="50%"}
**✅ Quality Indicators:**
- Specific numerical values
- Clear timelines
- Detailed procedures
- Realistic resource needs
- Academic language
:::

::: {.column width="50%"}
**❌ Warning Signs:**
- Vague instructions
- Unrealistic timelines
- Missing key details
- Generic recommendations
- No specific measurements
:::
::::

. . .

### Quick Poll: How Are We Doing?
- 🟢 **Green:** My outputs are detailed and actionable
- 🟡 **Yellow:** Some good parts, some vague parts  
- 🔴 **Red:** Most outputs are too generic

::: {.callout-tip}
**If you're yellow/red:** Try adding "Be more specific" to your prompts!
:::

---

## Time for the Data Demo! 📈 {background-color="#1a1a2c"}

### Your Choice Matters

Let's see which dataset won our poll!

. . .

::: {.callout-note}
## 🎉 The Winner Is...
[Announce the winning dataset]
:::

. . .

### Important Disclaimer

::: {.callout-warning}
**Synthetic Data Notice:** These datasets were created specifically for this demonstration. While the data is simulated, the analysis techniques are 100% real and applicable to your actual research data!

*Datasets created with assistance from Claude (Anthropic)*
:::

---

## Dataset Download & Setup 📁

### Get Ready for Analysis *(3 minutes)*

1. **Click this link:** [Insert GitHub link to winning dataset]
2. **Download** the CSV file to your computer
3. **Note the file location** (probably Downloads folder)
4. **Keep the browser tab open** with the dataset description

. . .

### While You Download...

**Dataset Preview:** [Show brief description of winning dataset structure]
- **Rows:** X observations
- **Columns:** Y variables
- **Study type:** [Fermentation/Shelf-life/Sensory/Process]
- **Key variables:** [List main measurements]

. . .

::: {.callout-tip}
**Pro tip:** Real research data often has missing values, errors, and inconsistencies - our clean dataset makes learning easier!
:::

---

## Uploading and Analyzing Data 📊

### Follow Along - Steps 4-5 Demo *(15 minutes)*

**Step 1: Upload** *(2 min)*
1. **In Copilot**, click the **attachment/paperclip** icon
2. **Select** your downloaded CSV file
3. **Wait** for upload confirmation

. . .

**Step 2: Initial Analysis** *(3 min)*
```text
I've uploaded a food science dataset. Please:
1. Describe what type of study this represents
2. List all the variables/columns and their units
3. Provide basic statistics (mean, min, max) for numerical columns
4. Tell me how many observations are in the dataset
5. Identify any missing or unusual values
```

::: {.callout-note}
**Take 2 minutes** to run this and read the results carefully
:::

::: {.notes}
Give students time to upload. Help anyone having issues.
:::

---

## Exploratory Data Analysis 🔍

### Let's Dig Deeper! *(12 minutes total)*

**Prompt 1:** *(3 min)*
```text
What patterns or trends do you see in this data? 
Look for relationships between variables, changes over time, 
and differences between groups/treatments.
```

. . .

**Prompt 2:** *(3 min)*
```text
Which treatment/product/condition performs best? 
Explain your reasoning with specific numbers from the data.
```

. . .

**Prompt 3:** *(3 min)*
```text
Are there any concerning or unexpected values? 
What questions would a peer reviewer ask about this data?
```

. . .

::: {.callout-tip}
Notice how we're using natural language instead of coding? This is the power of AI-assisted analysis!
:::

**Debrief:** *(3 min)* Share one interesting finding with the person next to you

---

## Creating Visualizations 📊

### A Picture Worth 1000 Data Points *(10 minutes)*

**Visualization prompt:** *(7 min)*

```text
Create a professional scientific figure showing:
[CUSTOMIZE BASED ON DATASET]:
- Fermentation: pH over time for all treatments with error bars
- Shelf life: Quality score degradation curves by product
- Sensory: Spider/radar chart comparing all products  
- Process: 3D surface plot showing yield vs temperature and pH

Requirements:
- Include proper axis labels with units
- Add a clear legend
- Use scientific color scheme
- Write a detailed figure caption
- Suggest statistical tests for the differences shown
```

. . .

**Image troubleshooting:** *(3 min)*
- Can't see the image? Check browser permissions
- Image looks wrong? Try "regenerate" or refine the prompt
- No image capability? The data interpretation is still valuable!

---

## Advanced Statistical Analysis 🧮

### Getting Sophisticated *(8 minutes)*

**Let's get statistical:**
```text
Perform appropriate statistical analysis for this dataset:

1. Are the differences between groups statistically significant? 
   Suggest and explain appropriate tests.

2. What correlations exist between variables? 
   Report correlation coefficients where relevant.

3. Can you build a simple predictive model? 
   Which variables best predict the main outcome?

4. What would you recommend based on this data? 
   Provide specific, actionable conclusions.

5. What are the limitations of this analysis?
   What additional data would strengthen the conclusions?
```

. . .

::: {.callout-warning}
**Remember:** AI-generated statistics should be verified with proper statistical software for publication!
:::

. . .

**Review time:** *(2 min)* Does the statistical approach make sense for your data type?

---

## From Data to Presentation 🎤

### The Magic Move *(7 minutes)*

**Final data prompt:**

```text
Based on all our analysis, create a 3-slide PowerPoint summary:

Slide 1: Study Overview
- Study design and objectives
- Key variables measured
- Sample size and methodology

Slide 2: Key Results 
- Include the main figure we created
- 2-3 bullet points of key findings
- Statistical significance where appropriate

Slide 3: Conclusions and Recommendations
- Main takeaways for food scientists
- Practical applications
- Future research directions

Make it professional and suitable for a research meeting.
Use clear, scientific language.
```

. . .

**Watch for:** The export to PowerPoint option! 

::: {.callout-tip}
**If export fails:** Copy the text and paste into PowerPoint manually - still much faster than writing from scratch!
:::

---

## Reflection Moment 🤔

### What Just Happened?

In **under 30 minutes**, we:
- ✅ Analyzed a complete dataset
- ✅ Generated publication-quality figures
- ✅ Performed statistical analysis
- ✅ Created a research presentation
- ✅ Identified future research directions

. . .

### Traditional Approach Time:
- Data cleaning: 2-3 hours
- Statistical analysis: 4-6 hours  
- Figure creation: 2-4 hours
- Writing: 3-5 hours
- **Total: 11-18 hours**

. . .

::: {.callout-important}
**But remember:** We still need human expertise to:
- Verify statistical validity
- Ensure scientific accuracy
- Make strategic decisions
- Connect to broader theory
- Design the actual experiments
:::

---

## The Evolution: AI Agents 🤖 {background-color="#2c1a1a"}

### From Manual to Automated

**Current approach:** You copy-paste prompts step by step

**Agent approach:** AI guides YOU through the process

. . .

:::: {.columns}
::: {.column width="50%"}
**Manual = You're the Driver**
- Full control over every step
- Need to remember all prompts
- Time-consuming setup
- Error-prone transitions
- Easy to skip steps
:::

::: {.column width="50%"}
**Agent = You're the Pilot**
- AI navigates the workflow
- You make key decisions
- Faster transitions
- Consistent quality
- Guided learning
:::
::::

. . .

::: {.callout-tip}
**Think of it like:** GPS for research - you choose the destination, it finds the best route
:::

---

## Agent Benefits: Why This Matters 💪

### Real-World Applications

:::: {.columns}
::: {.column width="50%"}
**For Students:**
- Never forget workflow steps
- Consistent high-quality outputs
- Learn best practices automatically
- Focus on science, not prompts
- Build confidence with AI tools
:::

::: {.column width="50%"}
**For Researchers:**
- Standardize lab procedures
- Train new team members faster
- Ensure reproducible workflows
- Scale successful approaches
- Integrate with existing tools
:::
::::

. . .

### Success Stories

::: {.callout-note}
**"I used to spend hours crafting prompts. Now my agent walks me through everything in minutes, and the quality is consistently better."** - Food Science PhD Student
:::

---

## Creating Your Research Agent 🛠️

### Let's Build Together! *(20 minutes)*

**In Microsoft Copilot:** *(Or ChatGPT/Claude if Copilot doesn't support agents)*

1. Look for **"Create GPT"** or **"Custom Instructions"** option
2. We'll name it: **"Food Science Research Assistant"**

. . .

**If your platform doesn't support agents:**
- Don't worry! We'll create a detailed instruction document
- You can copy-paste these instructions at the start of any chat
- Same functionality, just manual setup

. . .

**Agent Description:**
```text
An expert AI research assistant that guides food science 
students through a 10-step scientific discovery process, 
from hypothesis generation to manuscript preparation.
Maintains conversation context and tracks progress.
```

---

## Agent Instructions: The Brain 📝

### Core Behavior Instructions *(10 minutes)*

**Copy this instruction set:**

```text
You are an expert AI research scientist specializing in Food Science, 
designed to guide Masters students through a 10-step research process.

CORE BEHAVIOR:
1. Always track which step the user is currently on
2. Introduce each step clearly before asking for input
3. Execute the step based on user input with high detail
4. Present results in organized, academic format
5. Ask if they're ready for the next step or want refinements
6. Remember context from all previous steps
7. Provide specific, actionable outputs (not generic advice)
8. Include time estimates for each step

THE 10 STEPS WITH DETAILS:
1. Idea Generation (8 min): Generate 5 distinct hypotheses with abstracts
2. Parallel Exploration (12 min): Score and rank ideas, select top candidates  
3. Feasibility Testing (10 min): Design minimal experimental protocols
4. Optimization (15 min): Refine parameters and variables
5. Full Execution (15 min): Complete methodology and expected outcomes
6. Component Analysis (8 min): Identify critical success factors
7. Visualization (10 min): Create figures with scientific captions
8. Writing (12 min): Draft complete manuscript sections
9. Review (5 min): Peer review simulation with scoring
10. Iteration (5 min): Refine based on feedback

Always maintain a friendly, educational tone and explain 
why each step matters for research success. Provide specific 
examples relevant to food science when possible.
```

::: {.callout-tip}
**Customization tip:** Add your specific research area (fermentation, packaging, etc.) for more targeted help
:::

---

## Testing Your Agent 🧪

### Live Beta Test! *(10 minutes)*

**Someone volunteer to test live!**

**Starter prompt:**
> "Hello, I'd like help with my research project on [INSERT TOPIC]"

. . .

**What we're watching for:**
- ✅ Does it introduce Step 1 clearly?
- ✅ Does it wait for your input before proceeding?
- ✅ Does it provide specific, detailed outputs?
- ✅ Does it remember context between steps?
- ✅ Does it feel like a helpful research partner?

. . .

### Common Issues & Fixes:
- **Too generic?** → Add "Be specific with examples"
- **Skips steps?** → Emphasize "one step at a time"
- **Forgets context?** → Start fresh, might be a long conversation

::: {.callout-tip}
**Success indicator:** The agent should feel like a knowledgeable lab supervisor, not a rigid script!
:::

---

## Agent Superpowers 💪

### What Makes Agents Special?

:::: {.incremental}
1. **Memory:** Tracks your progress through all 10 steps automatically
2. **Consistency:** Same high-quality process every single time
3. **Guidance:** No need to remember complex prompts or templates
4. **Adaptation:** Adjusts to your specific research area and level
5. **Efficiency:** Streamlines the entire workflow with smart transitions
6. **Learning:** Builds better prompts based on your preferences
::::

. . .

### Real-World Benefits:

::: {.callout-note}
**Before Agent:** "What was that prompt for step 7 again? Let me find my notes..."

**With Agent:** "Continue to step 7" → Perfect visualization prompts automatically generated
:::

. . .

::: {.callout-important}
Think of it as having a PhD supervisor available 24/7 who never gets tired or forgets your research context!
:::

---

## Advanced Agent Features 🔧

### Level Up Your Assistant *(Optional)*

**Advanced instructions to add:**

```text
ADVANCED FEATURES:
- If user uploads data, automatically suggest appropriate analysis
- For literature reviews, provide citation templates
- When writing, include proper scientific formatting
- Suggest relevant statistical tests based on data type
- Flag potential ethical considerations
- Recommend journal targets based on research scope
- Generate conference abstract versions
- Create grant application outlines

CUSTOMIZATION BY FIELD:
- Fermentation: Focus on microbiology and biochemistry
- Packaging: Emphasize materials science and shelf life
- Nutrition: Include bioavailability and health outcomes
- Processing: Highlight engineering and food safety aspects
```

. . .

::: {.callout-tip}
**Pro tip:** Add these features gradually as you become more comfortable with the basic workflow
:::

---

## Your Research Toolkit 🧰 {background-color="#1a2c1a"}

### What You've Gained Today

✅ **Structured Workflow:** 10-step process from idea to publication

✅ **Practical Skills:** Data analysis without coding expertise

✅ **AI Agent:** Your personal research assistant with institutional memory

✅ **Critical Thinking:** Understanding AI limitations and verification needs

✅ **Time Management:** 100-minute complete research workflow

. . .

### Resources to Take Home:
- **Enhanced presentation slides** (PDF, HTML, PPTX)
- **All 4 practice datasets** with documentation
- **Complete prompt template library** 
- **Agent instruction templates** (basic + advanced)
- **Troubleshooting guide** for common issues

---

## Real-World Integration 🔄

### Making This Work in Your Studies

**This Week:**
1. **Try the workflow** on your actual research topic
2. **Customize your agent** with your specific field
3. **Share with classmates** - collective improvement
4. **Document what works** - build your personal prompt library

. . .

**This Month:**
- Integrate with existing research projects
- Use for literature reviews and grant applications
- Train your research group on the workflow
- Develop field-specific modifications

. . .

**Best Practices for Long-term Success:**
- **Always verify** AI outputs with peer-reviewed sources
- **Keep humans central** to all decision-making
- **Document your process** for reproducibility
- **Iterate and improve** based on results

---

## Ethical Guidelines & Academic Integrity 📜

### Using AI Responsibly in Research

**Required Citation Example:**
> "Research methodology development was assisted by a custom AI agent based on Microsoft Copilot (Microsoft Corporation, 2024). All generated hypotheses and experimental designs were subsequently validated against peer-reviewed literature. Statistical analyses were verified using [appropriate software]."

. . .

**What to Cite:**
- ✅ Hypothesis generation assistance
- ✅ Experimental design suggestions  
- ✅ Data analysis approaches
- ✅ Writing structure and organization

**What Not to Cite:**
- Grammar and spell checking
- Basic calculations
- Reference formatting

. . .

::: {.callout-warning}
**Institution-specific guidelines:** Always check your university's AI policy - requirements may vary!
:::

---

## Next Steps & Advanced Applications 📚

### Your Research Journey Continues

:::: {.columns}
::: {.column width="50%"}
**Immediate Next Steps:**
1. Apply workflow to current projects
2. Experiment with different prompts
3. Build your personal template library
4. Share successes (and failures!) with peers
:::

::: {.column width="50%"}
**Advanced Applications:**
- Multi-study meta-analyses
- Grant proposal development
- Conference presentation creation
- Peer review simulation
- Research collaboration planning
:::
::::

. . .

### Community & Continuous Learning:

::: {.callout-tip}
**Join the conversation:** Consider creating a study group to share AI research techniques and improve workflows together
:::

. . .

**Resources for Continued Learning:**
- University AI research guidelines
- Food science AI application papers
- Prompt engineering best practices
- Research methodology updates

---

## Troubleshooting & Support 🛠️

### When Things Don't Work

**Common Issues & Solutions:**

| Issue | Quick Fix | Long-term Solution |
|-------|-----------|-------------------|
| Agent gives generic responses | Add "Be specific with examples" | Refine instructions with more detail |
| Forgets previous steps | Start new chat session | Use platform with better memory |
| Analysis seems wrong | Cross-check with known methods | Always verify with domain experts |
| Can't upload data | Try different browser/platform | Have multiple platform accounts |

. . .

### Getting Help:
- **During class:** Immediate assistance available
- **After class:** Email with specific examples
- **Peer support:** Form study groups for collaborative problem-solving
- **Platform updates:** AI tools change rapidly - stay flexible

. . .

::: {.callout-important}
**Remember:** Technology fails sometimes. The workflow principles remain valuable even when specific tools don't cooperate!
:::

---

## Q&A and Exploration Time 🎯 {background-color="#1a1a1a"}

### Your Questions, Your Projects *(15 minutes)*

**Let's Discuss:**
- Specific research applications in your field?
- Technical challenges with your setup?
- Ethical considerations for your institution?
- Integration with existing research tools?
- Customizations for your research area?

. . .

### Try This Now:
**Live practice:** Pick a research question from your current studies and run it through Steps 1-3 with your new agent!

. . .

**Contact Information:**
- **Email:** [your-email@curtin.edu.au]
- **Office hours:** [Insert schedule]
- **Course materials:** [GitHub repository link]

---

## Final Reflection & Success Metrics 📊

### Measuring Your Progress

**By the end of today, you should be able to:**
- ✅ Break complex research tasks into manageable steps
- ✅ Write effective prompts for each workflow stage
- ✅ Critically evaluate AI-generated outputs
- ✅ Create and customize your own research agent
- ✅ Integrate AI tools with traditional research methods

. . .

### Self-Assessment Questions:
1. Can you explain the 10-step workflow to a colleague?
2. Do you feel confident starting a research project with AI assistance?
3. Can you identify when AI outputs need human verification?
4. Would you recommend this approach to other researchers?

. . .

::: {.callout-tip}
**Success indicator:** You're excited to try this on your own research, not overwhelmed by the complexity!
:::

---

## Thank You! 🙏

### You're Now AI-Empowered Researchers!

::: {.callout-tip}
## Remember: Amplification, Not Replacement
You're not replacing your scientific expertise—you're amplifying it with powerful AI tools that handle routine tasks so you can focus on creative thinking and critical analysis.
:::

. . .

### The Journey Continues:
- **Today:** You learned the workflow and built your agent
- **Tomorrow:** You apply it to real research challenges  
- **Next month:** You're mentoring others in AI-assisted research
- **Next year:** You're publishing papers that showcase the power of human-AI collaboration

. . .

**Created with assistance from Claude (Anthropic)**

### Happy Researching! 🚀

::: {.callout-note}
**All course materials, including presentations, datasets, audio guides, and interactive tools, will remain available at:** [GitHub Pages URL]
:::

