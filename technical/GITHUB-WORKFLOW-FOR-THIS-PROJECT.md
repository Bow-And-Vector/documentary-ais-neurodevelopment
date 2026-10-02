# GitHub Workflow for This Documentary Project

## What is GitHub and why we're using it

GitHub is a platform for version control and collaboration. Think of it as:
- A shared folder that tracks every change
- A way for multiple people (or AI agents) to work on the same project
- A record of what was changed, when, and why
- A backup system so nothing is ever lost

For this documentary, GitHub is where we store:
- Scripts and production notes
- Research and sources
- Interview guides
- Production timelines
- Visual storyboards
- Links to video files and assets

---

## Basic GitHub concepts you need to know

### Repository ("repo")
A repository is a folder that contains all your project files. You already have one:
- **Owner:** Bow-And-Vector (you)
- **Repo name:** documentary-ais-neurodevelopment
- **URL:** https://github.com/Bow-And-Vector/documentary-ais-neurodevelopment

This is your project's home.

### Branches
A branch is a separate version of your project. Think of it like:
- Main branch = the "official" version
- Other branches = experimental versions where you work on new things

For this project:
- **main** = final, approved versions of scripts and plans
- **production** = working drafts, edits in progress
- **research** = source material and reference documents

You can switch between branches without affecting the main version.

### Commits
A commit is a snapshot of your changes. Every time we add or update a file, we create a commit with a message explaining what changed.

Example commit message:
"Add 3-minute testimony script with visual cues"

This creates a permanent record of when and why something changed.

### Files and Folders
Your repo is organized by folder:
```
documentary-ais-neurodevelopment/
├── research/
│   ├── interview-protocol-and-fact-matrix.md
│   ├── sources.md
│   └── neuroscience-evidence.md
├── production/
│   ├── URGENT-october-sprint.md
│   ├── YOUR-TESTIMONY-SCRIPT.md
│   ├── EXPERT-INTERVIEW-GUIDE.md
│   ├── PRODUCTION-BIBLE-FINAL.md
│   └── shot-lists/
├── script/
│   ├── outreach-packet.md
│   └── dialogue-and-voiceover.md
├── assets/
│   ├── video-files/
│   ├── audio-files/
│   ├── graphics/
│   └── b-roll-notes/
├── distribution/
│   ├── social-media-captions.md
│   ├── email-templates.md
│   └── platforms-and-timing.md
└── README.md
```

---

## How to use GitHub with me (Copilot)

### Workflow 1: I create/update a file and push it to your repo

**What happens:**
1. You ask me to create or update a document
2. I write it
3. I push it directly to your GitHub repo
4. You see it appear in your repo on GitHub.com
5. You can download it, edit it locally, or view it in the browser

**Example:**
- You: "Create a shot list for the testimony video"
- Me: [I write the shot list and push it to production/shot-lists/testimony-shot-list.md]
- You: [You go to GitHub and see the new file]

### Workflow 2: You work on something locally and want to sync it back

**What happens:**
1. You download a file from your repo
2. You edit it on your computer
3. You want to save those changes back to GitHub
4. You use Git commands (or GitHub Desktop) to upload your changes
5. I can then see your changes and build on them

**How to do this (easy version):**
- Install GitHub Desktop (https://desktop.github.com/)
- Log in with your account
- Open your repo
- Make changes to files
- GitHub Desktop will show what changed
- Click "Commit" and add a message
- Click "Push" to send it to GitHub.com

**How to do this (command line version):**
```bash
# Clone the repo (download it for the first time)
git clone https://github.com/Bow-And-Vector/documentary-ais-neurodevelopment.git

# Navigate into the folder
cd documentary-ais-neurodevelopment

# Make changes to files in your editor

# Check what changed
git status

# Stage your changes
git add .

# Commit with a message
git commit -m "Update testimony script with new section on parents"

# Push to GitHub
git push origin main
```

### Workflow 3: Collaboration pattern for this project

**Weekly cycle:**

1. **Monday morning:** I create the week's production plans and push them to production/
2. **Monday-Wednesday:** You film, record, and collect materials
3. **Wednesday:** You upload your raw footage notes to assets/video-files/
4. **Wednesday-Thursday:** I review, create editing guides, update timelines
5. **Thursday-Friday:** You edit or coordinate editing
6. **Friday:** Final version pushed to main with release notes

---

## How to view and navigate your repo

### On GitHub.com (in your browser)

1. Go to https://github.com/Bow-And-Vector/documentary-ais-neurodevelopment
2. You'll see the file structure
3. Click any file to view it
4. Click the folder to navigate
5. Use the search box to find files by name

### Downloading files

1. Click on a file
2. Click the download icon (down arrow) in the top right
3. File downloads to your computer

### Viewing the history

1. Click on a file
2. Click "History" to see all changes made to that file
3. Click any commit to see exactly what changed and when

---

## How to ask me to find open-source tools and integrate them

### When you want to find tools for animation, 3D, video editing, etc.

**What to ask me:**
```
"Find open-source tools for [task]. I need [specific requirement]. 
Integrate them into a workflow that works with DaVinci Resolve."
```

**Examples:**
- "Find open-source tools for creating scientific animations of prenatal development. I need something that can show hormone pathways and receptor signaling clearly. Can you create a workflow document?"
- "Find open-source tools for Gaussian splatting and 3D avatar creation. I want to create a VR scene with me and you in it. What's the fastest workflow?"
- "Find open-source tools for creating infographics and data visualizations about SB 14 and Texas policy. I need something that produces clean, political graphics."

### What I'll do:

1. Search for relevant open-source repos on GitHub
2. Create a document that lists:
   - Tool name and GitHub link
   - What it does
   - System requirements
   - How to install it
   - How to use it for your specific need
   - Example output
3. Push a comprehensive guide to your repo
4. Walk you through the workflow

### Common open-source tools we might use:

**For animations:**
- Blender (3D modeling and animation)
- Manim (mathematical animations)
- Pencil2D (2D animation)
- Krita (digital painting and animation)

**For 3D and VR:**
- Blender (3D modeling)
- Godot Engine (3D/2D game engine, can do VR)
- Three.js (web-based 3D)
- COLMAP + Gaussian Splatting (for photogrammetry)

**For video editing:**
- You already have DaVinci Resolve (excellent)
- FFmpeg (command-line video processing)
- OpenShot (video editor)
- Kdenlive (video editor)

**For graphics and infographics:**
- Inkscape (vector graphics)
- GIMP (image editing)
- Graphviz (diagram creation)
- Gnuplot (data visualization)

**For audio:**
- Audacity (audio editing)
- FFmpeg (audio processing)
- SoX (sound exchange)

**For project management:**
- GitHub Projects (built into GitHub)
- Trello (free, integrates with GitHub)

---

## Organizing your GitHub for maximum efficiency

### Folder structure we recommend:

```
documentary-ais-neurodevelopment/
├── README.md (project overview and quick start)
├── production/
│   ├── PRODUCTION-BIBLE-FINAL.md (master production document)
│   ├── URGENT-october-sprint.md (timeline)
│   ├── YOUR-TESTIMONY-SCRIPT.md
│   ├── EXPERT-INTERVIEW-GUIDE.md
│   ├── shot-lists/
│   │   ├── testimony-shot-list.md
│   │   ├── expert-interview-setup.md
│   │   ├── b-roll-shots.md
│   │   └── animation-requirements.md
│   └── editing-guides/
│       ├── dci-resolve-workflow.md
│       └── color-grade-and-sound.md
├── research/
│   ├── sources.md (all scientific sources, links, citations)
│   ├── interview-protocol-and-fact-matrix.md
│   ├── neuroscience-evidence.md
│   └── policy-research/
│       ├── sb-14-text.md
│       ├── ken-paxton-timeline.md
│       └── texas-policy-overview.md
├── script/
│   ├── outreach-packet.md
│   ├── dialogue-and-voiceover.md
│   └── testimonies/
│       ├── your-testimony-3min.md
│       ├── your-testimony-60sec.md
│       └── expert-soundbites.md
├── technical/
│   ├── GITHUB-WORKFLOW-FOR-THIS-PROJECT.md (this file)
│   ├── open-source-tools-guide.md
│   ├── gaussian-splatting-workflow.md
│   ├── animation-creation-guide.md
│   └── vr-environment-setup.md
├── assets/
│   ├── VIDEO-FILES.md (index of all video, with links and notes)
│   ├── AUDIO-FILES.md (index of all audio)
│   ├── GRAPHICS.md (index of all graphics and animations)
│   └── B-ROLL-NOTES.md (descriptions and locations of b-roll)
└── distribution/
    ├── social-media-captions.md
    ├── email-templates.md
    ├── press-release.md
    └── platforms-and-timing.md
```

### Key documents to maintain:

1. **README.md** — Project overview, quick start, links to key documents
2. **production/PRODUCTION-BIBLE-FINAL.md** — Master document, updated weekly
3. **assets/VIDEO-FILES.md** — Index of all video assets with notes
4. **distribution/platforms-and-timing.md** — Release schedule and where to post

---

## How to use GitHub Projects for tracking progress

### Set up a project board:

1. Go to your repo
2. Click "Projects" tab
3. Click "New project"
4. Choose "Table" view
5. Create columns:
   - **Backlog** (things to do)
   - **In Progress** (actively working)
   - **Review** (ready for feedback)
   - **Done** (finished)

### Track tasks:

- Create a task for each piece of production:
  - "Film testimony video"
  - "Email expert contacts"
  - "Create animation of prenatal development"
  - "Edit 3-minute short"
  - "Upload to YouTube"

### Link to issues:

- Each task can link to a GitHub Issue
- Issues can have due dates, labels, assignments
- This keeps everything visible and trackable

---

## Quick reference: Common GitHub tasks

### I need to ask Copilot to do something

**Format:**
"In the documentary-ais-neurodevelopment repo, [task]. Push it to [folder] as [filename.md]."

**Examples:**
- "Create a shot list for the Gaussian splat sequence. Push it to production/shot-lists/ as gaussian-splat-shot-list.md."
- "Find open-source tools for prenatal development animation. Create a workflow guide and push it to technical/ as animation-creation-guide.md."
- "Review the testimony script and create a cinematography guide. Push it to production/shot-lists/ as testimony-cinematography-guide.md."

### I want to see what's in a folder

1. Go to GitHub.com
2. Navigate to the folder
3. All files are listed
4. Click any file to view

### I want to download everything

1. Go to your repo
2. Click the green "Code" button
3. Click "Download ZIP"
4. Unzip on your computer
5. You now have the full project locally

### I want to track changes over time

1. Click any file
2. Click "History"
3. See all commits with that file
4. Click any commit to see what changed

---

## Best practices for this project

1. **Commit messages should be clear and specific**
   - Good: "Add 3-minute testimony script with visual cues for filming"
   - Bad: "update stuff"

2. **Keep files organized by function**
   - Production files in production/
   - Research files in research/
   - Technical guides in technical/
   - Assets indexed in assets/

3. **Update your index files weekly**
   - assets/VIDEO-FILES.md should list all video with notes
   - assets/AUDIO-FILES.md should list all audio
   - This makes finding things easy

4. **Use the README.md as your project dashboard**
   - Quick overview of current status
   - Links to key documents
   - Upcoming deadlines
   - Who to contact

5. **Document decisions**
   - When you decide something (aesthetic choice, technical approach, casting), add it to a document
   - Why did you choose that approach?
   - This helps you stay consistent and remember your reasoning

---

## Summary

**GitHub is your project management system. It:**
- Stores all your scripts, plans, and notes
- Tracks changes over time
- Backs up your work
- Allows me to push files directly to you
- Allows you to sync changes back to me
- Keeps everything organized and searchable

**To use it effectively:**
- Ask me to create or update documents
- I push them to specific folders
- You download, edit, or view them
- You sync changes back when you're done
- We maintain a shared project that's always organized and up to date

This is how modern teams collaborate. And now you have a system that will scale as your project grows.
