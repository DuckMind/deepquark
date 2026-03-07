# DeepQuark

**DeepQuark** is an agentic AI platform developed by **DuckMind Team** that shifts the paradigm from "getting answers" to **automatically executing real work**.

Instead of just chatting with AI, DeepQuark lets AI **access data, plan, and carry out multi-step tasks** — so you can delegate work and come back when it's done.

DeepQuark is designed as an **AI coworker** that runs on your machine, capable of handling complex tasks by breaking them down and executing them step by step until results are delivered.

## From Answers to Action

DeepQuark doesn't just answer questions — it **gets work done**.

You describe the goal. DeepQuark will:

1. Analyze the task
2. Break it into steps
3. Execute each step
4. Track progress
5. Deliver the final result

You can watch the process in real time or hand it off and come back later.

## How DeepQuark Works

DeepQuark uses an **agentic workflow** model:

1. Understand the user's goal
2. Decompose it into smaller steps
3. Plan the execution
4. Access the necessary data
5. Execute each step
6. Synthesize the final result

Along the way, DeepQuark can read files, analyze data, write code, generate reports, create slide decks, and synthesize information from multiple sources.

## Automate Recurring Work

DeepQuark is especially useful for time-consuming, repetitive tasks. You can configure tasks to run daily, weekly, or monthly.

Examples include compiling morning briefings, running periodic data analysis, aggregating customer feedback, and auto-generating dashboards or slide decks.

## Use Cases

### Administrative

Generate daily reports or briefings from multiple data sources such as Discord, WhatsApp, Slack, Notion, GitHub, email, and internal documents — helping you quickly identify what matters most.

### Research & Analysis

DeepQuark can handle complex analytical tasks: market research, data aggregation, calculations, and professional report generation. Results can be exported to PowerPoint, Excel, Markdown, or structured analysis reports.

### Sales & Product

Aggregate feedback from call transcripts, Slack, CRM, and issue trackers. Then identify recurring issues, customer needs, and new product ideas.

### Legal & Compliance

Process large document sets by organizing them chronologically, tagging content, assessing importance, and generating document catalogs — making legal review faster and more systematic.

## You Stay in Control

DeepQuark is built on the **human-in-the-loop** principle. AI assists, but humans make the decisions.

### Runs Locally on Your Machine

DeepQuark runs inside a **virtualized environment (VM)** on your machine. You decide which directories AI can access, which data it can read, and which connectors it's allowed to use. AI cannot access anything you haven't explicitly permitted.

### Confirmation Before Action

For critical actions, DeepQuark will show the execution plan, wait for your confirmation, and only proceed after you approve. You can adjust the plan, change the approach, or cancel at any time.

## Vision

DeepQuark is moving toward a model where AI acts as a true **coworker** — one that understands goals, organizes work, executes multi-step processes, and delivers finished products.

Instead of *asking AI for answers*, we're shifting to *delegating work to AI and receiving results*.

---

## Installation

DeepQuark requires **Node.js (latest)** and is installed via npm. Below are platform-specific instructions.

### Windows (via WSL2)

WSL2 (Windows Subsystem for Linux) lets you run a Linux environment directly on Windows, ensuring smoother compatibility with development tools.

**Step 1 — Install WSL2**

Open **PowerShell** as Administrator (right-click Start → Windows PowerShell (Admin) or Terminal (Admin)) and run:

```powershell
wsl --install
```

Restart your computer if prompted. After reboot, an Ubuntu terminal window will appear for you to set up a Linux `username` and `password`.

**Step 2 — Update Ubuntu**

Open the Ubuntu terminal (or run `wsl` from cmd/PowerShell) and run:

```bash
sudo apt update && sudo apt upgrade -y
```

**Step 3 — Install Node.js (latest) via NVM**

Using NVM (Node Version Manager) makes it easy to manage Node.js versions and avoids permission issues with global packages.

```bash
# Install NVM
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash

# Reload shell configuration
source ~/.bashrc

# Install and activate Node.js (latest)
nvm install node
nvm use node

# Verify installation (should print the latest version)
node -v
```

**Step 4 — Install and run DeepQuark**

```bash
npm install -g @duckmind/deepquark
deepquark
```

> If `deepquark` is not found, you can run it via npx: `npx @duckmind/deepquark`

---

### macOS

Installation on macOS is straightforward and works on both Apple Silicon (M1/M2/M3) and Intel chips.

**Step 1 — Install NVM**

Open **Terminal** (or iTerm2) and run:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash

# Reload shell configuration (macOS defaults to zsh)
source ~/.zshrc
```

**Step 2 — Install Node.js (latest)**

```bash
nvm install node
nvm use node

# Verify (should print the latest version)
node -v
```

**Step 3 — Install and run DeepQuark**

```bash
npm install -g @duckmind/deepquark
deepquark
```

---

### Linux (Ubuntu / Debian / Fedora / CentOS)

**Step 1 — Update your system**

For Ubuntu/Debian:

```bash
sudo apt update && sudo apt upgrade -y
```

For Fedora/CentOS:

```bash
sudo dnf update -y
```

**Step 2 — Install NVM and Node.js (latest)**

```bash
# Install NVM
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash

# Reload shell configuration
source ~/.bashrc

# Install and activate Node.js (latest)
nvm install node
nvm use node

# Verify
node -v
```

**Step 3 — Install and run DeepQuark**

```bash
npm install -g @duckmind/deepquark
deepquark
```

---

## About DuckMind Team

DeepQuark is developed by **DuckMind Team**, with the mission of building AI systems that automate knowledge work, support programming and research, boost individual and organizational productivity, and connect AI with real-world tools.
