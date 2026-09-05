# Flowstate — AI Workplace Productivity Assistant

An AI-powered productivity platform that helps knowledge workers manage tasks, meetings, research, and daily planning — all connected through an intelligent assistant that understands context and surfaces risks before they become problems.

## Features

### Dashboard
- Live clock with contextual greeting and current date
- Today's productivity overview with completion ring and status breakdown
- Priority task list with progress indicators and AI signals
- Upcoming events (meetings, deadlines, events)
- AI Intelligence panel with relevant insights, recommended actions, and quick navigation

### Meetings & Communication
- Capture meeting details: title, date, participants, notes/transcript, context, audience, tone
- AI-powered meeting analysis producing:
  - Meeting Summary
  - Key Points
  - Decisions
  - Action Items (with responsible party and deadline)
  - Items Requiring Clarification
- Follow-up email generation with edit, regenerate, copy, accept, and reject controls
- One-click "Add to Task Planner" for action items
- Review-before-sending policy — no automatic email sending

### Task Planner
- Today's progress with completion percentage and status counts (Completed, On Track, Needs Attention, At Risk)
- Task list with priority, deadline, duration, progress, status, and AI signals
- Visual daily timeline (08:00–18:00) with tasks mapped to time slots
- AI actions: Optimise My Day, Prioritise Tasks, Analyse Progress, Suggest Revised Schedule
- Task detail drawer with AI assessment, progress slider, and mark-complete functionality
- Demo scenario loader (Normal Day, Overloaded, Deadline Crisis, Blocked Task, Completed, Full Challenge)

### Research & Intelligence
- Search any question, topic, or paste article text
- AI-generated research brief with:
  - Executive Summary
  - Key Insights
  - Trends
  - Business Implications
  - Opportunities
  - Risks
  - Recommendations
  - Further Questions
- Create tasks from research findings
- Demo scenarios (Industry Trends, Business Opportunity, Emerging Technology, Complex Report)

### AI Assistant
- Conversational chat interface connected to your task data
- Context-aware responses that reference your actual tasks, deadlines, and progress
- Example prompts:
  - "What should I work on first?"
  - "Which tasks are at risk?"
  - "What do I need to accomplish today?"
  - "What trends should I be watching?"
  - "I have two hours available — what should I work on?"
- Action buttons that navigate to relevant screens

### Responsible AI
- AI principles: AI assists, recommends, helps execute — humans review and decide
- Safeguards: review generated content, verify important information, regenerate, edit, reject
- Data and privacy considerations
- AI limitations documentation
- Verification requirements checklist

### Settings
- Working hours configuration
- Default tone and audience preferences
- Notification preferences (task alerts, meeting reminders, research updates)
- Productivity preferences (auto-prioritize)

## How Screens Connect

The screens are designed to demonstrate a complete workflow:

1. **Meeting → Tasks**: Analyze meeting notes → extract action items → add to Task Planner
2. **Meeting → Email**: Analyze meeting → generate follow-up email → review → copy
3. **Research → Tasks**: Research topic → identify recommendation → create task → appears in Task Planner
4. **Task Intelligence**: Task progress + deadline → AI risk assessment → recommendation → user decides
5. **Assistant → Any Screen**: Ask AI a question → get contextual answer → navigate to relevant screen

## Tech Stack

- **React 18** with TypeScript
- **Vite** for build tooling
- **Tailwind CSS** for styling
- **Lucide React** for icons
- **Supabase** for backend (database, auth, edge functions)

## Getting Started

```bash
# Install dependencies
npm install

# Start the dev server
npm run dev

# Build for production
npm run build

# Type check
npm run typecheck
```

## Project Structure

```
src/
├── components/        # Shared UI components (Sidebar, Header, badges, progress bars)
├── context/           # Global app state via React Context
├── data/              # Mock data and demo scenarios
├── lib/               # AI simulation logic
├── screens/           # Main application screens
│   ├── Dashboard.tsx
│   ├── Meetings.tsx
│   ├── TaskPlanner.tsx
│   ├── Research.tsx
│   ├── Assistant.tsx
│   ├── ResponsibleAI.tsx
│   └── Settings.tsx
├── types/             # TypeScript type definitions
├── App.tsx            # App shell with navigation
└── index.css          # Global styles and Tailwind config
```

## Design Principles

- **Human-in-the-loop**: AI suggests, humans decide. No automatic actions.
- **Context-aware**: The AI references real task data to provide meaningful recommendations.
- **Connected workflow**: Every screen links to others — meetings feed tasks, research creates tasks, the assistant navigates to tasks.
- **Professional aesthetic**: Clean, cohesive color system with teal accents, neutral ink tones, and restrained use of color for status indicators.
- **Collapsible sidebar**: Maximize screen space by collapsing the sidebar to icon-only mode.

## License

This project is part of the CAPACITI MVP demonstration.
