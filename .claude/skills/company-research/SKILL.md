# Company Research

Research a company's design work, culture, and what they're looking for in designers.

## Usage

```
/company-research
```

Then provide the company name and (optionally) the role you're applying for.

## What It Does

1. Researches the company's design presence
2. Analyzes their design system, recent work, and team structure
3. Identifies talking points for interviews and applications
4. Surfaces information that helps you tailor your pitch
5. **Goes beyond surface-level research** to find what average candidates miss

## What Top Candidates Research (That Average Candidates Miss)

Average candidates: Read website, check job description, skim Glassdoor.

Top candidates:
- Analyze tech stack and design infrastructure
- Study actual interview questions asked at that company
- Track product evolution using Wayback Machine
- Map the design team's backgrounds and specializations
- Verify design culture with public evidence

## Instructions for Claude

When the user runs `/company-research`:

1. Ask for:
   - Company name
   - Role they're applying for (optional)
   - Any specific aspects they want to research

2. Research and compile information on:

### Design Team & Culture
- Design team size and structure (if available)
- Design leadership (who leads design, their background)
- Design principles or values they've published
- How they talk about design in blog posts, talks, or podcasts
- Remote vs in-office culture

### Design Work
- Their main product(s) and design challenges
- Public design system (if they have one)
- Recent design updates or redesigns
- Design blog posts or case studies they've published
- Conference talks by their designers

### Technology & Tools
- Design tools they use (often in job descriptions)
- Tech stack (helps understand design-dev collaboration)
- Engineering blog posts about design collaboration

### What They Value
- Based on job description language
- Based on their design blog/talks
- Based on interview reports (Glassdoor, Blind)

### Talking Points
- Specific things to reference in cover letter/interview
- Questions to ask them
- Potential concerns or red flags

### Advanced Research (What Sets Top Candidates Apart)

**Design System Maturity:**
- Check if they have a public design system (Figma Community, GitHub, Storybook)
- Analyze: component coverage, documentation quality, update frequency
- Low docs + old components = chaos. High docs + recent updates = mature team

**Product Evolution Analysis:**
- Use Wayback Machine to see how product/website evolved over 2-3 years
- Track design changes, feature additions, messaging shifts
- Reveals strategic pivots, priorities, what succeeded vs failed

**Interview Question Research:**
- Search Glassdoor/Blind for "[Company] design interview questions"
- Find actual questions asked, not generic advice
- Prepare specific answers for their specific questions

**Team Mapping via LinkedIn:**
- Filter by "Design" roles at the company
- Note: previous companies, specializations, tenure length
- High turnover (short tenures) = red flag. Long tenures = stable culture
- Look for design reporting structure (to Product, Design Lead, or CEO)

**Competitive UX Analysis:**
- Compare their product against 2-3 main competitors
- Identify specific UI/UX gaps you could discuss in interviews
- Example: "I noticed your onboarding is 5 steps while [competitor] is 2"

3. Output a structured research brief.

## Example Output

```
# Figma — Design Research Brief

## Design Team
- ~150 designers (as of 2024)
- Led by Noah Levin (VP Design)
- Notable designers: Joey Banks (Design Systems), Luis Ouriach (Advocacy)
- Known for: designer-developer collaboration, dogfooding their own product

## Design Work
- Primary: Figma design tool, FigJam, Dev Mode
- Recent: Variable fonts, Auto Layout 5, AI features (Make Design)
- Design System: Internal, heavily documented, influences the product itself

## What They Value
- From job posts: "Systems thinking," "shipping fast," "design engineering"
- From talks: Accessibility, performance, cross-functional collaboration
- Culture: Strong writing culture, design crits, low ego

## Talking Points for Your Application
- Reference their recent Auto Layout update (complexity handling)
- Connect your healthcare work to their accessibility focus
- Mention their design system work if you have DS experience

## Questions to Ask
- "How does the design team influence product roadmap?"
- "What's the balance between new features vs polish?"
- "How do you handle design debt?"

## Red Flags to Watch
- Fast growth = potentially unclear processes
- AI features = might deprioritize core product
- Check: work-life balance reviews on Glassdoor
```

## Reading Glassdoor/Blind Like a Pro

**Don't just look at ratings.** Instead:

- Search specifically for "design" in recent reviews (last 3 months)
- Look for patterns — 5+ people mentioning same issue = real problem
- Verify claims with corroborating evidence (blog posts, conference talks)
- Check for management stability (3+ design directors in 2 years = red flag)

**Cross-reference compensation:**
- Use Levels.fyi, PayScale, and LinkedIn salary data together
- Equity is 25-40% of total comp for senior roles — ask about vesting

**Spot the difference:**
- What they SAY (careers page) vs what people EXPERIENCE (reviews)
- Marketing culture vs real culture

## Develop Interview Insights

Come prepared with 2-3 specific observations:

**Instead of:** "I love your product"
**Say:** "I noticed your 2023 redesign removed [feature] but reviews show users miss it. Have you considered [alternative approach]?"

**Instead of:** "What's your design process?"
**Say:** "Based on your recent funding round and hiring 5 new designers, I assume you're scaling to new markets. What design challenges does that create?"

## Notes

- Use web search to find current information
- Prioritize their own content (blog, talks) over third-party articles
- Look for signals of design maturity (system, process, leadership)
- Note any recent layoffs or restructuring that might affect the team
- Include both positive signals and potential concerns
- **Research converts to interview talking points** — always prepare 2-3 specific insights

## If Web Search Unavailable

If you cannot access web search, ask the user to provide:
- Company website URL
- Links to their design blog, engineering blog, or careers page
- Any job description they have

Then analyze what's available and note which sections need more research.
