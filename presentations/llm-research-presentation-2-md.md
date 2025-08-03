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

# Welcome Back! 
:::: {.columns}
::: {.column width="50%"}
**What We'll Do:**

- Practice the workflow hands-on
- Analyse real(istic) food science data
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

**Today's Goal:** By the end, you'll confidently use AI for your own research projects!

# System Check & Troubleshooting

**Quick Tech Inventory**

**✅ Can you access:**

- Microsoft Copilot (copilot.microsoft.com)
- File download capability
- New chat sessions

**Common Issues & Quick Fixes**

| Problem | Solution |
|---------|----------|
| "Response seems generic" | Add "Be specific" to prompts |
| "AI is confused" | Start new chat session |
| "Access denied" | Try incognito/private browsing |

**Help available:** Raise your hand anytime - we'll have micro-breaks every 15 minutes!

# Quick Recap: The 10-Step Workflow

 Step | Task | Time | Output |
|---|------|------|--------|
| 1 | Idea Generation | 8 min | 5 hypotheses table |
| 2 | Parallel Exploration | 12 min | 10-15 total ideas |
| 3 | Feasibility Testing | 10 min | Experimental plan + data |
| 4 | Optimisation | 15 min | Best parameters |
| 5 | Full Study | 15 min | Complete methodology |
| 6 | Component Analysis | 8 min | Key factors identified |
| 7 | Visualisation | 10 min | Figures + captions |
| 8 | Writing | 12 min | Full paper draft |
| 9 | Review | 5 min | Feedback report |
| 10 | Iteration | 5 min | Refined manuscript |

Today we'll practice Steps 1-3 together, then learn to build systems to handle the rest!

# Let's Get Started! 


## Step 1: Idea Generation 

**Everyone follow along:**

1. Open Microsoft Copilot
2. Copy this prompt exactly:

```
"What are some food science research ideas?"
```

# What Did You Notice? 🤔

- Did Copilot generate hypotheses?
- Were they all truly distinct?
- How was the formatting?
- Any surprising ideas?
- Quality of the abstracts?


# **The Problem We Experienced**

- Vague outputs? Missing context.
- Generic responses? No role assigned.
- Wrong format? Didn't specify what you wanted.

# Introducing CRAFT: Better Prompts, Better Results

| Key | Section       | Description                               |
|-----|---------------|-------------------------------------------|
| **C** | **Context**    | "This is food science research data..."   |
| **R** | **Role**       | "You are an expert food scientist..."    |
| **A** | **Action**     | "Generate 5 innovative hypotheses..."    |
| **F** | **Format**     | "Present as a structured table..."        |
| **T** | **Tone/Target**| "Use academic language for peer review..."|

**Try it now:** Look at the earlier prompt. Which CRAFT elements were missing? How could you improve it?

**Remember:** CRAFT is your conversation starter, not your final answer. Follow up, refine, iterate!

# CRAFT Analysis

**❌ Before CRAFT (weak example):**

```
"What are some food science research ideas?"
```
or 

```
"Give me some research ideas about plant milk."
```

**Missing:**
- ❌ **Context:** No research level, paper type, or constraints
- ❌ **Role:** AI doesn't know what expertise to use
- ❌ **Action:** Vague "some ideas" vs. specific "5 hypotheses"
- ❌ **Format:** No structure for output
- ❌ **Tone:** Unclear if academic, industry, or casual


# Let's Get Started! (again!)

**Everyone follow along with YOUR topic:**

1. Open Microsoft Copilot
2. Use this CRAFT template with YOUR research area:

```
You are an AI research scientist specialising in Food Science.
Given the following research area, generate 5 distinct and 
innovative scientific hypotheses suitable for a Masters-level 
research paper.

For each hypothesis, include:
- A clear Title
- 3-5 Keywords  
- A short Abstract (under 200 words)
- An explanation of its Novelty and Significance

Research Area: "[YOUR TOPIC FROM HOMEWORK]"
```

# What Did You Notice?

**Share Your Observations** 

- Did Copilot generate exactly 5 hypotheses?
- Were they all truly distinct?
- How was the formatting?
- Any surprising ideas?
- Quality of the abstracts?

**Key Learning:** Even with identical CRAFT structures, AI generates different outputs based on YOUR specific topic. This diversity is valuable!


# ✅ **CRAFT Analysis of This Prompt:**

| Element | ✅/❌ | What's There |
|---------|-------|-------------|
| **C**ontext | ✅ | "Given the following research area" + "Masters-level research paper" |
| **R**ole | ✅ | "You are an AI research scientist specialising in Food Science" |
| **A**ction | ✅ | "generate 5 distinct and innovative scientific hypotheses" |
| **F**ormat | ✅ | Detailed list: Title, Keywords, Abstract, Novelty explanation |
| **T**one/Target | ✅ | "scientific hypotheses" + "Masters-level" = academic tone |

::: {.notes}
**This is Actually a STRONG Prompt!**

**Why it works well:**

- **Specific role:** AI knows to think like a food science researcher
- **Clear task:** Exactly 5 hypotheses, not vague "some ideas"
- **Detailed format:** Structured output requirements
- **Appropriate level:** Masters-level sets the complexity
- **Rich context:** Specific research area provided
:::

# Did it work?

**Success Check: ✅**

- Ideas are specific and detailed
- Academic language throughout
- Clear research questions

**Red Flags: ❌**

- Vague or generic suggestions
- Repetitive ideas
- No specific methodology mentioned

# Step 2: Scoring and Selection

**Copy your hypotheses back into Copilot** 

**New CRAFT prompt:**

```
Here are 5 research hypotheses I generated. 
Please score each from 1-10 on:
- Originality (1=common, 10=groundbreaking)
- Feasibility (1=impossible, 10=easily doable for Masters)  
- Potential Impact (1=minor contribution, 10=field-changing)

Present as a table with total scores and recommend the top 3.
Explain your reasoning for the scores.

[PASTE YOUR 5 HYPOTHESES HERE]
```

**Take 3 minutes to run this, then we'll discuss results**

**Question:** Which hypothesis scored highest? Do you agree with the AI's reasoning?

# Step 3: Feasibility Testing

**Let's Design an Experiment!**

**Select your top hypothesis and use this CRAFT prompt:**

```
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

# **Success Metrics for Steps 1-3**

**Your outputs should have:**

**✅ Quality Indicators:**

- Specific numerical values
- Clear timelines
- Detailed procedures
- Realistic resource needs
- Academic language

**❌ Warning Signs:**

- Vague instructions
- Unrealistic timelines
- Missing key details
- Generic recommendations
- No specific measurements

# Quick Self Assessment

**Quick Poll: How Are We Doing?**

- 🟢 **Green:** My outputs are detailed and actionable
- 🟡 **Yellow:** Some good parts, some vague parts  
- 🔴 **Red:** Most outputs are too generic

**If you're yellow/red:** Try adding "Be more specific" to your prompts!

# Working with Real Data (Optional Demo)

**If You Have Data to Practice With...**

**For those who brought data or want to try our sample datasets:**

1. **Upload your CSV** to Copilot
2. **Ask basic questions** about patterns and trends
3. **Request simple visualisations**
4. **Generate interpretations**

# Sample CRAFT prompt for data:**
```
I've uploaded a food science dataset from [study type/context]. 
You are an experienced data analyst specialising in food research. 
Summarise the key findings and suggest 3 areas for deeper 
investigation that would be suitable for follow-up studies. 
Present as bullet points suitable for a research meeting, 
with each point including a brief rationale.
```
**Remember:** Always verify AI interpretations of your data!


# C.R.A.F.T Analysis

| Element | ✅/❌ | What's There |
|---------|-------|-------------|
| **C**ontext | ✅ | "I've uploaded a dataset form [study/type]" |
| **R**ole | ✅ | "You are an experienced food research data analyst" |
| **A**ction | ✅ | "Summarise key findings and suggest 3 areas for deeper investigation" |
| **F**ormat | ✅ | "Present as bullet points" |
| **T**one/Target | ✅ | "suitable for a research meeting and rationale" (professional/academic tone) |

::: {.notes}
**Why This Works Well:**

- **Clear context** about the data type
- **Specific role** that guides AI's analytical approach
- **Dual action** with exact quantity (3 areas)
- **Defined format** (bullet points)
- **Audience-specific tone** (research meeting = professional)
:::

# Building Your Research Process

**From Manual Steps to Systematic Approach**

**What we just did manually:**

- Step 1: Generated ideas with specific prompts
- Step 2: Evaluated and ranked systematically  
- Step 3: Designed feasibility studies

**How to make this repeatable:**

1. **Save your successful prompts** in a document
2. **Create templates** for your research area
3. **Build prompt libraries** for different tasks
4. **Develop your personal workflow**

**The goal:** Turn today's manual process into your efficient research system

# Advanced CRAFT Techniques

**Beyond the Basics**

**Prompt Chaining:**

1. "Generate 5 hypotheses about [topic]"
2. "Score the above hypotheses for feasibility"
3. "Design an experiment for the top-ranked hypothesis"

**Role Switching:**

- "As a journal reviewer, critique this hypothesis"
- "As an industry expert, assess commercial potential"
- "As a student, explain this in simple terms"

**Iterative Refinement:**

- "Make this more specific"
- "Add industry applications"
- "Consider budget constraints"
- "Include potential risks"

# Your Personal Prompt Library

**Start Building Today**

**Essential Templates to Save:**

**Idea Generation:**
```
You are an AI research scientist specialising in [FIELD].
Generate [NUMBER] innovative hypotheses for [LEVEL]-level 
research on [TOPIC]. Include title, keywords, abstract, 
and significance for each.
```

**Literature Review:**
```
You are an academic researcher. Summarise the current state 
of research on [TOPIC]. Identify 3 key gaps that warrant 
further investigation. Use academic tone suitable for 
peer review.
```

**Methodology Design:**
```
Design a [SCALE] experimental protocol to test [HYPOTHESIS].
Include materials, procedures, measurements, timeline, and 
expected challenges. Present as a structured research plan.
```

# Quality Control and Verification

**Your AI Safety Checklist**

**Always Check:**
- ✅ Do the numbers make scientific sense?
- ✅ Are the methodologies appropriate for the question?
- ✅ Do timelines and budgets seem realistic?
- ✅ Are safety and ethical considerations included?
- ✅ Can you actually access the suggested equipment/materials?

**Red Flags:**
- ❌ Unusually perfect or round numbers
- ❌ Methodologies that seem too complex or too simple
- ❌ Missing safety protocols
- ❌ Unrealistic timelines or budgets
- ❌ Citations you can't verify

**When in doubt:** Ask a follow-up question or consult with supervisors

# Reflection Moment

**What You've Accomplished Today**

**In 30 minutes of hands-on practice:**
- ✅ Generated research hypotheses for YOUR topic
- ✅ Systematically evaluated and ranked ideas
- ✅ Designed feasibility studies
- ✅ Learned CRAFT framework for better prompts
- ✅ Built your personal prompt templates

**Traditional Approach Time:**
- Literature review to find gaps: 2-3 weeks
- Hypothesis development: 1-2 weeks
- Initial experimental design: 1 week
- **Total: 4-6 weeks**

**But remember:** AI accelerates the process - human expertise ensures quality and makes final decisions

# Integration with Your Studies

**Making This Work in Real Research**

**This Week:**

1. **Apply the 3-step process** to your current assignments
2. **Build your prompt library** with successful templates
3. **Practice CRAFT framework** on different topics
4. **Share successes** (and failures!) with classmates

**This Month:**

- Use for literature reviews and research proposals
- Apply to lab report writing and data interpretation
- Integrate with thesis planning and development
- Develop field-specific prompt variations

**This Semester:**

- Build comprehensive research workflows
- Create collaboration templates for group projects
- Develop peer review and feedback processes

# Best Practices for Long-term Success

**Sustainable AI-Assisted Research**

**Do:**

- ✅ **Always verify** AI outputs with peer-reviewed sources
- ✅ **Keep humans central** to all strategic decisions
- ✅ **Document your processes** for reproducibility
- ✅ **Iterate and improve** based on results
- ✅ **Cite AI assistance** appropriately in academic work

**Don't:**

- ❌ **Accept first outputs** without refinement
- ❌ **Use AI for final decisions** without human judgment
- ❌ **Skip verification** of facts and figures
- ❌ **Plagiarise or misrepresent** AI-generated content
- ❌ **Ignore institutional** AI policies

# Ethical Guidelines & Academic Integrity

**Using AI Responsibly in Research**

**Required Citation Example:**

> "Research methodology development was assisted by Microsoft Copilot (Microsoft Corporation, 2024). All generated hypotheses and experimental designs were subsequently validated against peer-reviewed literature and refined through expert consultation."

**What to Always Cite:**

- ✅ Hypothesis generation assistance
- ✅ Experimental design suggestions  
- ✅ Data analysis approaches
- ✅ Writing structure and organisation

**Institution-specific guidelines:** Always check your university's AI policy - requirements may vary!

# Next Steps & Advanced Applications

**Your Research Journey Continues**

**Immediate Actions:**

1. **Finish your prompt library** with today's successful templates
2. **Apply the workflow** to a real research question this week
3. **Experiment with CRAFT variations** for different purposes
4. **Document what works** and what doesn't

**Advanced Applications:**

- Multi-study research planning
- Grant proposal development
- Conference presentation creation
- Peer review simulation
- Research collaboration planning

**Community Building:** Consider forming study groups to share AI research techniques and improve workflows together

# Troubleshooting & Support

**When Things Don't Work**

**Common Issues & Solutions:**

| Issue | Quick Fix | Long-term Solution |
|-------|-----------|-------------------|
| Generic responses | Add "Be specific with examples" | Develop more detailed CRAFT prompts |
| Forgets context | Start new chat session | Use structured conversation management |
| Wrong methodology | Cross-check with known methods | Build domain expertise verification |
| Can't upload data | Try different browser/platform | Have multiple platform accounts |

**Remember:** Technology fails sometimes. The workflow principles remain valuable even when specific tools don't cooperate!

**Measuring Your Progress**

**By the end of today, you should be able to:**
- ✅ Use CRAFT framework to write effective research prompts
- ✅ Apply the 3-step workflow to any research topic
- ✅ Critically evaluate AI-generated research suggestions
- ✅ Build and maintain your personal prompt library
- ✅ Integrate AI tools with traditional research methods

**Self-Assessment Questions:**
1. Can you explain CRAFT to a colleague?
2. Do you feel confident starting a research project with AI assistance?
3. Can you identify when AI outputs need human verification?
4. Would you recommend this approach to other researchers?

**Success indicator:** You're excited to apply this to your own research, not overwhelmed by the complexity!

# Thank You!

**You're Now AI-Empowered Researchers!**

## Remember: Amplification, Not Replacement
You're not replacing your scientific expertise—you're amplifying it with powerful AI tools that handle routine tasks so you can focus on creative thinking and critical analysis.

**The Journey Continues:**
- **Today:** You learned structured workflows and CRAFT framework
- **Tomorrow:** You apply them to real research challenges  
- **Next month:** You're mentoring others in AI-assisted research
- **Next year:** You're publishing papers that showcase human-AI collaboration

**Created with assistance from Claude (Anthropic)** - *demonstrating responsible AI collaboration*

**Happy Researching!** 🚀

**All course materials, including presentations, datasets, interactive tools, and resources, available at:** [GitHub Pages URL]
