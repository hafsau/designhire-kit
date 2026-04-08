# Cover Letter Generator

Generate a portfolio-aware cover letter that sounds human and references your actual work.

## Usage

```
/cover-letter
```

Then paste the job description when prompted.

## What It Does

1. Reads your resume from `context/resume.md`
2. Reads your portfolio case studies from `context/portfolio.md`
3. Reads your writing style preferences from `context/writing-style.md`
4. Analyzes the job description you provide
5. Generates a 3-4 paragraph cover letter that:
   - Opens with something specific about why this role interests you
   - Connects your portfolio work to their needs
   - References specific metrics from your experience
   - Sounds like a confident designer, not a generic applicant
   - Ends with a clear call to action (not "I look forward to hearing from you")

## Instructions for Claude

When the user runs `/cover-letter`:

1. First, read the user's context files:
   - `context/resume.md` for their background
   - `context/portfolio.md` for case studies and metrics
   - `context/writing-style.md` for tone preferences

2. **Check if context files are filled in.** If they contain placeholder text like "[Your Name]" or template instructions, ask the user to either:
   - Fill in the context files first, OR
   - Provide quick info now: name, current role, 1-2 relevant projects with metrics, preferred tone

3. Ask the user to paste the job description.

4. Analyze the job description for:
   - Company name and what they do
   - Key responsibilities and requirements
   - Design challenges they face
   - Skills they're looking for

5. Match the user's experience to the job:
   - Which case studies are most relevant?
   - What metrics demonstrate relevant skills?
   - What unique angle can they bring?

6. Generate a cover letter following these rules:

**Structure:**
- Opening (1 paragraph): Why this specific role/company excites you. Be specific — mention their product, recent work, or mission. Don't be generic.
- Middle (1-2 paragraphs): Connect your portfolio work to their needs. Reference specific case studies by name. Use metrics.
- Closing (1 paragraph): Clear call to action. Not "I look forward to hearing from you" — something specific like "I'd love to walk you through how I approached the MedRec redesign" or "Let's chat about how I could help [specific challenge]."

**Tone Rules (from CLAUDE.md humanizer):**
- No "I am writing to express my interest"
- No "esteemed organization" or similar inflated language
- No em-dash overuse
- No "leverage," "synergy," "robust," or other AI-giveaway words
- Use first person naturally
- Vary sentence length
- Have opinions and personality

**Length:** 250-400 words. Hiring managers skim — be concise.

7. Output the cover letter in a clean format, ready to copy.

## Example Output

```
Hi [Hiring Manager],

I saw the Product Designer role at Acme and got excited — you're building exactly the kind of complex B2B tool I love working on. The way you've approached data visualization in your recent dashboard update reminded me of the challenges I tackled at [Company].

My most relevant work is MedRec, a diabetes management app I designed for Kaiser. The existing interface had a 40% error rate in medication logging because users were overwhelmed by options. I redesigned the core workflow using progressive disclosure and reduced errors by 35%. That experience with healthcare compliance and error-reduction feels directly applicable to [specific thing from their JD].

I also built [Portfolio Company]'s design system from scratch, going from inconsistent components to a unified library that cut design-to-dev time by 50%. I know you're scaling your design team, and I've been through that process.

I'd love to walk you through my MedRec case study and discuss how I could help [specific challenge]. What does your calendar look like next week?

Best,
[Name]
```

## Notes

- Always reference at least one case study by name
- Always include at least one metric
- Match the formality level to the company (startup vs enterprise)
- If they mention specific technologies or methods, connect to your experience with them
