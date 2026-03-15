# Research Writing Skill

A Claude Code skill for producing informed, measured, evidence-driven long-form prose that reads as thoughtful and credible rather than promotional or AI-generated.

## Overview

This skill helps you write blog posts, research summaries, product announcements, technical narratives, industry analyses, white papers, thought leadership pieces, and any long-form content that should feel researched, authoritative, and human.

The skill follows a proven three-phase workflow and incorporates the [humanizer skill](https://github.com/blader/humanizer/) to eliminate AI writing patterns and ensure natural, human-like prose.

## Installation

1. Copy `SKILL.md` to your Claude Code skills directory (`~/.claude/skills/research-writing/`)
2. The skill will be automatically available in Claude Code

## How to Use

### Trigger Phrases

The skill automatically activates when you use phrases like:
- "write a blog post"
- "draft an announcement"
- "research-style writing"
- "make this sound informed"
- "write this like a real person"
- "thoughtful," "measured," or "credible" writing requests

### Basic Usage

Simply provide a topic or brief and the skill will guide you through the process:

```
/research-writing "Write a blog post about our new API features"
```

Or just ask naturally:
```
"Can you help me write a research summary about machine learning performance improvements?"
```

## The Three-Phase Workflow

### Phase 1: Interview
The skill conducts a structured interview to gather crucial context:
- **Audience and intent**: Who is this for? What should they take away?
- **Evidence and specifics**: What data, benchmarks, quotes, or examples are available?
- **Structure and constraints**: What article type fits? Any length or style requirements?
- **Edge cases and tradeoffs**: What tensions or limitations should be addressed?

### Phase 2: Draft
Creates the full draft following proven principles:
- Evidence-backed claims with specific numbers and comparisons
- Clear article structure (announcement, research report, narrative, or industry piece)
- Professional but not corporate tone
- Technical accuracy with accessible explanations

### Phase 3: Humanizer Pass
Automatically invokes the [humanizer skill](https://github.com/blader/humanizer/) to eliminate AI writing patterns:
- Removes significance inflation ("revolutionary," "game-changing")
- Fixes synonym cycling and elegant variation
- Eliminates promotional language and filler phrases
- Corrects structural tells and AI vocabulary patterns

## Input Examples

### Example 1: Product Announcement Brief

```
**Brief**: "We're launching a new code review feature that uses AI to catch bugs automatically. It reduced review time by 40% in our internal testing and found 23% more critical issues than human reviewers alone."

**Additional Context**:
- Target audience: Software engineering teams
- Key differentiator: Runs in real-time during development
- Available data: 6-month internal trial with 50 developers
- Publication: Company blog and developer newsletter
```

**The skill will interview to gather**:
- Specific benchmark comparisons
- User quotes from the trial
- Technical implementation details
- Pricing and availability information
- Limitations or caveats to mention

### Example 2: Research Summary Brief

```
**Brief**: "Write a research summary about our study on remote work productivity. We surveyed 1,200 knowledge workers across 6 months and found mixed results depending on job type and experience level."

**Additional Context**:
- Target audience: HR leaders and business executives
- Key finding: Productivity varied significantly by role
- Available data: Survey responses, productivity metrics, interview transcripts
- Length: 2,500-3,000 words
```

**The skill will interview to gather**:
- Specific productivity metrics and statistical significance
- Methodology details for credibility
- Demographic breakdown of survey participants
- Conflicting or surprising findings to address
- Implications for policy recommendations

### Example 3: Technical Narrative Brief

```
**Brief**: "Tell the story of how our engineering team solved the database scaling problem that was causing outages. We went from 12 outages per month to zero over 4 months."

**Additional Context**:
- Target audience: Technical leadership and engineering teams
- Story arc: Problem identification → Solution exploration → Implementation → Results
- Available sources: Engineering team interviews, incident reports, performance data
```

**The skill will interview to gather**:
- Technical details about the scaling solution
- Specific timeline and milestones
- Team member quotes about challenges faced
- Quantitative improvements beyond outage reduction
- Lessons learned for other engineering teams

## Article Type Examples

### Product Announcements
- Open with clear, concise framing
- Present capabilities with specific numbers
- Include benchmark comparisons
- Feature customer validation quotes
- End with availability details

### Research Reports
- Frame with clear research questions
- Explain methodology accessibly
- Present findings with appropriate precision
- Acknowledge limitations and caveats
- Connect to broader implications

### Technical Narratives
- Start with concrete problem context
- Build from specific to general insights
- Use detailed examples to illustrate concepts
- Include team perspectives and quotes
- Extract practical lessons for readers

### Industry Analyses
- Frame around real practitioner problems
- Demonstrate concrete use cases
- Include specific partner outcomes
- Avoid generic industry predictions
- Focus on actionable insights

## Key Writing Principles

### Evidence Over Assertion
❌ "The system shows major improvements"
✅ "The new model scores 76% on the 8-needle retrieval benchmark, compared to 18.5% for the previous version"

### Technical Terms in Context
❌ "The Gini coefficient fell. (Note: The Gini coefficient measures inequality.)"
✅ "The Gini coefficient, a standard measure of equality, fell from 0.37 to 0.32"

### Intellectual Honesty
❌ "Our solution completely eliminates the problem"
✅ "The system reduces false positives by 60%, though it still lags behind human experts in edge cases"

## What Gets Avoided

The skill actively eliminates common AI writing patterns:
- **Hype inflation**: "revolutionary," "game-changing," "unprecedented"
- **Generic conclusions**: "The future looks bright," "exciting times ahead"
- **AI vocabulary**: "delve," "leverage," "landscape" (abstract usage)
- **Promotional language**: "boasts," "showcasing," "vibrant"
- **Structural tells**: Excessive bullet points with inline headers
- **Synonym cycling**: Artificially rotating between "system," "platform," "solution"

## Attribution

This skill incorporates and automatically invokes the [humanizer skill](https://github.com/blader/humanizer/) created by [@blader](https://github.com/blader). The humanizer performs the final pass to eliminate AI writing patterns and ensure natural, human-like prose.

The research-writing methodology is based on analysis of effective technical and scientific communication across academic, industry, and journalistic contexts.

## Example Output Quality

**Before**: "Our groundbreaking new platform leverages cutting-edge AI to revolutionize the development landscape, offering unprecedented capabilities that will transform how teams collaborate."

**After**: "The new code review tool catches 23% more critical bugs than manual reviews alone. In our six-month trial with 50 developers, it reduced review cycles from an average of 2.3 days to 1.4 days while maintaining code quality standards."

## License

MIT License - See [LICENSE](LICENSE) file for details.

## Contributing

Contributions welcome! Please:
1. Test changes with diverse writing briefs
2. Ensure the three-phase workflow remains intact
3. Maintain attribution to the humanizer skill
4. Include examples of before/after output quality

## Support

For issues or questions:
- Open an issue in this repository
- Reference specific examples of unexpected behavior
- Include the input brief and desired output type