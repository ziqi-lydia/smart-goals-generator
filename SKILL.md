# smart-goals-generator

Write SMART goals from vague intentions, generate goal-setting worksheets, create tracking spreadsheets with progress milestones, and set up automated check-in reminders. Supports personal goals, professional development, fitness, nursing, academic, and business contexts.

## When to Use

Use when the user wants to:
- Turn a vague goal into a SMART goal (Specific, Measurable, Achievable, Relevant, Time-bound)
- Generate SMART goal examples for a specific context (nursing, fitness, career, business, academic)
- Create a SMART goals worksheet or template
- Build a goal tracking spreadsheet with milestones
- Set up recurring check-in reminders for goal progress
- Write performance review goals in SMART format

## Inputs Required

Ask the user for:
1. **Goal or intention** 鈥� can be vague (e.g. "get healthier", "grow my business", "improve at work")
2. **Context** (optional): personal, professional, fitness, nursing/healthcare, academic, business/startup
3. **Timeframe** (optional, default: 90 days / one quarter)
4. **Number of goals** (optional, default: 3-5)
5. **Output format**: 
   - Text summary (default)
   - Google Sheet worksheet with tracking
   - Both

## SMART Framework Reference

Every goal must pass all 5 criteria:

- **S 鈥� Specific**: WHO is doing WHAT, WHERE, and WHY? No ambiguity.
- **M 鈥� Measurable**: What NUMBER or metric proves it is done? Include baseline + target.
- **A 鈥� Achievable**: Is this realistic given current resources, skills, and constraints?
- **R 鈥� Relevant**: Does this connect to a bigger objective or value?
- **T 鈥� Time-bound**: What is the DEADLINE? Include milestones.

### Common Mistakes to Avoid
- "Improve customer satisfaction" 鈫� Not measurable. Fix: "Increase NPS score from 32 to 45 by Q3 2026"
- "Exercise more" 鈫� Not specific or measurable. Fix: "Run 3x/week for 30 minutes, completing 36 sessions by June 30"
- "Learn Spanish" 鈫� Not time-bound or measurable. Fix: "Complete Duolingo Spanish B1 course and hold a 15-minute conversation with a native speaker by September 1"

## Workflow Steps

### Step 1: Expand Vague Goals into SMART Format

For each goal the user provides:

1. **Clarify the intention** 鈥� restate what they actually want to achieve
2. **Add specificity** 鈥� define the exact action, scope, and context
3. **Define the metric** 鈥� choose a number, percentage, or binary milestone
4. **Reality-check** 鈥� flag if the goal seems unrealistic and suggest an adjusted version
5. **Connect to relevance** 鈥� explain WHY this goal matters in their context
6. **Set deadline + milestones** 鈥� break into weekly or monthly checkpoints

**Output format for each goal:**
```
GOAL: [One-sentence SMART goal]

S 鈥� Specific: [What exactly will be done, by whom, in what context]
M 鈥� Measurable: [Baseline 鈫� Target metric, how it will be tracked]
A 鈥� Achievable: [Why this is realistic, what resources/support are needed]
R 鈥� Relevant: [How this connects to the bigger picture]
T 鈥� Time-bound: [Deadline + milestone dates]

MILESTONES:
- Week 2: [checkpoint]
- Week 4: [checkpoint]
- Week 8: [checkpoint]
- Week 12: [final target]

TRACKING METHOD: [How to measure progress 鈥� app, spreadsheet, manual check-in]
```

### Step 2: Generate Context-Specific Examples

When user asks for examples, provide 5 fully written SMART goals for their context:

**Nursing / Healthcare Examples:**
1. "Reduce medication administration errors on my unit from 4/month to 0/month within 90 days by implementing a double-check verification protocol before each administration"
2. "Complete 24 CEU credits in critical care nursing by December 31, 2026, averaging 2 credits per month through online courses on AACN website"
3. "Improve patient satisfaction scores in post-op recovery from 78% to 90% within 6 months by implementing hourly comfort rounding and documenting pain reassessment within 30 minutes of intervention"

**Fitness Examples:**
1. "Run a sub-25-minute 5K by August 15, 2026, starting from current time of 32 minutes, by following a 3-day/week interval training program"
2. "Increase bench press from 135 lbs to 185 lbs within 16 weeks by following a progressive overload program with 5 lb increases every 2 weeks"
3. "Lose 15 pounds (from 195 to 180) by July 1, 2026, by maintaining a 500-calorie daily deficit tracked in MyFitnessPal and exercising 4x/week"

**Professional / Career Examples:**
1. "Earn AWS Solutions Architect certification by June 30, 2026, by completing 2 study modules per week on A Cloud Guru and passing 3 practice exams with 85%+ scores"
2. "Increase team's sprint velocity from 34 to 45 story points within 2 quarters by reducing scope creep through stricter acceptance criteria and limiting mid-sprint additions to emergencies only"
3. "Publish 12 LinkedIn articles on AI in supply chain management (1/month) by December 2026, each generating 50+ engagements, to establish thought leadership for a senior director promotion"

**Business / Startup Examples:**
1. "Increase MRR from $8,000 to $15,000 within 6 months by launching a mid-tier pricing plan, improving trial-to-paid conversion from 8% to 14%, and reducing monthly churn from 5% to 3%"
2. "Acquire 500 new email subscribers per month (up from 120) by publishing 3 SEO blog posts per week and launching a lead magnet by April 30"

**Academic Examples:**
1. "Raise cumulative GPA from 3.2 to 3.5 by end of Spring 2027 semester by attending all office hours, completing assignments 48 hours before deadlines, and forming a study group that meets twice weekly"

### Step 3: Create Google Sheet Worksheet

If user wants a tracking spreadsheet, create a Google Sheet with:

**Sheet 1: "SMART Goals Worksheet"**
- Column A: Goal # (1, 2, 3...)
- Column B: Goal Statement (the full SMART goal)
- Column C: Specific 鈥� What & Who
- Column D: Measurable 鈥� Baseline 鈫� Target
- Column E: Achievable 鈥� Resources Needed
- Column F: Relevant 鈥� Why It Matters
- Column G: Time-bound 鈥� Deadline
- Column H: Current Status (Not Started / In Progress / On Track / Behind / Completed)
- Column I: % Complete
- Column J: Notes

Format: Freeze row 1, alternating row colors, column widths adjusted for readability

**Sheet 2: "Progress Tracker"**
- Column A: Goal #
- Column B: Goal (short name)
- Column C: Week 1 progress
- Column D: Week 2 progress
- ... through Week 12 (or however long the timeframe)
- Final column: Target Achieved? (Yes/No)

Color-code progress cells:
- Green: on track or ahead
- Yellow: slightly behind
- Red: significantly behind
- Gray: not yet started

**Sheet 3: "Milestones"**
- Column A: Goal #
- Column B: Milestone Description
- Column C: Target Date
- Column D: Actual Date
- Column E: Status (Pending / Completed / Missed)
- Column F: Notes

### Step 4: Set Up Check-in Reminders (Optional)

If user wants automated check-ins:
- Suggest a weekly or bi-weekly workflow
- The workflow reads the Progress Tracker sheet
- Checks which goals are behind schedule
- Sends a summary message: "Goal Progress Check-in 鈥� 2 of 5 goals are on track, 1 is behind schedule on [metric]"

## Quality Standards

- Every SMART goal must pass ALL 5 criteria 鈥� reject any that fail even one
- Include specific numbers in EVERY goal 鈥� no vague language
- Milestones must be evenly distributed across the timeline, not all at the end
- Examples must feel realistic for the context 鈥� nursing goals should use actual clinical terminology, fitness goals should use real exercise metrics
- Worksheets must be ready to use immediately 鈥� pre-formatted, with example data that can be overwritten
- Always provide at least 3 milestones per goal
